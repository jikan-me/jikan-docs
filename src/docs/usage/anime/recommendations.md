# Anime: Recommendations
This method parses item data by ID from `https://myanimelist.net/anime/{id}/_/userrecs`

```
$data = $jikan->getAnimeRecommendations(
    new \Jikan\Request\Anime\AnimeRecommendationsRequest(1)
);

var_dump(
    $data[0]->getTitle(),
    $data[0]->getRecommendationCount(),
    $data[0]->getEntryMeta()->getUrl(),
    // ...
);
```
