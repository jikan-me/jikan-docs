This method parses search results from `https://myanimelist.net/profile/{anime/genre/{id}`

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Genre\AnimeGenre` | `\Jikan\Model\Genre\AnimeGenre` |

## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Action Anime
// Request: https://myanimelist.net/anime/genre/1
$actionAnime = $jikan->AnimeGenre(
    (new \Jikan\Request\Genre\AnimeGenreRequest(1))
);
```

[^1]: Request: [\Jikan\Request\Genre\AnimeGenreRequest](/objects/request/genre/anime.md)
[^2]: Model: [\Jikan\Model\Genre\AnimeGenre](/objects/model/genre/anime.md)