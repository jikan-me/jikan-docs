## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Fetch topics related to One Piece
// Request: https://myanimelist.net/anime/21/_/forum
$topics = $jikan->AnimeForum(
    (new \Jikan\Request\Anime\AnimeForumRequest(21))
);

foreach($topics as $topic) {
    echo $topic->getTitle() . "\n";
    echo "Replies: " . $topic->getReplies();

    echo "Last post by: " . $topic->lastPost()->getAuthorName();
}
```

## Methods
### `getTopicId() : int`
**Description:** Topic MyAnimeList ID

### `getUrl() : string`
**Description:** Topic MyAnimeList URL

### `getTitle() : string`
**Description:** Topic title

### `getDatePosted() : DateTimeImmutable`

### `getAuthorName() : string`
**Description:** Name of the topic's author

### `getAuthorUrl() : string`
**Description:** Author's profile URL

### `getReplies() : int`
**Description:** Topic replies count

### `getLastPost() : \Jikan\Model\Forum\ForumPost`
**Description:** Returns [^1]`\Jikan\Model\Forum\ForumPost`

### `getImageUrl() : string`
**Description:** News image URL

### `getIntro() : string`
**Description:** News intro text

[^1]: [\Jikan\Model\Forum\ForumPost](/objects/model/forum/forum-post)