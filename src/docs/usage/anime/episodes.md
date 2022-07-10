# Anime: Episodes
This method parses item data by ID from `https://myanimelist.net/anime/{id}/_/episode`

```
$data = $jikan->getAnimeEpisodes(
    new \Jikan\Request\Anime\AnimeEpisodesRequest(1)
);

var_dump(
    $data->getResults()[0]->getTitle(),
    $data->getLastVisiblePage(),
    $data->hasNextPage()
    // ...
);
```