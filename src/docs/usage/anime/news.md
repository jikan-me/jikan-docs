# Anime: News
This method parses item data by ID from `https://myanimelist.net/anime/{id}/_/news`

```
$data = $jikan->getNewsList(
    new \Jikan\Request\Anime\AnimeNewsRequest(1)
);

var_dump(
    $data->getResults()[0]->getTitle(),
    $data->getResults()[0]->getExcerpt(),
    $data->getLastVisiblePage(),
    $data->hasNextPage()
    // ...
);
```