## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Fetch pictures related to One Piece
// Request: https://myanimelist.net/anime/21/_/moreinfo
$anime = $jikan->AnimeMoreInfo(
    (new \Jikan\Request\Anime\AnimeMoreInfoRequest(21))
);

echo $anime->getMoreInfo();
```

## Methods
### `getMoreInfo() : ?string`
**Description:** More information related to Item