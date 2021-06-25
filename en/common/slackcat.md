---
layout: default
title: "slackcat"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="slackcat">
  <a href="/en/common/slackcat.html">slackcat</a> <a href="#slackcat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility for passing files and command output to Slack.
> More information: <https://github.com/bcicen/slackcat>.

#### Post a file to Slack:
```shell
slackcat --channel {{channel_name}} {{path/to/file}}
```
#### Post a file to Slack with a custom filename:
```shell
slackcat --channel {{channel_name}} --filename={{filename}} {{path/to/file}}
```
#### Pipe command output to Slack as a text snippet:
```shell
{{command}} | slackcat --channel {{channel_name}} --filename={{snippet_name}}
```
#### Stream command output to Slack continuously:
```shell
{{command}} | slackcat --channel {{channel_name}} --stream
```
{% endraw %}