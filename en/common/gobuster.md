---
layout: default
title: "gobuster"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gobuster">
  <a href="/en/common/gobuster.html">gobuster</a> <a href="#gobuster"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Brute-forces hidden paths on web servers and more.
> More information: <https://github.com/OJ/gobuster>.

#### Discover directories and files that match in the wordlist:
```shell
gobuster dir --url {{https://example.com/}} --wordlist {{path/to/file}}
```
#### Discover subdomains:
```shell
gobuster dns --domain {{example.com}} --wordlist {{path/to/file}}
```
#### Discover Amazon S3 buckets:
```shell
gobuster s3 --wordlist {{path/to/file}}
```
#### Discover other virtual hosts on the server:
```shell
gobuster vhost --url {{https://example.com/}} --wordlist {{path/to/file}}
```
#### Fuzz the value of a parameter:
```shell
gobuster fuzz --url {{https://example.com/?parameter=FUZZ}} --wordlist {{path/to/file}}
```
#### Fuzz the name of a parameter:
```shell
gobuster fuzz --url {{https://example.com/?FUZZ=value}} --wordlist {{path/to/file}}
```
{% endraw %}