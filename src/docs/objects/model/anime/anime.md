## Methods
### `getMalId() : int`
**Description:** MyAnimeList ID

### `getUrl() : string`
**Description:** MyAnimeList URL

### `getImageUrl() : string`
**Description:** Image URL

### `getPreviewVideoUrl() : string`
**Description:** Preview/Promo video embed URL

### `getTitle() : string`
**Description:** Official title

### `getTitleEnglish() : ?string`
**Description:** English title

### `getTitleJapanese() : ?string`
**Description:** Kanji title

### `getTitleSynonyms() : string[]`
**Description:** Other titles

### `getType() : string`
**Description:** Item type, e.g `TV`, `Movie`, `OVA`, etc

### `getSource() : string`
**Description:** Adaption source, e.g `Manga`, `Novel`, etc

### `getEpisodes() : ?int`
**Description:** Episode count, `null` if unknown

### `getImageUrl() : string`
**Description:** Other titles

### `getStatus() : string`
**Description:** Item status, e.g `Currently Airing`, `Finished Airing`, etc

### `isAiring() : bool`

### `getAired() : DateRange`
**Description:** Returns [^2]`\Jikan\Model\DateRange`

### `getDuration() : string`
**Description:** Episode duration

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

### `getPremiered() : string`
**Description:** Season & year

### `getBroadcast() : string`
**Description:** Day & Time item broadcasted on

### `getRelated() : array`
**Description:** Related items as [^1]`\Jikan\Model\MalUrl` in associative arrays with the keys as their respective relation

### `getProducers() : MalUrl[]`
**Description:** Producers as [^1]`\Jikan\Model\MalUrl`

### `getLicensors() : MalUrl[]`
**Description:** Licensors as [^1]`\Jikan\Model\MalUrl`

### `getStudios() : MalUrl[]`
**Description:** Studios as [^1]`\Jikan\Model\MalUrl`

### `getGenres() : MalUrl[]`
**Description:** Genres as [^1]`\Jikan\Model\MalUrl`

### `getProducers() : array`
**Description:** Producers as [^1]`\Jikan\Model\MalUrl`

### `getOpeningTheme() : string[]`

### `getEndingTheme() : string[]`

[^1]: [\Jikan\Model\MalUrl](/objects/misc/mal-url.md)
[^2]: [\Jikan\Model\DateRange](/objects/misc/date-range.md)