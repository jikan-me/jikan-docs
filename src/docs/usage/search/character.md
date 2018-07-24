This method parses search results from `https://myanimelist.net/character.php?q=`

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Search\CharacterSearchRequest` | `\Jikan\Model\Search\CharacterSearch` |

## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Search for "Lelouch"
// Request: https://myanimelist.net/character.php?q=Lelouch
$anime = $jikan->CharacterSearch(
    (new \Jikan\Request\Search\CharacterSearchRequest("lelouch"))
);
```

[^1]: Request: [\Jikan\Request\Search\CharacterSearchRequest](/objects/request/search/character.md)
[^2]: Model: [\Jikan\Model\Search\CharacterSearch](/objects/model/search/character.md)