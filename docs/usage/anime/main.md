This method parses item data by ID from `https://myanimelist.net/anime/{id}`

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Anime\AnimeRequest` | `\Jikan\Model\Anime\Anime` |

## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Fetch One Piece's anime data
// Request: https://myanimelist.net/anime/21
$anime = $jikan->Anime(
    (new \Jikan\Request\Anime\AnimeRequest(21))
);
```

[^1]: Request: [\Jikan\Request\Anime\AnimeRequest](/objects/request/anime/anime.md)
[^2]: Model: [\Jikan\Model\Anime\Anime](/objects/model/anime/anime.md)