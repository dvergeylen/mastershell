---
layout: default
title: "google-chrome"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="google-chrome">
  <a href="/en/linux/google-chrome.html">google-chrome</a> <a href="#google-chrome"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The web browser from Google.
> More information: <https://chrome.google.com>.

#### Run with a custom profile directory:
```shell
google-chrome --user-data-dir={{path/to/directory}}
```
#### Run without CORS validation, useful to test an API:
```shell
google-chrome --user-data-dir={{path/to/directory}} --disable-web-security
```
{% endraw %}