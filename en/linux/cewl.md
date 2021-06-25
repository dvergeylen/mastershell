---
layout: default
title: "cewl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="cewl">
  <a href="/en/linux/cewl.html">cewl</a> <a href="#cewl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> URL spidering tool for making a cracking wordlist from web content.
> More information: <https://digi.ninja/projects/cewl.php>.

#### Create a wordlist file from the given URL up to 2 links depth:
```shell
cewl --depth {{2}} --write {{path/to/wordlist.txt}} {{url}}
```
#### Output an alphanumeric wordlist from the given URL with words of minimum 5 characters:
```shell
cewl --with-numbers --min_word_length {{5}} {{url}}
```
#### Output a wordlist from the given URL in debug mode including email addresses:
```shell
cewl --debug --email {{url}}
```
#### Output a wordlist from the given URL using HTTP Basic or Digest authentication:
```shell
cewl --auth_type {{basic|digest}} --auth_user {{username}} --auth_pass {{password}} {{url}}
```
#### Output a wordlist from the given URL through a proxy:
```shell
cewl --proxy_host {{host}} --proxy_port {{port}} {{url}}
```
{% endraw %}