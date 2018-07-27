# Manga: Stats
This method parses item data by ID from `https://myanimelist.net/manga/{id}/_/stats`

**Response:** `\Jikan\Model\Manga\MangaStats`

## Usage: Legacy
**Arguments:** `int $id`
```
<?php

// Fetch Naruto's (MAL ID: 21) stats
$stats = $jikan->MangaStats(21);

echo "Reading: " . $stats->getReading();
echo "Rated 10/10: " . $stats->getScores()[10]->getVotes();
echo "Rated 1/10: " . $stats->getScores()[1]->getVotes();
```

## Usage: Standard

**Arguments:** `\Jikan\Request\Manga\MangaStatsRequest`
```
<?php

$stats = $jikan->getMangaStats(
    (new \Jikan\Request\Manga\MangaStatsRequest(11))
);

echo "Reading: " . $stats->getReading();
echo "Rated 10/10: " . $stats->getScores()[10]->getVotes();
echo "Rated 1/10: " . $stats->getScores()[1]->getVotes();
```

[^1]: Request: [\Jikan\Request\Manga\MangaStatsRequest](/objects/request/manga/stats.md)
[^2]: Model: [\Jikan\Model\Manga\MangaStats](/objects/model/manga/stats.md)