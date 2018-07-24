This method parses search results from `https://myanimelist.net/manga/magazine/{id}`

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Magazine\MagazineRequest` | `\Jikan\Model\Magazine\Magazine` |

## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Magazine Shounen Jump Weekly
// Request: https://myanimelist.net/manga/magazine/83
$mangaByMagazine = $jikan->Magazine(
    (new \Jikan\Request\Magazine\MagazineRequest())
);
```

[^1]: Request: [\Jikan\Request\Magazine\MagazineRequest](/objects/request/magazine/magazine.md)
[^2]: Model: [\Jikan\Model\Magazine\Magazine](/objects/model/magazine/magazine.md)