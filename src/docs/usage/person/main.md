# Person: Main
This method parses item data by ID from `https://myanimelist.net/people/{id}`

**Response:** `\Jikan\Model\Person\Person`

## Usage: Legacy
**Argument:** `int`
```
<?php

// Fetch Seki, Tomokazu's (MAL ID: 1) data from it's main page
$person = $jikan->Person(1);
```

## Usage: Standard
**Argument:** `\Jikan\Request\Person\PersonRequest`
```
<?php

$person = $jikan->getPerson(
    (new \Jikan\Request\Person\PersonRequest(1))
);
```

[^1]: Request: [\Jikan\Request\Person\PersonRequest](/objects/request/person/person.md)
[^2]: Model: [\Jikan\Model\Person\Person](/objects/model/person/person.md)