# Search: Person
This method parses search results from `https://myanimelist.net/people.php?q={query}`

**Response:** `\Jikan\Model\Search\PersonSearch`

## Usage: Legacy
**Arguments:** `string $query`, `int $page`
```
<?php
// Search results for "Sawashiro"
$personSearchResults = $jikan->PersonSearch("sawashiro");

// Search results from page 2
$personSearchResults = $jikan->PersonSearch("sawashiro", 2);

// There's no Advanced search (filters) for Person results
```

## Usage: Standard
**Argument:** `\Jikan\Request\Search\PersonSearchRequest`
```
<?php

$personSearchResults = $jikan->getPersonSearch(
    (new \Jikan\Request\Search\PersonSearchRequest("sawashiro"))
);
```

[^1]: Request: [\Jikan\Request\Search\PersonSearchRequest](/objects/request/search/person.md)
[^2]: Model: [\Jikan\Model\Search\PersonSearch](/objects/model/search/person.md)