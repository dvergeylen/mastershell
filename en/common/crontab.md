---
layout: default
title: "crontab"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="crontab">
  <a href="/en/common/crontab.html">crontab</a> <a href="#crontab"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Schedule cron jobs to run on a time interval for the current user.
> Job definition format: "(min) (hour) (day_of_month) (month) (day_of_week) command_to_execute".
> More information: <https://manned.org/crontab>.

#### Edit the crontab file for the current user:
```shell
crontab -e
```
#### Edit the crontab file for a specific user:
```shell
sudo crontab -e -u {{user}}
```
#### Replace the current crontab with the contents of the given file:
```shell
crontab {{path/to/file}}
```
#### View a list of existing cron jobs for current user:
```shell
crontab -l
```
#### Remove all cron jobs for the current user:
```shell
crontab -r
```
#### Sample job which runs at 10:00 every day (* means any value):
```shell
0 10 * * * {{command_to_execute}}
```
#### Sample job which runs every minute on the 3rd of April:
```shell
* * 3 Apr * {{command_to_execute}}
```
#### Sample job which runs a certain script at 02:30 every Friday:
```shell
30 2 * * Fri {{/absolute/path/to/script.sh}}
```
{% endraw %}