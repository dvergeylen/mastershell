---
layout: default
title: "scrapy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="scrapy">
  <a href="/en/common/scrapy.html">scrapy</a> <a href="#scrapy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Web-crawling framework.
> More information: <https://scrapy.org>.

#### Create a project:
```shell
scrapy startproject {{project_name}}
```
#### Create a spider (in project directory):
```shell
scrapy genspider {{spider_name}} {{website_domain}}
```
#### Edit spider (in project directory):
```shell
scrapy edit {{spider_name}}
```
#### Run spider (in project directory):
```shell
scrapy crawl {{spider_name}}
```
#### Fetch a webpage as scrapy sees it and print source in stdout:
```shell
scrapy fetch {{url}}
```
#### Open a webpage in the default browser as scrapy sees it (disable JavaScript for extra fidelity):
```shell
scrapy view {{url}}
```
#### Open scrapy shell for URL, which allows interaction with the page source in python shell (or ipython if available):
```shell
scrapy shell {{url}}
```
{% endraw %}