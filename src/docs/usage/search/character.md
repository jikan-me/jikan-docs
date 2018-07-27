# Search: Character
This method parses search results from `https://myanimelist.net/character.php?q={query}`

**Response:** `\Jikan\Model\Search\CharacterSearch`

## Usage: Legacy
**Arguments:** `string $query`, `int $page`
```
<?php
// Search results for "Lelouch"
$characterSearchResults = $jikan->CharacterSearch("Lelouch");

// Search results from page 2
$characterSearchResults = $jikan->CharacterSearch("Lelouch", 2);

// There's no Advanced search (filters) for Character results
```

## Usage: Standard
**Argument:** `\Jikan\Request\Search\CharacterSearchRequest(`
```
<?php

$characterSearchResults = $jikan->getCharacterSearch(
    (new \Jikan\Request\Search\CharacterSearchRequest("lelouch"))
);
```

[^1]: Request: [\Jikan\Request\Search\CharacterSearchRequest](/objects/request/search/character.md)
[^2]: Model: [\Jikan\Model\Search\CharacterSearch](/objects/model/search/character.md)