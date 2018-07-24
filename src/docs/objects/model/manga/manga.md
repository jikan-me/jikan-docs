## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Fetch Naruto's manga data
// Request: https://myanimelist.net/manga/11
$manga = $jikan->Manga(
    (new \Jikan\Request\Manga\MangaRequest(11))
);
```

## Methods
### `getMalId() : int`
**Description:** MyAnimeList ID

### `getUrl() : string`
**Description:** MyAnimeList URL

### `getImageUrl() : string`
**Description:** Image URL

### `getTitle() : string`
**Description:** Official title

### `getTitleEnglish() : ?string`
**Description:** English title

### `getTitleJapanese() : ?string`
**Description:** Japanese title

### `getTitleSynonyms() : string[]`
**Description:** Other titles

### `getType() : string`
**Description:** Item type, e.g `Manga`, `Manhwa`, `Novel`, etc

### `getChapters() : ?int`
**Description:** Chapter count, `null` if unknown

### `getVolumes() : ?int`
**Description:** Volume count, `null` if unknown

### `getStatus() : string`
**Description:** Item status, e.g `Currently Publishing`, `Finished`, etc

### `isPublishing() : bool`

### `getPublished() : DateRange`
**Description:** Returns [^2]`\Jikan\Model\DateRange`

### `getRating() : string`
**Description:** Item rating, e.g `PG`, `R17`, etc

### `getScore() : float`
**Description:** Item score

### `getScoredBy() : int`
**Description:** Number of users item scored by

### `getRank() : int`
**Description:** Item rank on MyAnimeList

### `getPopularity() : int`
**Description:** Item popularity on MyAnimeList

### `getMembers() : int`
**Description:** Item members on MyAnimeList

### `getFavorites() : int`
**Description:** Item favorites on MyAnimeList

### `getSynopsis() : string`

### `getBackground() : string`
**Description:** Background information

### `getBroadcast() : string`
**Description:** Day & Time item broadcasted on

### `getRelated() : array`
**Description:** Related items as [^1]`\Jikan\Model\MalUrl` in associative arrays with the keys as their respective relation

### `getAuthors() : MalUrl[]`
**Description:** Authors as [^1]`\Jikan\Model\MalUrl`

### `getSerializations() : MalUrl[]`
**Description:** Serializations as [^1]`\Jikan\Model\MalUrl`

### `getGenres() : MalUrl[]`
**Description:** Genres as [^1]`\Jikan\Model\MalUrl`

[^1]: [\Jikan\Model\MalUrl](/objects/misc/mal-url.md)
[^2]: [\Jikan\Model\DateRange](/objects/misc/date-range.md)