---
layout: default
title: "abduco"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="abduco">
  <a href="/en/common/abduco.html">abduco</a> <a href="#abduco"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Terminal session manager.
> More information: <http://www.brain-dump.org/projects/abduco/>.

#### List sessions:
```shell
abduco
```
#### Attach to a session, creating it if it doesn't exist:
```shell
abduco -A {{name}} {{bash}}
```
#### Attach to a session with `dvtm`, creating it if it doesn't exist:
```shell
abduco -A {{name}}
```
#### Detach from a session:
```shell
Ctrl + \
```
#### Attach to a session in read-only mode:
```shell
abduco -Ar {{name}}
```
{% endraw %}