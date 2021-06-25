---
layout: default
title: "theHarvester"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="theharvester">
  <a href="/en/common/theharvester.html">theHarvester</a> <a href="#theharvester"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool designed to be used in the early stages of a penetration test.
> More information: <https://github.com/laramies/theHarvester>.

#### Gather information on a domain using Google:
```shell
theHarvester --domain {{domain_name}} --source google
```
#### Gather information on a domain using multiple sources:
```shell
theHarvester --domain {{domain_name}} --source {{google,bing,crtsh}}
```
#### Change the limit of results to work with:
```shell
theHarvester --domain {{domain_name}} --source {{google}} --limit {{200}}
```
#### Save the output to two files in xml and html format:
```shell
theHarvester --domain {{domain_name}} --source {{google}} --file {{output_file_name}}
```
#### Output all available options:
```shell
theHarvester --help
```
{% endraw %}