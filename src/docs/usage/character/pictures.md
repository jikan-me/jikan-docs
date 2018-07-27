# Character: Pictures
This method parses item data by ID from `https://myanimelist.net/character/{id}/_/pictures`

**Response** [^1]`\Jikan\Model\Common\Picture[]`

## Usage: Legacy
**Arguments:** `int $id`
```
<?php

// Fetch pictures related to Spike Spiegel (MAL ID: 1)
$pics = $jikan->CharacterPictures(1);

foreach($pictures as $picture) {
    echo "<img src='" . $picture->getLarge() ."'>";
}
```

## Usage: Standard

**Arguments:** `\Jikan\Request\Character\CharacterPicturesRequest`
```
<?php

$pics = $jikan->getCharacterPictures(
    (new \Jikan\Request\Character\CharacterPicturesRequest(1))
);

foreach($pictures as $picture) {
    echo "<img src='" . $picture->getLarge() ."'>";
}
```


[^1]: [\Jikan\Model\Common\Picture](/objects/model/common/picture)