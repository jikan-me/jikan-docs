# Anime: Stats
This method parses item data by ID from `https://myanimelist.net/anime/{id}/_/stats`

```
$data = $jikan->getAnimeStats(
    new \Jikan\Request\Anime\AnimeStatsRequest(1)
);

var_dump(
    $data->getCompleted(),
    $data->getWatching(),
    $data->getScores()[0]->getVotes()
    // ...
);
```