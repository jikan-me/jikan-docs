# Anime: Pictures
This method parses item data by ID from `https://myanimelist.net/anime/{id}/_/pics`

```
$data = $jikan->getAnimePictures(
    new \Jikan\Request\Anime\AnimePicturesRequest(1)
);

var_dump(
    (string) $data[0]
    // ...
);
```