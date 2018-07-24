This method parses item data by ID from `https://myanimelist.net/manga/{id}`

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Manga\MangaRequest` | `\Jikan\Model\Manga\Manga` |

## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Fetch Naruto's manga data
// Request: https://myanimelist.net/manga/11
$manga = $jikan->Manga(
    (new \Jikan\Request\Manga\MangaRequest(11))
);
```

[^1]: Request: [\Jikan\Request\Manga\MangaRequest](/objects/request/manga/manga.md)
[^2]: Model: [\Jikan\Model\Manga\Manga](/objects/model/manga/manga.md)