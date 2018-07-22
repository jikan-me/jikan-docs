This method parses item data by ID from `https://myanimelist.net/anime/{id}`

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Anime\AnimeStats` | `\Jikan\Model\Anime\AnimeStats` |

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

[^1]: Request: [\Jikan\Request\Anime\AnimeStatsRequest](/objects/request/anime/stats.md)
[^2]: Model: [\Jikan\Model\Anime\AnimeStats](/objects/model/anime/stats.md)