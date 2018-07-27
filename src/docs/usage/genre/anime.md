# Genre: Anime
This method parses anime genres from `https://myanimelist.net/profile/anime/genre/{id}`

**Response:** `\Jikan\Model\Genre\AnimeGenre`

## Usage: Legacy
**Arguments:** `int $id`, `int $page`
```
<?php

// Action Anime (MAL ID: 1)
$actionAnime = $jikan->AnimeGenre(1);
```

## Usage: Standard
**Argument:** `\Jikan\Request\Genre\AnimeGenreRequest`
```
<?php

$actionAnime = $jikan->getAnimeGenre(
    (new \Jikan\Request\Genre\AnimeGenreRequest(1))
);
```

[^1]: Request: [\Jikan\Request\Genre\AnimeGenreRequest](/objects/request/genre/anime.md)
[^2]: Model: [\Jikan\Model\Genre\AnimeGenre](/objects/model/genre/anime.md)