---
layout: default
title: "transcrypt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="transcrypt">
  <a href="/en/common/transcrypt.html">transcrypt</a> <a href="#transcrypt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Transparently encrypt files within a Git repository.
> More information: <https://github.com/elasticdog/transcrypt>.

#### Initialize an unconfigured repository:
```shell
transcrypt
```
#### List the currently encrypted files:
```shell
git ls-crypt
```
#### Display the credentials of a configured repository:
```shell
transcrypt --display
```
#### Initialize and decrypt a fresh clone of a configured repository:
```shell
transcrypt --cipher={{cipher}}
```
#### Rekey to change the encryption cipher or password:
```shell
transcrypt --rekey
```
{% endraw %}