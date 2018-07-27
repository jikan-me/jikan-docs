# Character: Main
This method parses item data by ID from `https://myanimelist.net/character/{id}`

**Response:** `\Jikan\Model\Character\Character`

## Usage: Legacy
**Argument:** `int`
```
<?php

// Fetch Spike Spiegel's (MAL ID: 1) data from it's main page
$character = $jikan->Character(1);
```

## Usage: Standard
**Argument:** `\Jikan\Request\Character\CharacterRequest`
```
<?php

$character = $jikan->getCharacter(
    (new \Jikan\Request\Character\CharacterRequest(1))
);
```

[^1]: Request: [\Jikan\Request\Character\CharacterRequest](/objects/request/character/character.md)
[^2]: Model: [\Jikan\Model\Character\Character](/objects/model/character/character.md)