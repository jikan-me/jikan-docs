# Anime: Videos
This method parses item data by ID from `https://myanimelist.net/anime/{id}/_/video`

**Response:** `\Jikan\Model\Anime\AnimeVideos`

## Usage: Legacy
**Arguments:** `int $id`
```
<?php

// Fetch episodes & promo videos related to One Piece (MAL ID: 21)
$videos = $jikan->AnimeVideos(1);

// Episodes
var_dump(
    $videos->getEpisodes()
);

// Promo Videos
var_dump(
    $videos->getPromos()
);
```

## Usage: Standard

**Arguments:** `\Jikan\Request\Anime\AnimeVideos`
```
<?php

$videos = $jikan->getAnimeVideos(
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
