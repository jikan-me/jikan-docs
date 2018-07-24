This method parses search results from `https://myanimelist.net/profile/{anime/genre/{id}`

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Genre\MangaGenre` | `\Jikan\Model\Genre\MangaGenre` |

## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Action Manga
// Request: https://myanimelist.net/manga/genre/1
$actionManga = $jikan->MangaGenre(
    (new \Jikan\Request\Genre\MangaGenreRequest(1))
);
```

[^1]: Request: [\Jikan\Request\Genre\MangaGenreRequest](/objects/request/genre/manga.md)
[^2]: Model: [\Jikan\Model\Genre\MangaGenre](/objects/model/genre/manga.md)