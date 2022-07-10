# Anime: More Info
This method parses item data by ID from `https://myanimelist.net/anime/{id}/_/moreinfo`

```
<?php

echo $jikan->getAnimeMoreInfo(
    (new \Jikan\Request\Anime\AnimeMoreInfoRequest(21))
);
```
