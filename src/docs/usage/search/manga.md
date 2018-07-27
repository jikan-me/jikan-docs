# Search: Manga
This method parses search results from `https://myanimelist.net/manga.php?q={query}`

**Response:** `\Jikan\Model\Search\MangaSearch`

## Usage: Legacy
**Arguments:** `string $query`, `int $page`, `\Jikan\Request\Search\MangaSearchRequest $request = NULL`
```
<?php
use \Jikan\Helper\Constants;

// Search results for "Oyasumi Punpun"
$mangaSearchResults = $jikan->MangaSearch("Oyasumi Punpun");

// Search results from page 2
$mangaSearchResults = $jikan->MangaSearch("Oyasumi Punpun", 2);

// Advanced Search (Filters)
// Only manga
$mangaSearchResults = $jikan->MangaSearch("Oyasumi Punpun", 1,
    (new \Jikan\Request\Search\MangaSearchRequest())
        ->setType(Constants::SEARCH_FILTER_MANGA);

// Search for manga WITHOUT any queries
// that have the genres `Fantasy` and `Adventure`
// that have ratings above 8
$mangaSearchResults = $jikan->MangaSearch(null, 1,
    (new \Jikan\Request\Search\MangaSearchRequest())
        ->setType(Constants::SEARCH_FILTER_MANGA)
        ->setGenre(Constants::GENRE_FANTASY, Constants::GENRE_ADVENTURE)
        ->setScore(8);
);
```

## Usage: Standard
**Argument:** `\Jikan\Request\Search\MangaSearchRequest`
```
<?php

$mangaSearchResults = $jikan->getMangaSearch(
    (new \Jikan\Request\Search\MangaSearchRequest("Oyasumi Punpun"));
);
```

[^1]: Request: [\Jikan\Request\Search\MangaSearchRequest](/objects/request/search/manga.md)
[^2]: Model: [\Jikan\Model\Search\MangaSearch](/objects/model/search/manga.md)