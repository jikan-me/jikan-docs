# User: History
This method parses user history from `https://myanimelist.net/history/{username}`

**Response:** `\Jikan\Model\User\History[]`

## Usage: Legacy
**Argument:** `string $username`, `string $type = null`
```
<?php
use \Jikan\Helper\Constants;

// All history (anime and manga)
$userHistory = $jikan->UserHistory('nekomata1037');

// Anime history
$userHistory = $jikan->UserHistory('nekomata1037', Constants::ANIME);

// Manga history
$userHistory = $jikan->UserHistory('nekomata1037', Constants::MANGA);
```

## Usage: Standard
**Argument:** `\Jikan\Request\User\UserHistoryRequest`
```
<?php

$userHistory = $jikan->getUserHistory(
    (new \Jikan\Request\User\UserHistoryRequest('nekomata1037'))
);
```

[^1]: Request: [\Jikan\Request\User\UserHistoryRequest](/objects/request/user/history.md)
[^2]: Model: [\Jikan\Model\User\History](/objects/model/user/history.md)