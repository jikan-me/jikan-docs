# Manga: More Info
This method parses item data by ID from `https://myanimelist.net/manga/{id}/_/moreinfo`

**Response:** `string`

## Usage: Legacy
**Arguments:** `int $id`
```
<?php

// More/Misc Info on Naruto (MAL ID: 21) 
echo $jikan->MangaMoreInfo(11);
```

## Usage: Standard

**Arguments:** `\Jikan\Request\Manga\MangaMoreInfoRequest`
```
<?php

echo $jikan->getMangaMoreInfo(
    (new \Jikan\Request\Manga\MangaMoreInfoRequest(11))
);
```

[^1]: Request: [\Jikan\Request\Manga\MangaMoreInfo](/objects/request/manga/more-info.md)
[^2]: Model: [\Jikan\Model\Manga\MangaMoreInfo](/objects/model/manga/more-info.md)