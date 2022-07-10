# Anime: Forum
This method parses item data by ID from `https://myanimelist.net/anime/{id}/_/forum`

```
$topics = $jikan->getAnimeForum(
    (new \Jikan\Request\Anime\AnimeForumRequest(21))
);

foreach($topics as $topic) {
    echo $topic->getTitle() . "\n";
    echo "Replies: " . $topic->getReplies();

    echo "Last post by: " . $topic->lastPost()->getAuthorName();
}
```