## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Fetch Seki, Tomokazu's data
// Request: https://myanimelist.net/people/1
$person = $jikan->Person(
    (new \Jikan\Request\Person\PersonRequest(1))
);

$animeStaffPositions = $person->getAnimeStaffPositions();
// get anime and position the person has worked on
foreach($animeStaffPositions as $staff) {
    echo "Worked on " . $staff->getAnimeMeta()->getName() . " as " . $staff->getPosition() . "\n";
}
```

## Methods
### `getPosition() : string`
**Description:** Position title

### `getAnimeMeta() : AnimeMeta`
**Description:** [^1]\Jikan\Model\Common\AnimeMeta

[^1]: [\Jikan\Model\Common\AnimeMeta](/objects/model/common/anime-meta.md)