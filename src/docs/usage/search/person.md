This method parses search results from `https://myanimelist.net/people.php?q=`

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Search\PersonSearchRequest` | `\Jikan\Model\Search\PersonSearch` |

## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Search for "sawashiro"
// Request: https://myanimelist.net/people.php?q=sawashiro
$anime = $jikan->PersonSearch(
    (new \Jikan\Request\Search\PersonSearchRequest("sawashiro"))
);
```

[^1]: Request: [\Jikan\Request\Search\PersonSearchRequest](/objects/request/search/person.md)
[^2]: Model: [\Jikan\Model\Search\PersonSearch](/objects/model/search/person.md)