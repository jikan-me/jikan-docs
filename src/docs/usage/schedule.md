# Seasonal
This method parses anime schedule from `https://myanimelist.net/anime/season/schedule`


**Response:** `\Jikan\Model\Schedule\Schedule`

## Usage: Legacy
**Arguments:** None
```
<?php

// Weekly Anime Schedule
$schedule = $jikan->getSchedule();
```

## Usage: Standard
**Argument:** `\Jikan\Request\Schedule\ScheduleRequest`
```
<?php
$schedule = $jikan->getSchedule(
    (new \Jikan\Request\Schedule\ScheduleRequest())
);
```

[^1]: Request: [\Jikan\Request\Schedule\ScheduleRequest](/objects/request/schedule/schedule.md)
[^2]: Model: [\Jikan\Model\Schedule\Producer](/objects/model/schedule/schedule.md)