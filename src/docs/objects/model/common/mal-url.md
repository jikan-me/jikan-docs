This class is basically a parse of links, e.g below 
```
<a href="https://myanimelist.com/type/id">Text Here</a>
```

## Methods
### `getMalId() : int`
**Description:** Extracts MyAnimeList ID from URL property

### `getType() : string`
**Description:** Gets URL type, e.g `anime`, `manga`, `user`, etc

### `getUrl() : string`
**Description:** Returns URL string

### `getName() : string`
**Description:** Returns associated string with URL

### `getTitle() : string`
**Description:** Alias of `getName()`