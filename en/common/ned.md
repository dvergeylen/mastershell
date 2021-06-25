---
layout: default
title: "ned"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ned">
  <a href="/en/common/ned.html">ned</a> <a href="#ned"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Is like `grep` but with powerful replace capabilities.
> Unlike `sed`, as it isn't restricted to line oriented editing.
> More information: <https://github.com/nevdelap/ned>.

#### Recursively search starting in the current directory, ignoring case:
```shell
ned --ignore-case --recursive '{{^[dl]og}}' {{.}}
```
#### Search always showing colored output:
```shell
ned --colors '{{^[dl]og}}' {{.}}
```
#### Search never showing colored output:
```shell
ned --colors=never '{{^[dl]og}}' {{.}}
```
#### Search ignoring certain files:
```shell
ned --recursive --exclude '{{*.htm}}' '{{^[dl]og}}' {{.}}
```
#### Simple replace:
```shell
ned '{{dog}}' --replace '{{cat}}' {{.}}
```
#### Replace using numbered group references:
```shell
ned '{{the ([a-z]+) dog and the ([a-z]+) dog}}' --replace '{{the $2 dog and the $1 dog}}' {{.}}
```
#### Replace changing case:
```shell
ned '{{([a-z]+) dog}}' --case-replacements --replace '{{\U$1\E! dog}}' --stdout {{.}}
```
#### Preview results of a find and replace without updating the target files:
```shell
ned '{{^[sb]ad}}' --replace '{{happy}}' --stdout {{.}}
```
{% endraw %}