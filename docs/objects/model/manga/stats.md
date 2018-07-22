## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Fetch Naruto's manga stats
// Request: https://myanimelist.net/manga/11/_/stats
$manga = $jikan->MangaStats(
    (new \Jikan\Request\Manga\MangaStatsRequest(11))
);

echo "Watching: " . $manga->getWatching();
echo "Rated 10/10: " . $manga->getScores()[10]->getVotes();
echo "Rated 1/10: " . $manga->getScores()[1]->getVotes();
```

## Methods
### `getReading() : int`
**Description:** Count of MyAnimeList users currently reading

### `getCompleted() : int`
**Description:** Count of MyAnimeList users completed

### `getOnHold() : int`
**Description:** Count of MyAnimeList users on hold

### `getDropped() : int`
**Description:** Count of MyAnimeList users who've dropped

### `getPlanToRead() : int`
**Description:** Count of MyAnimeList users planning to read

### `getTotal() : int`
**Description:** Count of total MyAnimeList users with statuses set for this item

### `getScores() : array`
**Description:** Scores by MyAnimeList users with array indexes 1-10