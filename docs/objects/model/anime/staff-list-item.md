## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Fetch One Piece's characters and staff
// Request: https://myanimelist.net/anime/21
$anime = $jikan->AnimeCharactersAndStaff(
    (new \Jikan\Request\Anime\AnimeCharactersAndStaffRequest(21))
);

// echo all staff names
$people = $anime->getStaff();
foreach ($people as $person) {
    echo $person->getName() . "\n";
}

```

## Methods
### `getMalId() : int`
**Description:** MyAnimeList ID

### `getUrl() : string`
**Description:** MyAnimeList URL

### `getImageUrl() : string`
**Description:** Image URL

### `getName() : string`
**Description:** Person's name

### `getPositions() : string[]`
**Description:** Person's positions