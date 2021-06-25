---
layout: default
title: "dirsearch"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="dirsearch">
  <a href="/en/common/dirsearch.html">dirsearch</a> <a href="#dirsearch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Web path scanner.
> More information: <https://github.com/maurosoria/dirsearch>.

#### Scan a web server for common paths with common extensions:
```shell
dirsearch --url {{url}} --extensions-list
```
#### Scan a list of web servers for common paths with the `.php` extension:
```shell
dirsearch --url-list {{path/to/url-list.txt}} --extensions {{php}}
```
#### Scan a web server for user-defined paths with common extensions:
```shell
dirsearch --url {{url}} --extensions-list --wordlist {{path/to/url-paths.txt}}
```
#### Scan a web server using a cookie:
```shell
dirsearch --url {{url}} --extensions {{php}} --cookie {{cookie}}
```
#### Scan a web server using the `HEAD` HTTP method:
```shell
dirsearch --url {{url}} --extensions {{php}} --http-method {{HEAD}}
```
#### Scan a web server, saving the results to a `.json` file:
```shell
dirsearch --url {{url}} --extensions {{php}} --json-report {{path/to/report.json}}
```
{% endraw %}