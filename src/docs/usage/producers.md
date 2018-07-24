This method parses search results from `https://myanimelist.net/manga/producer/{id}`

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Producer\ProducerRequest` | `\Jikan\Model\Producer\Producer` |

## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Producer Production I.G
// Request: https://myanimelist.net/anime/producer/10
$animeByProducer = $jikan->Producer(
    (new \Jikan\Request\Producer\ProducerRequest())
);
```

[^1]: Request: [\Jikan\Request\Producer\ProducerRequest](/objects/request/producer/producer.md)
[^2]: Model: [\Jikan\Model\Producer\Producer](/objects/model/producer/producer.md)