---
layout: default
title: "yes"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="yes">
  <a href="/en/common/yes.html">yes</a> <a href="#yes"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Output something repeatedly.
> This command is commonly used to answer yes to every prompt by install commands (such as apt-get).
> More information: <https://www.gnu.org/software/coreutils/yes>.

#### Repeatedly output "message":
```shell
yes {{message}}
```
#### Repeatedly output "y":
```shell
yes
```
#### Accept everything prompted by the `apt-get` command:
```shell
yes | sudo apt-get install {{program}}
```
{% endraw %}