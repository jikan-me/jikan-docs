## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Fetch One Piece's episodes
// Request: https://myanimelist.net/anime/21/_/episode
$anime = $jikan->AnimeEpisodes(
    (new \Jikan\Request\Anime\AnimeEpisodesRequest(21, 1))
);
var_dump(
    $anime->getEpisodes()
);
```

## Methods
### `getEpisodes() : EpisodeListItem[]`
**Description:** Returns an array of [^1]`\Jikan\Model\Anime\EpisodeListItem`


### `getEpisodesLastPage() : int`
**Description:** Number of pages for the episode list. There's 100 episodes per page. Anime with more than 100 episodes will be paginated.


[^1]: [\Jikan\Model\Anime\EpisodesListItem](/objects/model/anime/episode-list-item)