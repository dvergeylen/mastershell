---
layout: default
title: "nms"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="nms">
  <a href="/en/common/nms.html">nms</a> <a href="#nms"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line tool that recreates the famous data decryption effect seen in the 1992 movie Sneakers from stdin.
> More information: <https://github.com/bartobri/no-more-secrets>.

#### Decrypt text after a keystroke:
```shell
echo "{{Hello, World!}}" | nms
```
#### Decrypt output immediately, without waiting for a keystroke:
```shell
{{ls -la}} | nms -a
```
#### Decrypt the content of a file, with a custom output color:
```shell
cat {{path/to/file}} | nms -a -f {{blue|white|yellow|black|magenta|green|red}}
```
#### Clear the screen before decrypting:
```shell
{{command}} | nms -a -c
```
{% endraw %}