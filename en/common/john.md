---
layout: default
title: "john"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="john">
  <a href="/en/common/john.html">john</a> <a href="#john"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Password cracker.
> More information: <https://www.openwall.com/john/>.

#### Crack password hashes:
```shell
john {{path/to/hashes.txt}}
```
#### Show passwords cracked:
```shell
john --show {{path/to/hashes.txt}}
```
#### Display users' cracked passwords by user identifier from multiple files:
```shell
john --show --users={{user_ids}} {{path/to/hashes*}} {{path/to/other/hashes*}}
```
#### Crack password hashes, using a custom wordlist:
```shell
john --wordlist={{path/to/wordlist.txt}} {{path/to/hashes.txt}}
```
#### List available hash formats:
```shell
john --list=formats
```
#### Crack password hashes, using a specific hash format:
```shell
john --format={{md5crypt}} {{path/to/hashes.txt}}
```
#### Crack password hashes, enabling word mangling rules:
```shell
john --rules {{path/to/hashes.txt}}
```
#### Restore an interrupted cracking session from a state file, e.g. `mycrack.rec`:
```shell
john --restore={{path/to/mycrack.rec}}
```
{% endraw %}