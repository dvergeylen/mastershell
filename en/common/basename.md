---
layout: default
title: "basename"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="basename">
  <a href="/en/common/basename.html">basename</a> <a href="#basename"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remove leading directory portions from a path.
> More information: <https://www.gnu.org/software/coreutils/basename>.

#### Show only the file name from a path:
```shell
basename {{path/to/file}}
```
#### Show only the rightmost directory name from a path:
```shell
basename {{path/to/directory/}}
```
#### Show only the file name from a path, with a suffix removed:
```shell
basename {{path/to/file}} {{suffix}}
```
{% endraw %}