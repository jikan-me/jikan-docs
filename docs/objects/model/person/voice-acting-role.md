## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Fetch Seki, Tomokazu's data
// Request: https://myanimelist.net/people/1
$person = $jikan->Person(
    (new \Jikan\Request\Person\PersonRequest(1))
);

$voiceActingRoles = $person->getVoiceActingRoles();
// get character names the person has dubbed
foreach($voiceActingRoles as $role) {
    echo $role->getAnimeMeta()->getName() . "\n";
}
```

## Methods
### `getRole() : string`
**Description:** Role title

### `getAnimeMeta() : AnimeMeta`
**Description:** [^1]\Jikan\Model\Common\AnimeMeta

### `getCharacterMeta() : CharacterMeta`
**Description:** [^2]\Jikan\Model\Common\CharacterMeta

[^1]: [\Jikan\Model\Common\AnimeMeta](/objects/model/common/anime-meta.md)
[^2]: [\Jikan\Model\Common\CharacterMeta](/objects/model/common/character-meta.md)