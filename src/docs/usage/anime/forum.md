## Usage

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Anime\AnimeForum` | `\Jikan\Model\Forum\ForumTopic[]` |

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
None. Refer to [^1]ForumTopic


[^1]: [\Jikan\Model\Forum\ForumTopic](/objects/model/forum/forum-topic)