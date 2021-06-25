---
layout: default
title: "firefox"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="firefox">
  <a href="/en/common/firefox.html">firefox</a> <a href="#firefox"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A free and open source web browser.
> More information: <https://developer.mozilla.org/en-US/docs/Mozilla/Command_Line_Options>.

#### Launch Firefox and open a web page:
```shell
firefox {{https://www.duckduckgo.com}}
```
#### Open a new window:
```shell
firefox --new-window {{https://www.duckduckgo.com}}
```
#### Open a private (incognito) window:
```shell
firefox --private-window
```
#### Search for "wikipedia" using the default search engine:
```shell
firefox --search "{{wikipedia}}"
```
#### Launch Firefox in safe mode, with all extensions disabled:
```shell
firefox --safe-mode
```
#### Take a screenshot of a web page in headless mode:
```shell
firefox --headless --screenshot {{path/to/output_file.png}} {{https://example.com/}}
```
#### Use a specific profile to allow multiple separate instances of Firefox to run at once:
```shell
firefox --profile {{path/to/directory}} {{https://example.com/}}
```
#### Set Firefox as the default browser:
```shell
firefox --setDefaultBrowser
```
{% endraw %}