This method parses item data by ID from `https://myanimelist.net/anime/{id}/_/characters`

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Anime\AnimeCharactersAndStaff` | `\Jikan\Model\Anime\AnimeCharactersAndStaff` |

## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Fetch One Piece's characters and staff
// Request: https://myanimelist.net/anime/21
$anime = $jikan->AnimeCharactersAndStaff(
    (new \Jikan\Request\Anime\AnimeCharactersAndStaffRequest(21))
);
```

[^1]: Request: [\Jikan\Request\Anime\AnimeCharactersAndStaffRequest](/objects/request/anime/characters-and-staff.md)
[^2]: Model: [\Jikan\Model\Anime\AnimeCharactersAndStaffRequest](/objects/model/anime/characters-and-staff.md)