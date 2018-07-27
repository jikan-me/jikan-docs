# Manga: Forum
This method parses item data by ID from `https://myanimelist.net/manga/{id}/_/forum`

**Response:** `\Jikan\Model\Forum\ForumTopic[]`

## Usage: Legacy
**Arguments:** `int $id`
```
<?php

// Fetch forum topics related to Naruto (MAL ID: 11) 
$topics = $jikan->MangaForum(1);

foreach($topics as $topic) {
    echo $topic->getTitle() . "\n";
    echo "Replies: " . $topic->getReplies();

    echo "Last post by: " . $topic->lastPost()->getAuthorName();
}
```

## Usage: Standard

**Arguments:** `\Jikan\Request\Manga\MangaForumRequest`
```
<?php

$topics = $jikan->getMangaForum(
    (new \Jikan\Request\Manga\MangaForumRequest(11))
);

foreach($topics as $topic) {
    echo $topic->getTitle() . "\n";
    echo "Replies: " . $topic->getReplies();

    echo "Last post by: " . $topic->lastPost()->getAuthorName();
}
```


[^1]: [\Jikan\Model\Forum\ForumTopic](/objects/model/forum/forum-topic)