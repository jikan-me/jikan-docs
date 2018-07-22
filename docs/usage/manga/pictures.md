## Usage

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Manga\MangaPictures` | `\Jikan\Model\Common\Picture[]` |

```
<?php

$jikan = new Jikan\Jikan;

// Fetch pictures related to Naruto
// Request: https://myanimelist.net/manga/11/_/pics
$pics = $jikan->MangaPictures(
    (new \Jikan\Request\Magna\MangaPicturesRequest(1))
);

foreach($pictures as $picture) {
    echo "<img src='" . $picture->getLarge() ."'>";
}

```

## Methods
None. Refer to [^1]\Jikan\Model\Common\Picture


[^1]: [\Jikan\Model\Common\Picture](/objects/model/common/picture)