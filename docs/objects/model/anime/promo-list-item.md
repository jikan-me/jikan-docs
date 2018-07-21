## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Fetch videos of Cowbow Bepop
// Request: https://myanimelist.net/anime/1/_/video
$videos = $jikan->AnimeVideos(
    (new \Jikan\Request\Anime\AnimeVideosRequest(1))
);

// Promo Video Titles
$promos = $videos->getPromos();

foreach($promos as $promo) {
    echo $promo->getTitle() . "\n";
}
```

## Methods
### `getTitle() : string`
**Description:** Promo video title

### `getImageUrl() : string`
**Description:** Promo thumbnail image URL

### `getVideoUrl() : string`
**Description:** Promo video URL