# Person: Pictures
This method parses item data by ID from `https://myanimelist.net/people/{id}/_/pictures`

**Response** [^1]`\Jikan\Model\Common\Picture[]`

## Usage: Legacy
**Arguments:** `int $id`
```
<?php

// Fetch pictures related to Spike Spiegel (MAL ID: 1)
$pics = $jikan->PersonPictures(1);

foreach($pictures as $picture) {
    echo "<img src='" . $picture->getLarge() ."'>";
}
```

## Usage: Standard

**Arguments:** `\Jikan\Request\Person\PersonPictures`
```
<?php

$pics = $jikan->getPersonPictures(
    (new \Jikan\Request\Person\PersonPicturesRequest(1))
);

foreach($pictures as $picture) {
    echo "<img src='" . $picture->getLarge() ."'>";
}
```


[^1]: [\Jikan\Model\Common\Picture](/objects/model/common/picture)