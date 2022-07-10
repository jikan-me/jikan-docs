# Anime: Characters And Staff
This method parses item data by ID from `https://myanimelist.net/anime/{id}/_/characters`

```
$data = $jikan->getAnimeCharactersAndStaff(
    new \Jikan\Request\Anime\AnimeCharactersAndStaffRequest(1)
);

var_dump(
    $data->getCharacters()[0]->getCharacter()->getName(), // first character's name
    $data->getStaff() // staff array
    // ...
);
```