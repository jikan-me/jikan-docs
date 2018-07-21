## Usage

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Anime\AnimeMoreInfo` | `\Jikan\Model\Anime\AnimeMoreInfo[]` |

```
<?php

$jikan = new Jikan\Jikan;

// Fetch pictures related to One Piece
// Request: https://myanimelist.net/anime/21/_/moreinfo
$anime = $jikan->AnimeMoreInfo(
    (new \Jikan\Request\Anime\AnimeMoreInfoRequest(21))
);

echo $anime->getMoreInfo();
```

[^1]: Request: [\Jikan\Request\Anime\AnimeMoreInfo](/objects/request/anime/more-info.md)
[^2]: Model: [\Jikan\Model\Anime\AnimeMoreInfo](/objects/model/anime/more-info.md)