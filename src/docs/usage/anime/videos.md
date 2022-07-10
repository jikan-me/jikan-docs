# Anime: Videos
This method parses item data by ID from `https://myanimelist.net/anime/{id}/_/video`

```
$data = $jikan->getAnimeVideos(
    new \Jikan\Request\Anime\AnimeVideosRequest(1)
);

var_dump(
    $data->getEpisodes()[0]->getTitle(),
    $data->getMusicVideos()[0]->getVideo()->getEmbedUrl(),
    $data->getPromos()[0]->getTrailer()->getImages()->getMaximumImageUrl()
    // ...
);
```