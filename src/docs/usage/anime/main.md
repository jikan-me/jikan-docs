# Anime: Main
This method parses item data by ID from `https://myanimelist.net/anime/{id}`

```
<?php

$data = $jikan->getAnime(
    new \Jikan\Request\Anime\AnimeRequest(21)
);

var_dump(
    $data->getTitles()[0]->getTitle(),
    $data->getImages()->getJpg()->getLargeImageUrl(),
    $data->getSynopsis()
    // ...
);
```