---
layout: default
title: "icalBuddy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="icalbuddy">
  <a href="/en/osx/icalbuddy.html">icalBuddy</a> <a href="#icalbuddy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line utility for printing events and tasks from the macOS calendar database.
> More information: <https://hasseg.org/icalBuddy/>.

#### Show events later today:
```shell
icalBuddy -n eventsToday
```
#### Show uncompleted tasks:
```shell
icalBuddy uncompletedTasks
```
#### Show a formatted list separated by calendar for all events today:
```shell
icalBuddy -f -sc eventsToday
```
#### Show tasks for a specified number of days:
```shell
icalBuddy -n tasksDueBefore:today+{{days}}
```
#### Show events in a time range:
```shell
icalBuddy eventsFrom:'{{start_date}}' to:'{{end_date}}'
```
{% endraw %}