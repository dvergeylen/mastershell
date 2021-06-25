---
layout: default
title: "sonar-scanner"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sonar-scanner">
  <a href="/en/common/sonar-scanner.html">sonar-scanner</a> <a href="#sonar-scanner"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> SonarScanner is a generic scanner for SonarQube projects that do not use build tools such as Maven, Gradle, or Ant.
> More information: <https://docs.sonarqube.org/latest/analysis/scan/sonarscanner/>.

#### Scan a project with configuration file in your project's root directory named `sonar-project.properties`:
```shell
sonar-scanner
```
#### Scan a project using configuration file other than `sonar-project.properties`:
```shell
sonar-scanner -D{{project.settings=myproject.properties}}
```
#### Print help information:
```shell
sonar-scanner -h
```
#### Print debugging information:
```shell
sonar-scanner -X
```
{% endraw %}