# Top: Characters
This method parses top manga from `https://myanimelist.net/people.php`

**Response:** `\Jikan\Model\Top\TopPerson[]`

## Usage: Legacy
**Arguments:** `int $page`
```
<?php
// Top people
$topPeople = $jikan->TopPeople();

// Top people page 2
$topPeople = $jikan->TopPeople(1);
```

## Usage: Standard
**Argument:** `\Jikan\Request\Top\TopPeopleRequest`
```
<?php

$topPeople = $jikan->getTopPeople(
    (new \Jikan\Request\Top\TopPeopleRequest())
);
```

[^1]: Request: [\Jikan\Request\Top\TopPeople](/objects/request/top/person.md)
[^2]: Model: [\Jikan\Model\Top\TopPerson](/objects/model/top/person.md)