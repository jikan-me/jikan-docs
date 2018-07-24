This method parses item data by ID from `https://myanimelist.net/anime/{id}/_/episode`

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Anime\AnimeEpisodesRequest` | `\Jikan\Model\Anime\AnimeEpisodes` |

## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Fetch One Piece's episodes
// Request: https://myanimelist.net/anime/21/_/episode
$anime = $jikan->AnimeEpisodes(
    (new \Jikan\Request\Anime\AnimeEpisodesRequest(21, 1))
);
var_dump(
    $anime->getEpisodes()
);
```

[^1]: Request: [\Jikan\Request\Anime\AnimeEpisodesRequest](/objects/request/anime/episodes)
[^2]: Model: [\Jikan\Model\Anime\AnimeEpisodes](/objects/model/anime/episodes)
