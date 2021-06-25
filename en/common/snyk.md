---
layout: default
title: "snyk"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="snyk">
  <a href="/en/common/snyk.html">snyk</a> <a href="#snyk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Find vulnerabilities in your code and remediate risks.
> More information: <https://snyk.io>.

#### Log in to your Snyk account:
```shell
snyk auth
```
#### Test your code for any known vulnerabilities:
```shell
snyk test
```
#### Test a local Docker image for any known vulnerabilities:
```shell
snyk test --docker {{docker_image}}
```
#### Record the state of dependencies and any vulnerabilities on snyk.io:
```shell
snyk monitor
```
#### Auto patch and ignore vulnerabilities:
```shell
snyk wizard
```
{% endraw %}