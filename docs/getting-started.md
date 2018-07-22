## Instantiating
We get started by instantiating Jikan
```
<?php
use Jikan\Jikan;

$jikan = new Jikan;
```

!!! tip
    v2 has return types added everywhere, this enables you to autocomplete anything in your IDE



## Migration Notes
Jikan v2's usage is completely different from v1.

- All main methods in Jikan have to pass their respective `Jikan\Request` objects which hold request information. More onto that on the next page.
- Responses are returned as **PHP objects**, no longer as arrays
- Extended Requests **no longer** exist. They're now as seperate requests.
- All object properties are **private** and must be accessed via getters
- Date/Timestamps are now returned as `\DateTimeImmutable` objects
- Date ranges are returned as `\Jikan\Model\Common\DateRange`
- Common URLs are parsed as `\Jikan\Model\Common\MalUrl`

[^1]: [DateRange](/misc/date-range.md)
[^2]: [MalUrl]()