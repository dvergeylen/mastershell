---
layout: default
title: "phpcs"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="phpcs">
  <a href="/en/common/phpcs.html">phpcs</a> <a href="#phpcs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tokenize PHP, JavaScript and CSS files to detect violations of a defined set of coding standards.
> More information: <https://github.com/squizlabs/PHP_CodeSniffer>.

#### Sniff the specified directory for issues (defaults to the PEAR standard):
```shell
phpcs {{path/to/directory}}
```
#### Display a list of installed coding standards:
```shell
phpcs -i
```
#### Specify a coding standard to validate against:
```shell
phpcs {{path/to/directory}} --standard {{standard}}
```
#### Specify comma-separated file extensions to include when sniffing:
```shell
phpcs {{path/to/directory}} --extensions {{file_extension(s)}}
```
#### Specify the format of the output report (e.g. `full`, `xml`, `json`, `summary`):
```shell
phpcs {{path/to/directory}} --report {{format}}
```
#### Set config variables to be used during the process:
```shell
phpcs {{path/to/directory}} --config-set {{key}} {{value}}
```
#### A comma-separated list of files to load before processing:
```shell
phpcs {{path/to/directory}} --bootstrap {{file(s)}}
```
#### Don't recurse into subdirectories:
```shell
phpcs {{path/to/directory}} -l
```
{% endraw %}