# Genre: Manga
This method parses manga genres from `https://myanimelist.net/profile/manga/genre/{id}`

**Response:** `\Jikan\Model\Genre\MangaGenre`

## Usage: Legacy
**Arguments:** `int $id`, `int $page`
```
<?php

// Action Manga (MAL ID: 1)
$actionManga = $jikan->MangaGenre(1);
```

## Usage: Standard
**Argument:** `\Jikan\Request\Genre\MangaGenreRequest`
```
<?php

$actionManga = $jikan->getMangaGenre(
    (new \Jikan\Request\Genre\MangaGenreRequest(1))
);
```

[^1]: Request: [\Jikan\Request\Genre\MangaGenreRequest](/objects/request/genre/manga.md)
[^2]: Model: [\Jikan\Model\Genre\MangaGenre](/objects/model/genre/manga.md)