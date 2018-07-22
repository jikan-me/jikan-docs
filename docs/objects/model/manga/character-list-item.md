## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Fetch Naruto's characters
// Request: https://myanimelist.net/manga/11/_/characters
$characters = $jikan->MangaCharacters(
    (new \Jikan\Request\Manga\MangaCharactersRequest(11))
);

// echo all character names
foreach ($characters as $character) {
    echo $character->getName() . "\n";
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
**Description:** Characters's name

### `getRole() : string`
**Description:** Character's role