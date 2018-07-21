## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Fetch One Piece's data
// Request: https://myanimelist.net/anime/21
$anime = $jikan->Anime(
    (new \Jikan\Request\Anime\AnimeRequest(21))
);

$aired = $anime->getAired();
echo $aired->getAiredString();

// check if anime has aired
if (is_null($aired->getFrom())) {
    echo $anime->getTitle() . " has NOT aired yet";
}
```

This class is basically a parse of links, e.g below 
```
<a href="https://myanimelist.com/type/id">Text Here</a>
```

## Methods
### `getMalId() : int`
**Description:** Extracts MyAnimeList ID from URL property

### `getType() : string`
**Description:** Gets URL type, e.g `anime`, `manga`, `user`, etc

### `getUrl() : string`
**Description:** Returns URL string

### `getName() : string`
**Description:** Returns associated string with URL