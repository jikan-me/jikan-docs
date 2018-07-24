This method parses search results from `https://myanimelist.net/manga.php?q=`

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Search\MangaSearchRequest` | `\Jikan\Model\Search\MangaSearch` |

## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Search for "Oyasumi Punpun"
// Request: https://myanimelist.net/manga.php?q=Oyasumi Punpun
$anime = $jikan->MangaSearch(
    (new \Jikan\Request\Search\MangaSearchRequest("Oyasumi Punpun"))
);
```

[^1]: Request: [\Jikan\Request\Search\MangaSearchRequest](/objects/request/search/manga.md)
[^2]: Model: [\Jikan\Model\Search\MangaSearch](/objects/model/search/manga.md)