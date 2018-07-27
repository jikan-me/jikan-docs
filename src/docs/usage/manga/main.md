# Manga: Main
This method parses item data by ID from `https://myanimelist.net/manga/{id}`

**Response:** `\Jikan\Model\Manga\Manga`

## Usage: Legacy
**Argument:** `int`
```
<?php

// Fetch Naruto's (MAL ID: 11) data from it's main page
$manga = $jikan->Manga(11);
```

## Usage: Standard
**Argument:** `\Jikan\Request\Manga\MangaRequest`
```
<?php

$manga = $jikan->getManga(
    (new \Jikan\Request\Manga\MangaRequest(11))
);
```

[^1]: Request: [\Jikan\Request\Manga\MangaRequest](/objects/request/manga/manga.md)
[^2]: Model: [\Jikan\Model\Manga\Manga](/objects/model/manga/manga.md)