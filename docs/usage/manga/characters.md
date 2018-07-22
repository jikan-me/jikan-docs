This method parses item data by ID from `https://myanimelist.net/manga/{id}/_/characters`

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Manga\AnimeCharactersAndStaff` | `\Jikan\Model\Manga\CharacterListItem[]` |

## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Fetch Naruto's characters
// Request: https://myanimelist.net/manga/11/_/characters
$manga = $jikan->MangaCharacters(
    (new \Jikan\Request\Manga\MangaCharactersRequest(11))
);
```

[^1]: Request: [\Jikan\Request\Manga\MangaCharactersRequest](/objects/request/manga/characters-and-staff.md)
[^2]: Model: [\Jikan\Model\Manga\CharacterListItem](/objects/model/manga/character-list-item.md)