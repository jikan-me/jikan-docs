## Usage

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Person\PersonPictures` | `\Jikan\Model\Common\Picture[]` |

```
<?php

$jikan = new Jikan\Jikan;

// Fetch pictures related to Seki, Tomokazu
// Request: https://myanimelist.net/Person/1/_/pics
$pics = $jikan->PersonPictures(
    (new \Jikan\Request\Person\PersonPicturesRequest(1))
);

foreach($pictures as $picture) {
    echo "<img src='" . $picture->getLarge() ."'>";
}

```

## Methods
None. Refer to [^1]\Jikan\Model\Common\Picture


[^1]: [\Jikan\Model\Common\Picture](/objects/model/common/picture)