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
### `getUrl() : string`
**Description:** Permalink URL to forum post

### `getAuthorName() : string`
**Description:** Author's name for the post

### `getAuthorUrl() : string`
**Description:** Author's profile URL for the post

### `getRelativeDate() : DateTimeImmutable`