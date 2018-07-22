## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Fetch Seki, Tomokazu's data
// Request: https://myanimelist.net/people/1
$person = $jikan->Person(
    (new \Jikan\Request\Person\PersonRequest(1))
);

echo $person->getName();
```

## Methods
### `getMalId() : int`
**Description:** MyAnimeList ID

### `getUrl() : string`
**Description:** MyAnimeList URL

### `getImageUrl() : string`
**Description:** Image URL

### `getWebsiteUrl() : ?string`
**Description:** Website URL of person

### `getName() : string`
**Description:** Name

### `getGivenName() : string`

### `getFamilyName() : string`

### `getAlternativeNames() : string[]`

### `getBirthday() : ?DateTimeImmutable`

### `getMemberFavorites() : int`
**Description:** Count of MyAnimeList users favoriting this Person

### `getAbout() : string`
**Description:** Biography

### `getVoiceActingRoles() : VoiceActingRole[]`
**Description:** Voice acting roles for this Person. Returns array of [^1]`\Jikan\Model\Person\VoiceActingRole`

### `getAnimeStaffPositions() : AnimeStaffPosition[]`
**Description:** Anime staff positions for this Person. Returns array of [^2]`\Jikan\Model\Person\AnimeStaffPosition`

### `getPublishedManga() : PublishedManga[]`
**Description:** Published Manga by this Person. Returns array of [^3]`\Jikan\Model\Person\PublishedManga`

[^1]: [\Jikan\Model\Person\VoiceActingRole](/objects/model/person/voice-acting-role.md)
[^2]: [\Jikan\Model\Person\AnimeStaffPosition](/objects/model/person/anime-staff-position.md)
[^3]: [\Jikan\Model\Person\PublishedManga](/objects/model/person/published-manga.md)