# User: History
This method parses user friends from `https://myanimelist.net/profile/{username}/friends`

**Response:** `\Jikan\Model\User\Friend[]`

## Usage: Legacy
**Argument:** `string $username`, `int $page`
```
<?php

// Friends: Nekomata1037
$userFriends = $jikan->UserFriends('nekomata1037');

// I don't have many friends so this will return empty :'(
$userFriends = $jikan->UserFriends('nekomata1037', 2);
```

## Usage: Standard
**Argument:** `\Jikan\Request\User\UserFriendsRequest`
```
<?php

$userFriends = $jikan->getUserFriends(
    (new \Jikan\Request\User\UserFriendsRequest('nekomata1037'))
);
```

[^1]: Request: [\Jikan\Request\User\UserFriendsRequest](/objects/request/user/friends.md)
[^2]: Model: [\Jikan\Model\User\Friend](/objects/model/user/friends.md)