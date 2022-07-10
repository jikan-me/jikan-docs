# Anime: Episodes
This method parses item data by ID from `https://myanimelist.net/anime/{id}/_/episode/1`

```
$data = $jikan->getAnimeEpisode(
    new \Jikan\Request\Anime\AnimeEpisodeRequest(1)
);

var_dump(
    $data->getTitle(),
    $data->getSynopsis(),
    $data->getAired(),
    $data->getDuration()
    // ...
);
```