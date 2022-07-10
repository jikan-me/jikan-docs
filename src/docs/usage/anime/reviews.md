# Anime: Reviews
This method parses item data by ID from `https://myanimelist.net/anime/{id}/_/reviews`

```
$data = $jikan->getAnimeReviews(
    new \Jikan\Request\Anime\AnimeReviewsRequest(1)
);

var_dump(
    $data->getResults()[0]->getVotes(),
    $data->getResults()[0]->getReview(),
    $data->getResults()[0]->getEpisodesWatched(),
    // ...
);
```
