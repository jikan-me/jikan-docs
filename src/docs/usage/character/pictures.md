## Usage

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Character\CharacterPictures` | `\Jikan\Model\Common\Picture[]` |

```
<?php

$jikan = new Jikan\Jikan;

// Fetch pictures related to Spike Spiegel
// Request: https://myanimelist.net/character/1/_/pics
$pics = $jikan->CharacterPictures(
    (new \Jikan\Request\Character\CharacterPicturesRequest(1))
);

foreach($pictures as $picture) {
    echo "<img src='" . $picture->getLarge() ."'>";
}

```

## Methods
None. Refer to [^1]\Jikan\Model\Common\Picture


[^1]: [\Jikan\Model\Common\Picture](/objects/model/common/picture)