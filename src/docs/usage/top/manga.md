# Top: Manga
This method parses top manga from `https://myanimelist.net/topmanga.php`

**Response:** `\Jikan\Model\Top\TopManga[]`

## Usage: Legacy
**Arguments:** `int $page`, `string $type`
```
<?php
use \Jikan\Helper\Constants;

// Top manga
$topManga = $jikan->TopManga();

// Top manga page 2
$topManga = $jikan->TopManga(2);

// Top favorited manga
$topManga = $jikan->TopManga(1, Constants::TOP_FAVORITES);

// ( ͡° ͜ʖ ͡°)
$topManga = $jikan->TopManga(1, Constants::TOP_DOUJINSHI);
```

## Usage: Standard
**Argument:** `\Jikan\Request\Top\TopMangaRequest`
```
<?php
use \Jikan\Helper\Constants;

$topManga = $jikan->getTopManga(
    (new \Jikan\Request\Top\TopMangaRequest(
        1,
        Constants::TOP_MANGA // excludes novels, manhwa, manhua, etc
    ))
);
```

[^1]: Request: [\Jikan\Request\Top\TopManga](/objects/request/top/manga.md)
[^2]: Model: [\Jikan\Model\Top\TopManga](/objects/model/top/manga.md)