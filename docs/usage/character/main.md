This method parses item data by ID from `https://myanimelist.net/character/{id}`

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Character\CharacterRequest` | `\Jikan\Model\Character\Character` |

## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Fetch Spike Spiegel's data
// Request: https://myanimelist.net/character/1
$character = $jikan->Character(
    (new \Jikan\Request\Character\CharacterRequest(1))
);
```

[^1]: Request: [\Jikan\Request\Character\CharacterRequest](/objects/request/character/character.md)
[^2]: Model: [\Jikan\Model\Character\Character](/objects/model/character/character.md)