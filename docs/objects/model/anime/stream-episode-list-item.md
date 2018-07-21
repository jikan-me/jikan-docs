## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Fetch videos of Cowbow Bepop
// Request: https://myanimelist.net/anime/1/_/video
$videos = $jikan->AnimeVideos(
    (new \Jikan\Request\Anime\AnimeVideosRequest(1))
);

// Streamable Episodes
$episodes = $videos->getEpisodes();

foreach($episodes as $episode) {
    echo $episode->getTitle() . "\n";
}
```

## Methods
### `getImageUrl() : string`
**Description:** Episode thumbnail image URL

### `getUrl() : string`
**Description:** Episode MyAnimeList URL

### `getTitle() : string`
**Description:** Episode title

### `getEpisode() : string`
**Description:** Episode title/number