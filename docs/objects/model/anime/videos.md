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

## Methods
### `getPromos() : PromoListItem[]`
**Description:** Returns an array of [^1]`\Jikan\Model\Anime\PromoListItem`


### `getEpisodes() : StreamEpisodeListItem[]`
**Description:** Returns an array of [^2]`\Jikan\Model\Anime\StreamEpisodeListItem`


[^1]: [\Jikan\Model\Anime\PromoListItem](/objects/model/anime/promo-list-item)
[^2]: [\Jikan\Model\Anime\StreamEpisodeListItem](/objects/model/anime/stream-episode-list-item)