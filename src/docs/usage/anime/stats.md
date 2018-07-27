# Anime: Stats
This method parses item data by ID from `https://myanimelist.net/anime/{id}/_/stats`

**Response:** `\Jikan\Model\Anime\AnimeStats`

## Usage: Legacy
**Arguments:** `int $id`
```
<?php

// Fetch One Piece's (MAL ID: 21) stats
$stats = $jikan->AnimeStats(21);

echo "Watching: " . $stats->getWatching();
echo "Rated 10/10: " . $stats->getScores()[10]->getVotes();
echo "Rated 1/10: " . $stats->getScores()[1]->getVotes();
```

## Usage: Standard

**Arguments:** `\Jikan\Request\Anime\AnimeStatsRequest`
```
<?php

$stats = $jikan->getAnimeStats(
    (new \Jikan\Request\Anime\AnimeStatsRequest(21))
);

echo "Watching: " . $stats->getWatching();
echo "Rated 10/10: " . $stats->getScores()[10]->getVotes();
echo "Rated 1/10: " . $stats->getScores()[1]->getVotes();
```


[^1]: Request: [\Jikan\Request\Anime\AnimeStatsRequest](/objects/request/anime/stats.md)
[^2]: Model: [\Jikan\Model\Anime\AnimeStats](/objects/model/anime/stats.md)