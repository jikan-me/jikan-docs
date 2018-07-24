## Usage
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

## Methods
### `getMoreInfo() : ?string`
**Description:** More information related to Item