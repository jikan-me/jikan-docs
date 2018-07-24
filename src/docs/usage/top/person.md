This method parses search results from `https://myanimelist.net/person.php`

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Top\TopPeople` | `\Jikan\Model\Top\TopPerson[]` |

## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Top People listing
// Request: https://myanimelist.net/people.php
$topPeople = $jikan->TopPeople(
    (new \Jikan\Request\Top\TopPeople())
);
```

[^1]: Request: [\Jikan\Request\Top\TopPeople](/objects/request/top/person.md)
[^2]: Model: [\Jikan\Model\Top\TopPerson](/objects/model/top/person.md)