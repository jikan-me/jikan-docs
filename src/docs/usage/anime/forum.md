# Anime: Forum
This method parses item data by ID from `https://myanimelist.net/anime/{id}/_/forum`

**Response:** `\Jikan\Model\Forum\ForumTopic[]`

## Usage: Legacy
**Arguments:** `int $id`
```
<?php

// Fetch forum topics related to One Piece (MAL ID: 21) 
$episodes = $jikan->AnimeForum(21);
```

## Usage: Standard

**Arguments:** `\Jikan\Request\Anime\AnimeForumRequest`
```
<?php

$topics = $jikan->getAnimeForum(
    (new \Jikan\Request\Anime\AnimeForumRequest(21))
);

foreach($topics as $topic) {
    echo $topic->getTitle() . "\n";
    echo "Replies: " . $topic->getReplies();

    echo "Last post by: " . $topic->lastPost()->getAuthorName();
}
```

[^1]: [\Jikan\Request\Anime\AnimeForumRequest](/objects/request/anime/forum)
[^2]: [\Jikan\Model\Forum\ForumTopic](/objects/model/forum/forum-topic)