---
layout: default
title: "croc"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="croc">
  <a href="/en/common/croc.html">croc</a> <a href="#croc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Send and receive files easily and securely over any network.
> More information: <https://github.com/schollz/croc>.

#### Send a file or directory:
```shell
croc send {{path/to/file_or_directory}}
```
#### Send a file or directory with a specific passphrase:
```shell
croc send --code {{passphrase}} {{path/to/file_or_directory}}
```
#### Receive a file or directory on receiving machine:
```shell
croc {{passphrase}}
```
#### Send and connect over a custom relay:
```shell
croc --relay {{ip_to_relay}} send {{path/to/file_or_directory}}
```
#### Receive and connect over a custom relay:
```shell
croc --relay {{ip_to_relay}} {{passphrase}}
```
#### Host a croc relay on the default ports:
```shell
croc relay
```
#### Display parameters and options for a croc command:
```shell
croc {{send|relay}} --help
```
{% endraw %}