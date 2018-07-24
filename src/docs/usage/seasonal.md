This method parses search results from `https://myanimelist.net/anime/season`

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Seasonal\SeasonalRequest` | `\Jikan\Model\Seasonal\Seasonal` |

## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Anime this season
// Request: https://myanimelist.net/anime/season
$season = $jikan->Seasonal(
    (new \Jikan\Request\Seasonal\SeasonalRequest(
        2017,
        \Jikan\Helper\Constants::WINTER
    ))
);
```

[^1]: Request: [\Jikan\Request\Seasonal\SeasonalRequest](/objects/request/schedule/seasonal.md)
[^2]: Model: [\Jikan\Model\Seasonal\Producer](/objects/model/schedule/seasonal.md)