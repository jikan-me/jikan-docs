# Producer
This method parses anime by producers from `https://myanimelist.net/anime/producer/{id}`


**Response:** `\Jikan\Model\Producer\Producer`

## Usage: Legacy
**Argument:** `int $id`, `int $page`
```
<?php

// Producer Production I.G
$animeByProducer = $jikan->Producer(10);
```

## Usage: Standard
**Argument:** `\Jikan\Request\Producer\ProducerRequest`
```
<?php

$animeByProducer = $jikan->getProducer(
    (new \Jikan\Request\Producer\ProducerRequest(10))
);
```

[^1]: Request: [\Jikan\Request\Producer\ProducerRequest](/objects/request/producer/producer.md)
[^2]: Model: [\Jikan\Model\Producer\Producer](/objects/model/producer/producer.md)