This method parses search results from `https://myanimelist.net/character.php`

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Top\TopCharacters` | `\Jikan\Model\Top\TopCharacter[]` |

## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Top Characters listing
// Request: https://myanimelist.net/character.php
$topCharacters = $jikan->TopCharacters(
    (new \Jikan\Request\Top\TopCharacters())
);
```

[^1]: Request: [\Jikan\Request\Top\TopCharacters](/objects/request/top/character.md)
[^2]: Model: [\Jikan\Model\Top\TopCharacter](/objects/model/top/character.md)