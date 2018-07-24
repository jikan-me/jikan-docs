This method parses search results from `https://myanimelist.net/history/{username}`

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\User\UserHistoryRequest` | `\Jikan\Model\User\History[]` |

## Usage
```
<?php

$jikan = new Jikan\Jikan;

// User profile
// Request: https://myanimelist.net/history/nekomata1037
$user = $jikan->UserHistory(
    (new \Jikan\Request\User\UserHistoryRequest("nekomata1037))
);
```

[^1]: Request: [\Jikan\Request\User\UserHistoryRequest](/objects/request/user/history.md)
[^2]: Model: [\Jikan\Model\User\History](/objects/model/user/history.md)