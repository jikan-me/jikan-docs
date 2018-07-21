This method parses item data by ID from `https://myanimelist.net/anime/{id}/_/video`

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Anime\AnimeVideos` | `\Jikan\Model\Anime\AnimeVideos` |

## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Fetch videos of Cowbow Bepop
// Request: https://myanimelist.net/anime/1/_/video
$videos = $jikan->AnimeVideos(
    (new \Jikan\Request\Anime\AnimeVideosRequest(1))
);

// Episodes
var_dump(
    $videos->getEpisodes()
);

// Promo Videos
var_dump(
    $videos->getPromos()
);
```

[^1]: Request: [\Jikan\Request\Anime\AnimeVideosRequest](/objects/request/anime/videos)
[^2]: Model: [\Jikan\Model\Anime\AnimeVideos](/objects/model/anime/videos)
