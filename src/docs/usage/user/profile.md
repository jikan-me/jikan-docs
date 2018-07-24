This method parses search results from `https://myanimelist.net/profile/{username}`

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\User\UserProfileRequest` | `\Jikan\Model\User\UserProfile[]` |

## Usage
```
<?php

$jikan = new Jikan\Jikan;

// User profile
// Request: https://myanimelist.net/profile/nekomata1037
$user = $jikan->UserProfile(
    (new \Jikan\Request\User\UserProfileRequest("nekomata1037))
);
```

[^1]: Request: [\Jikan\Request\User\UserProfileRequest](/objects/request/user/profile.md)
[^2]: Model: [\Jikan\Model\User\TopAnime](/objects/model/user/profile.md)