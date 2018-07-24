This method parses search results from `https://myanimelist.net/profile/{username}/friends`

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\User\UserFriendsRequest` | `\Jikan\Model\User\Friend[]` |

## Usage
```
<?php

$jikan = new Jikan\Jikan;

// User friends
// Request: https://myanimelist.net/profile/nekomata1037/friends
$friends = $jikan->UserFriends(
    (new \Jikan\Request\User\UserFriendsRequest("nekomata1037))
);
```

[^1]: Request: [\Jikan\Request\User\UserFriendsRequest](/objects/request/user/friends.md)
[^2]: Model: [\Jikan\Model\User\Friend](/objects/model/user/friends.md)