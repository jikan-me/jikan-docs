This method parses search results from `https://myanimelist.net/topanime.php`

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Top\TopAnime` | `\Jikan\Model\Top\TopAnime[]` |

## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Top Upcoming Anime listing
// Request: https://myanimelist.net/topanime.php
$anime = $jikan->TopAnime(
    (new \Jikan\Request\Top\TopAnime(
        1,
        \Jikan\Helper\Constants::TOP_UPCOMING
    ))
);
```

[^1]: Request: [\Jikan\Request\Top\TopAnime](/objects/request/top/anime.md)
[^2]: Model: [\Jikan\Model\Top\TopAnime](/objects/model/top/anime.md)