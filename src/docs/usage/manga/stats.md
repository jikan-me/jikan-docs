This method parses item data by ID from `https://myanimelist.net/manga/{id}`

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Manga\MangaStats` | `\Jikan\Model\Manga\MangaStats` |

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

[^1]: Request: [\Jikan\Request\Manga\MangaStatsRequest](/objects/request/manga/stats.md)
[^2]: Model: [\Jikan\Model\Manga\MangaStats](/objects/model/manga/stats.md)