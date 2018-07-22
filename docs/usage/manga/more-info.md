## Usage

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Manga\MangaMoreInfo` | `\Jikan\Model\Manga\MangaMoreInfo` |

```
<?php

$jikan = new Jikan\Jikan;

// More Info related to Naruto manga
// Request: https://myanimelist.net/manga/11/_/moreinfo
$moreinfo = $jikan->MangaMoreInfo(
    (new \Jikan\Request\Manga\MangaMoreInfoRequest(11))
);

echo $moreinfo->getMoreInfo();
```

[^1]: Request: [\Jikan\Request\Manga\MangaMoreInfo](/objects/request/manga/more-info.md)
[^2]: Model: [\Jikan\Model\Manga\MangaMoreInfo](/objects/model/manga/more-info.md)