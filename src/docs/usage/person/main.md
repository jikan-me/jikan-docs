This method parses item data by ID from `https://myanimelist.net/people/{id}`

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Person\PersonRequest` | `\Jikan\Model\Person\Person` |

## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Fetch Seki, Tomokazu's data
// Request: https://myanimelist.net/people/1
$person = $jikan->Person(
    (new \Jikan\Request\Person\PersonRequest(1))
);
```

[^1]: Request: [\Jikan\Request\Person\PersonRequest](/objects/request/person/person.md)
[^2]: Model: [\Jikan\Model\Person\Person](/objects/model/person/person.md)