## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Fetch One Piece's characters and staff
// Request: https://myanimelist.net/anime/21
$anime = $jikan->AnimeCharactersAndStaff(
    (new \Jikan\Request\Anime\AnimeCharactersAndStaffRequest(21))
);

// echo all character names
$characters = $anime->getCharacters();
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

### `getVoiceActors() : string`
**Description:** Voice actors in an array as [^1]`\Jikan\Model\Character\VoiceActor`

[^1]: [\Jikan\Model\Character\VoiceActor](/objects/model/character/voice-actor)