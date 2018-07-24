This method parses search results from `https://myanimelist.net/topmanga.php`

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Top\TopManga` | `\Jikan\Model\Top\TopManga[]` |

## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Top Manga listing
// Request: https://myanimelist.net/topmanga.php
$manga = $jikan->TopManga(
    (new \Jikan\Request\Top\TopManga())
);
```

[^1]: Request: [\Jikan\Request\Top\TopManga](/objects/request/top/manga.md)
[^2]: Model: [\Jikan\Model\Top\TopManga](/objects/model/top/manga.md)