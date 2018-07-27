# Top: Characters
This method parses top manga from `https://myanimelist.net/character.php`

**Response:** `\Jikan\Model\Top\TopCharacter[]`

## Usage: Legacy
**Arguments:** `int $page`
```
<?php
// Top characters
$topCharacters = $jikan->TopCharacters();

// Top characters page 2
$topCharacters = $jikan->TopCharacters(2);
```

## Usage: Standard
**Argument:** `\Jikan\Request\Top\TopCharactersRequest`
```
<?php

$topCharacters = $jikan->getTopCharacters(
    (new \Jikan\Request\Top\TopCharactersRequest())
);
```

[^1]: Request: [\Jikan\Request\Top\TopCharacters](/objects/request/top/character.md)
[^2]: Model: [\Jikan\Model\Top\TopCharacter](/objects/model/top/character.md)