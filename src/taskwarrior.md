# Taskwarrior

## Dates

* `due` обозначает дату, после которой задачу выполнять уже нет смысла
  * `task +TODAY list` - фильтрует задачи, которые нужно сделать до сегодня, шорткат
  * `task due:today list`
  * `task +OVERDUE list` выведет просроченные задачи

* `scheduled` - когда станет возможно работать над задачей
  * В `task +READY list` попадают задачи без scheduled и для которых scheduled-дата прошла
  * В `+READY` не попадают задачи, которые зависят от других задач

То есть если у задачи есть сроки от-до, их можно проставить через scheduled-due

* `wait` - скрыть задачу из списка до указанной даты
  * `task waiting` - ждущие задачи, альтернатива `task +WAITING all`

* `until` - автоматически удалить задачу после этой даты

### Как выводить в отчете по умолчанию только `+READY` задачи

```
task config report.next.filter 'status:pending limit:page +READY'
```

`status:pending limit:page` уже было, мы добавили `+READY`. Чтобы посмотреть, что есть, можно сделать так:

```
task show report.next.filter
```
