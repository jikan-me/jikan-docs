# User: Profile
This method parses user profiles from `https://myanimelist.net/profile/{username}`

**Response:** `\Jikan\Model\User\Profile[]`

## Usage: Legacy
**Argument:** `string $username`
```
<?php

// Profile: Nekomata1037
$userProfile = $jikan->UserProfile('nekomata1037');
```

## Usage: Standard
**Argument:** `\Jikan\Request\User\UserProfileRequest`
```
<?php

$userProfile = $jikan->getUserProfile(
  new \Jikan\Request\User\UserProfileRequest('nekomata1037')
);
```

[^1]: Request: [\Jikan\Request\User\UserProfileRequest](/objects/request/user/profile.md)
[^2]: Model: [\Jikan\Model\User\TopAnime](/objects/model/user/profile.md)