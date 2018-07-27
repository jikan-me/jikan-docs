# Manga: News
This method parses item data by ID from `https://myanimelist.net/manga/{id}/_/news`

**Response:** `\Jikan\Model\News\NewsListItem[]`

## Usage: Legacy
**Arguments:** `int $id`
```
<?php

// Fetch news articles related to Naruto (MAL ID: 11) 
$news = $jikan->MangaNews(1);

foreach($news as $topic) {
    echo $topic->getTitle() . "\n";
    echo $topic->getIntro();

    echo "Author: " . $topic->getAuthor()->getName();
}
```

## Usage: Standard

**Arguments:** `\Jikan\Request\Manga\MangaNewsRequest`
```
<?php

$news = $jikan->getNewsList(
    (new \Jikan\Request\Manga\MangaNewsRequest(11))
);

foreach($news as $topic) {
    echo $topic->getTitle() . "\n";
    echo $topic->getIntro();

    echo "Author: " . $topic->getAuthor()->getName();
}
```


[^1]: [\Jikan\Request\Manga\MangaNewsRequest](/objects/request/manga/news)
[^2]: [\Jikan\Model\News\NewsListItem](/objects/model/news/news-list-item)