# Magazine
This method parses manga by magazines from `https://myanimelist.net/manga/magazine/{id}`


**Response:** `\Jikan\Model\Magazine\Magazine`

## Usage: Legacy
**Argument:** `int $id`, `int $page`
```
<?php

// Magazine Shounen Jump Weekly
$mangaByMagazine = $jikan->Magazine(83);
```

## Usage: Standard
**Argument:** `\Jikan\Request\Magazine\MagazineRequest`
```
<?php

$mangaByMagazine = $jikan->getMagazine(
    (new \Jikan\Request\Magazine\MagazineRequest(83))
);
```

[^1]: Request: [\Jikan\Request\Magazine\MagazineRequest](/objects/request/magazine/magazine.md)
[^2]: Model: [\Jikan\Model\Magazine\Magazine](/objects/model/magazine/magazine.md)