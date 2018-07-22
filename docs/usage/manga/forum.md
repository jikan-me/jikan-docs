## Usage

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Manga\MangaForum` | `\Jikan\Model\Forum\ForumTopic[]` |

```
<?php

$jikan = new Jikan\Jikan;

// Fetch topics related to Naruto manga
// Request: https://myanimelist.net/manga/11/_/forum
$topics = $jikan->MangaForum(
    (new \Jikan\Request\Manga\MangaForumRequest(11))
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