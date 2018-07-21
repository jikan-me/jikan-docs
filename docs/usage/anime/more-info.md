## Usage

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Anime\AnimeMoreInfo` | `\Jikan\Model\Anime\AnimeMoreInfo[]` |

```
<?php

$jikan = new Jikan\Jikan;

// Fetch pictures related to One Piece
// Request: https://myanimelist.net/anime/21/_/pics
$pics = $jikan->AnimePictures(
    (new \Jikan\Request\Anime\AnimePicturesRequest(21))
);

foreach($pictures as $picture) {
    echo "<img src='" . $picture->getLarge() ."'>";
}
```

## Methods
None. Refer to [^1]\Jikan\Model\Common\Picture


[^1]: [\Jikan\Model\Common\Picture](/objects/model/common/picture)