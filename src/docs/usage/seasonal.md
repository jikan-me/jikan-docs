# Seasonal
This method parses seasonal anime from `https://myanimelist.net/anime/season`


**Response:** `\Jikan\Model\Search\PersonSearch`

## Usage: Legacy
**Arguments:** `int $year`, `string $season`
```
<?php
use \Jikan\Helper\Constants;

// Anime this season
$season = $jikan->Seasonal();

// Anime from Winter 2017
$season = $jikan->Seasonal(2017, Constants::SEASON_WINTER);
```

## Usage: Standard
**Argument:** `\Jikan\Model\Seasonal\Seasonal`
```
<?php
use \Jikan\Helper\Constants;

$season = $jikan->getSeasonal(
    (new \Jikan\Request\Seasonal\SeasonalRequest(
        2017,
        Constants::WINTER
    ))
);
```

[^1]: Request: [\Jikan\Request\Seasonal\SeasonalRequest](/objects/request/schedule/seasonal.md)
[^2]: Model: [\Jikan\Model\Seasonal\Producer](/objects/model/schedule/seasonal.md)