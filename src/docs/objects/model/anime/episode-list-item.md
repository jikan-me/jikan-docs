## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Fetch One Piece's episodes
// Request: https://myanimelist.net/anime/21/_/episode
$anime = $jikan->AnimeEpisodes(
    (new \Jikan\Request\Anime\AnimeEpisodesRequest(21, 1))
);

$episodes = $anime->getEpisodes();
// echo all episode titles
foreach ($episodes as $episode) {
    echo $episode->getTitle();
}
```

## Methods
### `getEpisodeId() : int`
**Description:** MyAnimeList Episode ID

### `getVideoUrl() : string`
**Description:** MyAnimeList episode URL

### `getForumUrl() : string`
**Description:** MyAnimeList forum topic URL

### `getTitle() : string`
**Description:** Episode title

### `getTitleJapanese() : string`
**Description:** Episode title in Japanese

### `getTitleRomanji() : string`
**Description:** Episode title in Romanji

### `getAired() : ?DateRange`
**Description:** Returns [^1]`\Jikan\Model\Common\DateRange`

### `isFiller() : bool`

### `isRecap() : bool`

[^1]: [\Jikan\Model\Common\DateRange](/objects/model/common/date-range)