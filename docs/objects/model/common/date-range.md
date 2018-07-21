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

## Methods
### `getFrom() : ?DateTimeImmutable`

### `getUntil() : ?DateTimeImmutable`

### `getAiredString() : string`
**Description:** Raw parsed string from MyAnimeList