## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Fetch Spike Spiegel's data
// Request: https://myanimelist.net/character/1
$character = $jikan->Character(
    (new \Jikan\Request\Character\CharacterRequest(1))
);

echo $character->getName();
```

## Methods
### `getMalId() : int`
**Description:** MyAnimeList ID

### `getUrl() : string`
**Description:** MyAnimeList URL

### `getImageUrl() : string`
**Description:** Image URL

### `getName() : string`
**Description:** Name

### `getNameKanji() : ?string`
**Description:** Name in Kanji

### `getNicknames() : string[]`
**Description:** Nicknames

### `getAbout() : string`
**Description:** Biography

### `getMemberFavorites() : int`
**Description:** Count of MyAnimeList users favoriting this Character

### `getAnimeography() : Animeography[]`
**Description:** Anime this character was in. Returns array of [^1]`\Jikan\Model\Character\Animeography`

### `getMangaography() : Mangaography[]`
**Description:** Manga this character was in. Returns array of [^2]`\Jikan\Model\Character\Mangaography`

### `getVoiceActors() : Animeography[]`
**Description:** Voice actors for this Character. Returns array of [^3]`\Jikan\Model\Character\VoiceActor`

[^1]: [\Jikan\Model\Character\Animeography](/objects/model/character/animeography.md)
[^2]: [\Jikan\Model\Character\Mangaography](/objects/model/character/mangaography.md)
[^3]: [\Jikan\Model\Character\VoiceActor](/objects/model/character/voice-actor.md)