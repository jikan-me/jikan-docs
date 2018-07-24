## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Fetch One Piece's anime stats
// Request: https://myanimelist.net/anime/21/_/stats
$anime = $jikan->AnimeStats(
    (new \Jikan\Request\Anime\AnimeStatsRequest(21))
);

echo "Watching: " . $anime->getWatching();
echo "Rated 10/10: " . $anime->getScores()[10]->getVotes();
echo "Rated 1/10: " . $anime->getScores()[1]->getVotes();
```

## Methods
### `getWatching() : int`
**Description:** Count of MyAnimeList users currently watching

### `getCompleted() : int`
**Description:** Count of MyAnimeList users completed

### `getOnHold() : int`
**Description:** Count of MyAnimeList users on hold

### `getDropped() : int`
**Description:** Count of MyAnimeList users who've dropped

### `getPlanToWatch() : int`
**Description:** Count of MyAnimeList users planning to watch

### `getTotal() : int`
**Description:** Count of total MyAnimeList users with statuses set for this item

### `getScores() : array`
**Description:** Scores by MyAnimeList users with array indexes 1-10