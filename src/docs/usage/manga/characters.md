# Manga: Characters
This method parses item data by ID from `https://myanimelist.net/manga/{id}/_/characters`

**Response:** `\Jikan\Model\Manga\CharacterListItem[]`

## Usage: Legacy
**Arguments:** `int $id`
```
<?php

// Fetch Naruto's (MAL ID: 11) characters
$characters = $jikan->MangaCharacters(11);
```

## Usage: Standard

**Arguments:** `\Jikan\Request\Manga\AnimeCharactersAndStaff`
```
<?php

$characters = $jikan->getMangaCharacters(
    (new \Jikan\Request\Manga\MangaCharactersRequest(11))
);
```

[^1]: Request: [\Jikan\Request\Manga\MangaCharactersRequest](/objects/request/manga/characters.md)
[^2]: Model: [\Jikan\Model\Manga\CharacterListItem](/objects/model/manga/character-list-item.md)