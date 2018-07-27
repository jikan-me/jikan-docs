# Anime: News
This method parses item data by ID from `https://myanimelist.net/anime/{id}/_/news`

**Response:** `\Jikan\Model\News\NewsListItem[]`

## Usage: Legacy
**Arguments:** `int $id`
```
<?php

// Fetch news articles related to One Piece (MAL ID: 21) 
$news = $jikan->AnimeNews(
    (new \Jikan\Request\Anime\AnimeNewsRequest(21))
);

foreach($news as $topic) {
    echo $topic->getTitle() . "\n";
    echo $topic->getIntro();

    echo "Author: " . $topic->getAuthor()->getName();
}
```

## Usage: Standard

**Arguments:** `\Jikan\Request\Anime\AnimeNewsRequest`
```
<?php

$news = $jikan->getNewsList(
    (new \Jikan\Request\Anime\AnimeNewsRequest(21))
);

foreach($news as $topic) {
    echo $topic->getTitle() . "\n";
    echo $topic->getIntro();

    echo "Author: " . $topic->getAuthor()->getName();
}
```


[^1]: [\Jikan\Model\News\NewsListItem](/objects/model/news/news-list-item)