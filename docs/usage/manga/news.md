## Usage

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Manga\MangaNews` | `\Jikan\Model\News\NewsListItem[]` |

```
<?php

$jikan = new Jikan\Jikan;

// Fetch news related to Naruto manga
// Request: https://myanimelist.net/manga/21/_/news
$news = $jikan->MangaNews(
    (new \Jikan\Request\Manga\MangaNewsRequest(11))
);

foreach($news as $topic) {
    echo $topic->getTitle() . "\n";
    echo $topic->getIntro();

    echo "Author: " . $topic->getAuthor()->getName();
}

```

## Methods
None. Refer to [^1]NewsListItem


[^1]: [\Jikan\Model\News\NewsListItem](/objects/model/news/news-list-item)