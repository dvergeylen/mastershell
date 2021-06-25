---
layout: default
title: "gimp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gimp">
  <a href="/en/common/gimp.html">gimp</a> <a href="#gimp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> GNU image manipulation program.
> More information: <https://docs.gimp.org/en/gimp-fire-up.html#gimp-concepts-running-command-line>.

#### Launch GIMP:
```shell
gimp
```
#### Launch GIMP without showing the splash screen:
```shell
gimp --no-splash
```
#### Start a new GIMP instance, even if there is already a running one:
```shell
gimp --new-instance
```
#### Open the given file as a new image:
```shell
gimp --as-new {{path/to/image}}
```
#### Print errors and warnings to the console instead of showing them in a dialog box:
```shell
gimp --console-messages
```
#### Enable debugging signal handlers:
```shell
gimp --debug-handlers
```
{% endraw %}