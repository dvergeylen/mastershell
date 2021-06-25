---
layout: default
title: "gcalcli"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gcalcli">
  <a href="/en/common/gcalcli.html">gcalcli</a> <a href="#gcalcli"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line tool to interact with Google Calendar.
> Requests Google API authorization upon first launch.
> More information: <https://github.com/insanum/gcalcli>.

#### List your events for all your calendars over the next 7 days:
```shell
gcalcli agenda
```
#### Show events starting from or between specific dates (also takes relative dates e.g. "tomorrow"):
```shell
gcalcli agenda {{mm/dd}} [{{mm/dd}}]
```
#### List events from a specific calendar:
```shell
gcalcli --calendar {{calendar_name}} agenda
```
#### Display an ASCII calendar of events by week:
```shell
gcalcli calw
```
#### Display an ASCII calendar of events for a month:
```shell
gcalcli calm
```
#### Quick-add an event to your calendar:
```shell
gcalcli --calendar {{calendar_name}} quick "{{mm/dd}} {{HH:MM}} {{event_name}}"
```
#### Add an event to calendar. Triggers interactive prompt:
```shell
gcalcli --calendar "{{calendar_name}}" add
```
{% endraw %}