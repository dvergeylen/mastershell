---
layout: default
title: "zipalign"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="zipalign">
  <a href="/en/common/zipalign.html">zipalign</a> <a href="#zipalign"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zip archive alignment tool.
> Part of the Android SDK build tools.
> More information: <https://developer.android.com/studio/command-line/zipalign>.

#### Align the data of a ZIP file on 4-byte boundaries:
```shell
zipalign {{4}} {{path/to/input.zip}} {{path/to/output.zip}}
```
#### Check that a ZIP file is correctly aligned on 4-byte boundaries and display the results in a verbose manner:
```shell
zipalign -v -c {{4}} {{path/to/input.zip}}
```
{% endraw %}