# Timewarrior

* `timew start`
* `timew stop`
* `timew start 'Using tags', Software` - начать интервал с двумя указанными тегами
* `timew continue` - начать интервал с теми же тегами что последний

Тегам можно проставить описание в конфиге:
```
timew config tags.Software.description "Learning about new software"
```

Запись постфактум:
* `timew track 9:00 - 11:00 'Done something'`
* `timew track 9am for 2h 'Done something'`
* `timew track 9am to 12am 'Done something'`
* `timew track 2h before 12am 'Done something'`

Варианты записи интервалов можно посмотреть в `timew help interval`.


## Links

* [Official site](https://timewarrior.net/)
* [PDF Cheatsheet](https://github.com/mkluge/timewcs)
