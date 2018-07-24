## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Fetch Seki, Tomokazu's data
// Request: https://myanimelist.net/people/1
$person = $jikan->Person(
    (new \Jikan\Request\Person\PersonRequest(1))
);

$publishedManga = $person->getPublishedManga();
// get manga and position the person has worked on
foreach($publishedManga as $staff) {
    echo "Worked on " . $staff->getMangaMeta()->getName() . " as " . $staff->getPosition() . "\n";
}
```

## Methods
### `getPosition() : string`
**Description:** Position title

### `getMangaMeta() : MangaMeta`
**Description:** [^1]\Jikan\Model\Common\MangaMeta

[^1]: [\Jikan\Model\Common\MangaMeta](/objects/model/common/manga-meta.md)