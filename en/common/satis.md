---
layout: default
title: "satis"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="satis">
  <a href="/en/common/satis.html">satis</a> <a href="#satis"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The command-line utility for the Satis static Composer repository.
> More information: <https://github.com/composer/satis>.

#### Initialise a Satis configuration:
```shell
satis init {{satis.json}}
```
#### Add a VCS repository to the Satis configuration:
```shell
satis add {{repository_url}}
```
#### Build the static output from the configuration:
```shell
satis build {{satis.json}} {{path/to/output_directory}}
```
#### Build the static output by updating only the specified repository:
```shell
satis build --repository-url {{repository_url}} {{satis.json}} {{path/to/output_directory}}
```
#### Remove useless archive files:
```shell
satis purge {{satis.json}} {{path/to/output_directory}}
```
{% endraw %}