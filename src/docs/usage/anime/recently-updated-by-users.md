# Anime: Recently Updated By Users
This method parses item data by ID from `https://myanimelist.net/anime/{id}/_/stats`

```
$data = $jikan->getAnimeRecentlyUpdatedByUsers(
    new \Jikan\Request\Anime\AnimeRecentlyUpdatedByUsersRequest(1)
);

var_dump(
    $data->getResults()[0]->getUser()->getUsername(),
    $data->getLastVisiblePage(),
    // ...
);
```
