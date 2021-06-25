---
layout: default
title: "fin"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fin">
  <a href="/en/common/fin.html">fin</a> <a href="#fin"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Docksal command-line utility.
> More information: <https://docs.docksal.io/fin/fin/>.

#### Start the project in the current directory:
```shell
fin project start
```
#### Stop the project in the current directory:
```shell
fin project stop
```
#### Open a shell into a specific container:
```shell
fin bash {{container_name}}
```
#### Display logs of a specific container:
```shell
fin logs {{container_name}}
```
#### Display logs of a specific container and follow the log:
```shell
fin logs -f {{container_name}}
```
{% endraw %}