# Top: Anime
This method parses top anime from `https://myanimelist.net/topanime.php`

**Response:** `\Jikan\Model\Top\TopAnime[]`

## Usage: Legacy
**Arguments:** `int $page`, `string $type`
```
<?php
use \Jikan\Helper\Constants;

// Top anime
$topAnime = $jikan->TopAnime();

// Top anime page 2
$topAnime = $jikan->TopAnime(2);

// Top upcoming manga
$topAnime = $jikan->TopAnime(1, Constants::TOP_UPCOMING);

// Top anime movies
$topAnime = $jikan->TopAnime(1, Constants::TOP_MOVIES);
```

## Usage: Standard
**Argument:** `\Jikan\Request\Top\TopAnimeRequest`
```
<?php
use \Jikan\Helper\Constants;

$topAnime = $jikan->getTopAnime(
    (new \Jikan\Request\Top\TopAnimeRequest(
        1,
        Constants::TOP_UPCOMING
    ))
);
```

[^1]: Request: [\Jikan\Request\Top\TopAnime](/objects/request/top/anime.md)
[^2]: Model: [\Jikan\Model\Top\TopAnime](/objects/model/top/anime.md)