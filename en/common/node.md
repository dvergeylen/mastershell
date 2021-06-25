---
layout: default
title: "node"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="node">
  <a href="/en/common/node.html">node</a> <a href="#node"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Server-side JavaScript platform (Node.js).
> More information: <https://nodejs.org>.

#### Run a JavaScript file:
```shell
node {{path/to/file}}
```
#### Start a REPL (interactive shell):
```shell
node
```
#### Evaluate JavaScript code by passing it as an argument:
```shell
node -e "{{code}}"
```
#### Evaluate and print result, useful to see node's dependencies versions:
```shell
node -p "{{process.versions}}"
```
#### Activate inspector, pausing execution until a debugger is connected once source code is fully parsed:
```shell
node --no-lazy --inspect-brk {{path/to/file}}
```
{% endraw %}