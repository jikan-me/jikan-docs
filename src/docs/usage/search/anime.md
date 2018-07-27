# Search: Anime
This method parses search results from `https://myanimelist.net/anime.php?q={query}`

**Response:** `\Jikan\Model\Search\AnimeSearch`

## Usage: Legacy
**Arguments:** `string $query`, `int $page`, `\Jikan\Request\Search\AnimeSearchRequest $request = NULL`
```
<?php
use \Jikan\Helper\Constants;

// Search results for "No Game No Life"
$animeSearchResults = $jikan->AnimeSearch("No Game No Life");

// Search results from page 2
$animeSearchResults = $jikan->AnimeSearch("No Game No Life", 2);

// Advanced Search (Filters)
// Only movies
$animeSearchResults = $jikan->AnimeSearch("No Game No Life", 1,
    (new \Jikan\Request\Search\AnimeSearchRequest())
        ->setType(Constants::SEARCH_FILTER_MOVIES);

// Search for anime movies WITHOUT any queries
// that have the genres `Fantasy` and `Adventure`
// that have ratings above 8
$animeSearchResults = $jikan->AnimeSearch(null, 1,
    (new \Jikan\Request\Search\AnimeSearchRequest())
        ->setType(Constants::SEARCH_FILTER_MOVIES)
        ->setGenre(Constants::GENRE_FANTASY, Constants::GENRE_ADVENTURE)
        ->setScore(8);
);
```

## Usage: Standard
**Argument:** `\Jikan\Request\Search\AnimeSearchRequest`
```
<?php

$animeSearchResults = $jikan->getAnimeSearch(
    (new \Jikan\Request\Search\AnimeSearchRequest("No Game No Life"));
);
```

[^1]: Request: [\Jikan\Request\Search\AnimeSearchRequest](/objects/request/search/anime.md)
[^2]: Model: [\Jikan\Model\Search\AnimeSearch](/objects/model/search/anime.md)