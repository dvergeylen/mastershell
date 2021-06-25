---
layout: default
title: "asciinema"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="asciinema">
  <a href="/en/common/asciinema.html">asciinema</a> <a href="#asciinema"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Record and replay terminal sessions, and optionally share them on asciinema.org.
> More information: <https://asciinema.org/>.

#### Associate the local install of `asciinema` with an asciinema.org account:
```shell
asciinema auth
```
#### Make a new recording (once finished, user will be prompted to upload it or save it locally):
```shell
asciinema rec
```
#### Make a new recording and save it to a local file:
```shell
asciinema rec {{path/to/file}}.cast
```
#### Replay a terminal recording from a local file:
```shell
asciinema play {{path/to/file}}.cast
```
#### Replay a terminal recording hosted on asciinema.org:
```shell
asciinema play https://asciinema.org/a/{{cast_id}}
```
#### Make a new recording, limiting any idle time to at most 2.5 seconds:
```shell
asciinema rec -i {{2.5}}
```
#### Print the full output of a locally saved recording:
```shell
asciinema cat {{path/to/file}}.cast
```
#### Upload a locally saved terminal session to asciinema.org:
```shell
asciinema upload {{path/to/file}}.cast
```
{% endraw %}