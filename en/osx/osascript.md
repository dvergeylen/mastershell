---
layout: default
title: "osascript"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="osascript">
  <a href="/en/osx/osascript.html">osascript</a> <a href="#osascript"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run AppleScript or JavaScript for Automation (JXA) from the command-line.

#### Run an AppleScript command:
```shell
osascript -e '{{say "Hello world"}}'
```
#### Run multiple AppleScript commands:
```shell
osascript -e '{{say "Hello"}}' -e '{{say "world"}}'
```
#### Run a compiled (`*.scpt`), bundled (`*.scptd`), or plaintext (`*.applescript`) AppleScript file:
```shell
osascript {{path/to/apple.scpt}}
```
#### Get the bundle identifier of an application (useful for `open -b`):
```shell
osascript -e 'id of app "{{Application}}"'
```
#### Run a JavaScript command:
```shell
osascript -l JavaScript -e '{{console.log("Hello world");}}'
```
#### Run a JavaScript file:
```shell
osascript -l JavaScript {{path/to/script.js}}
```
{% endraw %}