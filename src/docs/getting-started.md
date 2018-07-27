## Instantiating
So there's 2 ways to use Jikan and every usage page will include examples of both methods.
#### Legacy
This is how you used Jikan in v1 except it has one major difference. "Extended requests" are now separate requests.

```
<?php
require __DIR__ . '/vendor/autoload.php';
use Jikan\Jikan;

$jikan = new Jikan;
```

#### Standard
This is for advanced PHP developers and how Jikan is to be used. Furthermore it follows PSR2 standards. The Legacy method is a wrapper for `MalClient`.

```
<?php
require __DIR__ . '/vendor/autoload.php';
use Jikan\MyAnimeList\MalClient;

$jikan = new MalClient;
```



!!! tip
    v2 has type hints, code documentation and follows PSR2 standards strictly. This enables autocompletion in many IDEs.



## Migration Notes
Jikan v2's usage is completely different from v1.

- All methods in `MalClient` require their respective `Jikan\Request` object which hold request information.
- Responses are returned as **PHP objects**, no longer as arrays
- Extended Requests **no longer** exist. They're now as seperate requests.
- All object properties are **private** and must be accessed via getters
- Date/Timestamps are now returned as [^1]`\DateTimeImmutable` objects and are **always** in **Universal Time Coordinated (UTC)**
- Date ranges are returned as [^2]`\Jikan\Model\Common\DateRange`
- Common URLs are parsed as [^3]`\Jikan\Model\Common\MalUrl`

[^2]: [DateTimeImmutable](http://php.net/manual/en/class.datetimeimmutable.php)
[^2]: [DateRange](/object/model/common/date-range.md)
[^3]: [MalUrl](/object/model/common/mal-url.md)