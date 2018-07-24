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
### `getUrl() : string`
**Description:** News MyAnimeList URL

### `getTitle() : string`
**Description:** News title

### `getDate() : DateTimeImmutable`

### `getAuthor() : \Jikan\Model\Common\MalUrl`
**Description:** Returns [^1]`\Jikan\Model\Common\MalUrl`

### `getForumUrl() : string`
**Description:** Related forum topic MyAnimeList URL

### `getImageUrl() : string`
**Description:** News image URL

### `getIntro() : string`
**Description:** News intro text

[^1]: [\Jikan\Model\Common\MalUrl](/objects/model/common/mal-url)