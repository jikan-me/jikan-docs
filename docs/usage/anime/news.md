## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Fetch news related to One Piece
// Request: https://myanimelist.net/anime/21/_/news
$news = $jikan->AnimeNews(
    (new \Jikan\Request\Anime\AnimeNewsRequest(21))
);

foreach($news as $topic) {
    echo $topic->getTitle() . "\n";
    echo $topic->getIntro();

    echo "Author: " . $topic->getAuthor()->getName();
}

```

## Methods
None. Refer to [^1]NewsListItem


[^1]: [\Jikan\Model\News\NewsListItem](/objects/model/common/news-list-item)