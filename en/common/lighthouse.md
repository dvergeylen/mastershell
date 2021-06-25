---
layout: default
title: "lighthouse"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="lighthouse">
  <a href="/en/common/lighthouse.html">lighthouse</a> <a href="#lighthouse"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Analyzes web applications and web pages, collecting modern performance metrics and insights on developer best practices.
> More information: <https://github.com/GoogleChrome/lighthouse>.

#### Generate an HTML report for a specific website and save it to a file in the current directory:
```shell
lighthouse {{https://example.com}}
```
#### Generate a JSON report and print it:
```shell
lighthouse --output {{json}} {{https://example.com}}
```
#### Generate a JSON report and save it to a specific file:
```shell
lighthouse --output {{json}} --output-path {{path/to/file.json}} {{https://example.com}}
```
#### Generate a report using the browser in headless mode without logging to stdout:
```shell
lighthouse --quiet --chrome-flags="{{--headless}}" {{https://example.com}}
```
#### Generate a report, using the HTTP header key/value pairs in the specified JSON file for all requests:
```shell
lighthouse --extra-headers={{path/to/file.json}} {{https://example.com}}
```
#### Generate a report for specific categories only:
```shell
lighthouse --only-categories={{performance,accessibility,best-practices,seo,pwa}} {{https://example.com}}
```
#### Generate a report with device emulation and all throttling disabled:
```shell
lighthouse --screenEmulation.disabled --throttling-method={{provided}} --no-emulatedUserAgent {{https://example.com}}
```
#### Display help:
```shell
lighthouse --help
```
{% endraw %}