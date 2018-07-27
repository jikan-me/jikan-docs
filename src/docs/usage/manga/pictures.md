# Manga: Pictures
This method parses item data by ID from `https://myanimelist.net/manga/{id}/_/pics`

**Response:** `\Jikan\Model\Common\Picture[]`

## Usage: Legacy
**Arguments:** `int $id`
```
<?php

// Fetch pictures related to One Piece (MAL ID: 11)
$pics = $jikan->MangaPictures(11);

foreach($pictures as $picture) {
    echo "<img src='" . $picture->getLarge() ."'>";
}
```

## Usage: Standard

**Arguments:** `\Jikan\Request\Manga\MangaPicturesRequest`
```
<?php

$pics = $jikan->getMangaPictures(
    (new \Jikan\Request\Magna\MangaPicturesRequest(11))
);

foreach($pictures as $picture) {
    echo "<img src='" . $picture->getLarge() ."'>";
}
```
[^1]: [\Jikan\Request\Anime\AnimePicturesRequest](/objects/request/anime/pictures)
[^2]: [\Jikan\Model\Common\Picture](/objects/model/common/picture)