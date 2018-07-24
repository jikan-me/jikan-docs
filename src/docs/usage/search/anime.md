This method parses search results from `https://myanimelist.net/anime.php?q=`

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Search\AnimeSearchRequest` | `\Jikan\Model\Search\AnimeSearch` |

## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Search for "No Game No Life"
// Request: https://myanimelist.net/anime.php?q=No Game No Life
$anime = $jikan->AnimeSearch(
    (new \Jikan\Request\Search\AnimeSearchRequest("No Game No Life"))
);
```

[^1]: Request: [\Jikan\Request\Search\AnimeSearchRequest](/objects/request/search/anime.md)
[^2]: Model: [\Jikan\Model\Search\AnimeSearch](/objects/model/search/anime.md)