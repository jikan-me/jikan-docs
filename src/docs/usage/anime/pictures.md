# Anime: Pictures
This method parses item data by ID from `https://myanimelist.net/anime/{id}/_/pics`

**Response:** `\Jikan\Model\Common\Picture[]`

## Usage: Legacy
**Arguments:** `int $id`
```
<?php

// Fetch pictures related to One Piece (MAL ID: 21)
$pics = $jikan->AnimePictures(21);
```

## Usage: Standard

**Arguments:** `\Jikan\Request\Anime\AnimePicturesRequest`
```
<?php

$pics = $jikan->getAnimePictures(
    (new \Jikan\Request\Anime\AnimePicturesRequest(21))
);

foreach($pictures as $picture) {
    echo "<img src='" . $picture->getLarge() ."'>";
}
```

[^1]: [\Jikan\Request\Anime\AnimePicturesRequest](/objects/request/anime/pictures)
[^2]: [\Jikan\Model\Common\Picture](/objects/model/common/picture)