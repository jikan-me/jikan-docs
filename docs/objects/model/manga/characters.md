## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Fetch One Piece's characters and staff
// Request: https://myanimelist.net/anime/21
$anime = $jikan->AnimeCharactersAndStaff(
    (new \Jikan\Request\Anime\AnimeCharactersAndStaffRequest(21))
);
var_dump(
    $anime->getCharacters()
);
```

## Methods
### `getCharacters() : CharacterListItem[]`
**Description:** Returns an array of [^1]`\Jikan\Model\Character\CharacterListItem`

[^1]: [\Jikan\Model\Manga\CharacterListItem](/objects/model/manga/character-list-item)