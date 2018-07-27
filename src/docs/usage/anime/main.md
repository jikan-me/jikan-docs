# Anime: Main
This method parses item data by ID from `https://myanimelist.net/anime/{id}`

**Response:** `\Jikan\Model\Anime\Anime`

## Usage: Legacy
**Argument:** `int`
```
<?php

// Fetch One Piece's (MAL ID: 21) data from it's main page
$anime = $jikan->Anime(21);
```

## Usage: Standard
**Argument:** `\Jikan\Request\Anime\AnimeRequest`
```
<?php

$anime = $jikan->getAnime(
    (new \Jikan\Request\Anime\AnimeRequest(21))
);
```

[^1]: Request: [\Jikan\Request\Anime\AnimeRequest](/objects/request/anime/anime.md)
[^2]: Model: [\Jikan\Model\Anime\Anime](/objects/model/anime/anime.md)