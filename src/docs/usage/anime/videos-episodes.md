# Anime: Videos
This method parses item data by ID from `https://myanimelist.net/anime/{id}/_/video`

```
$data = $jikan->getAnimeVideosEpisodes(
    new \Jikan\Request\Anime\AnimeVideosEpisodesRequest(21, 2)
);

var_dump(
    $data->getResults()[0]->getTitle(),
    $data->getLastVisiblePage()
    // ...
);
```