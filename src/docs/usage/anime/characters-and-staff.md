# Anime: Characters And Staff
This method parses item data by ID from `https://myanimelist.net/anime/{id}/_/characters`

**Response:** `\Jikan\Model\Anime\AnimeCharactersAndStaff`

## Usage: Legacy
**Arguments:** `int $id`
```
<?php

// Fetch One Piece's (MAL ID: 21) characters & staff
$charactersAndStaff = $jikan->AnimeCharactersAndStaff(21);
```

## Usage: Standard

**Arguments:** `\Jikan\Request\Anime\AnimeCharactersAndStaffRequest`
```
<?php

$charactersAndStaff = $jikan->getAnimeCharactersAndStaff(
    (new \Jikan\Request\Anime\AnimeCharactersAndStaffRequest(21))
);
```

[^1]: Request: [\Jikan\Request\Anime\AnimeCharactersAndStaffRequest](/objects/request/anime/characters-and-staff.md)
[^2]: Model: [\Jikan\Model\Anime\AnimeCharactersAndStaff](/objects/model/anime/characters-and-staff.md)