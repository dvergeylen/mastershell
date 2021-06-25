---
layout: default
title: "fossa"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="fossa">
  <a href="/en/common/fossa.html">fossa</a> <a href="#fossa"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI for the Fossa service - Generate realtime license audits, vulnerability scans and reports about dependencies licenses.
> More information: <https://github.com/fossas/fossa-cli>.

#### Initialize a `.fossa.yml` configuration file:
```shell
fossa init
```
#### Run a default project build:
```shell
fossa build
```
#### Analyze built dependencies:
```shell
fossa analyze
```
#### Generate reports:
```shell
fossa report
```
#### Test current revision against the FOSSA scan status and exit with errors if issues are found:
```shell
fossa test
```
{% endraw %}