## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Fetch One Piece's characters and staff
// Request: https://myanimelist.net/anime/21
$anime = $jikan->AnimeCharactersAndStaff(
    (new \Jikan\Request\Anime\AnimeCharactersAndStaffRequest(21))
);

// echo all character's dubbed languages
$characters = $anime->getCharacters();
foreach ($characters as $character) {
    echo $character->getName() . "\n";

    $voiceActors = $character->getVoiceActors();
    foreach ($voiceActors as $voiceActor) {
        echo $voiceActor->getLanguage() . "\n";
    }
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
**Description:** Voice Actor's name

### `getLanguage() : string`
**Description:** Dubbed language