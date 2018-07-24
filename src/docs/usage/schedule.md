This method parses search results from `https://myanimelist.net/anime/season/schedule`

| Argument | Response |
| -------- | -------- |
| `\Jikan\Request\Schedule\ScheduleRequest` | `\Jikan\Model\Schedule\Schedule` |

## Usage
```
<?php

$jikan = new Jikan\Jikan;

// Weekly Anime Schedule
// Request: https://myanimelist.net/anime/season/schedule
$schedule = $jikan->Schedule(
    (new \Jikan\Request\Schedule\ScheduleRequest())
);
```

[^1]: Request: [\Jikan\Request\Schedule\ScheduleRequest](/objects/request/schedule/schedule.md)
[^2]: Model: [\Jikan\Model\Schedule\Producer](/objects/model/schedule/schedule.md)