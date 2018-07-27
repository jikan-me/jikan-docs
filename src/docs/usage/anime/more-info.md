# Anime: More Info
This method parses item data by ID from `https://myanimelist.net/anime/{id}/_/moreinfo`

**Response:** `string`

## Usage: Legacy
**Arguments:** `int $id`
```
<?php

// More/Misc Info on One Piece (MAL ID: 21) 
echo $jikan->AnimeMoreInfo(21);
```

## Usage: Standard

**Arguments:** `\Jikan\Request\Anime\AnimeMoreInfo`
```
<?php

echo $jikan->getAnimeMoreInfo(
    (new \Jikan\Request\Anime\AnimeMoreInfoRequest(21))
);
```

[^1]: Request: [\Jikan\Request\Anime\AnimeMoreInfo](/objects/request/anime/more-info.md)
[^2]: Model: [\Jikan\Model\Anime\AnimeMoreInfo](/objects/model/anime/more-info.md)