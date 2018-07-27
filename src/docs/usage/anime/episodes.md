# Anime: Episodes
This method parses item data by ID from `https://myanimelist.net/anime/{id}/_/episode`

**Response:** `\Jikan\Model\Anime\AnimeEpisodes`

## Usage: Legacy
**Arguments:** `int $id`, `int $page`
```
<?php

// Fetch One Piece's (MAL ID: 21) episodse list
$episodes = $jikan->AnimeEpisodes(21);

// Episode lists are paginated if there's more than 100 episodes
// Thus to fetch episodes starting from 101: page 2
$episodes = $jikan->AnimeEpisodes(21, 2);
```

## Usage: Standard

**Arguments:** `\Jikan\Request\Anime\AnimeCharactersAndStaffRequest`
```
<?php

$episodes = $jikan->getAnimeEpisodes(
    (new \Jikan\Request\Anime\AnimeEpisodesRequest(21))
);
```

[^1]: Request: [\Jikan\Request\Anime\AnimeEpisodesRequest](/objects/request/anime/episodes)
[^2]: Model: [\Jikan\Model\Anime\AnimeEpisodes](/objects/model/anime/episodes)
