---
layout: default
title: "rpmbuild"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rpmbuild">
  <a href="/en/linux/rpmbuild.html">rpmbuild</a> <a href="#rpmbuild"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> RPM Package Build tool.
> More information: <https://docs.fedoraproject.org/en-US/quick-docs/creating-rpm-packages/>.

#### Build binary and source packages:
```shell
rpmbuild -ba {{path/to/spec_file}}
```
#### Build a binary package without source package:
```shell
rpmbuild -bb {{path/to/spec_file}}
```
#### Specify additional variables when building a package:
```shell
rpmbuild -bb {{path/to/spec_file}} --define "{{variable1}} {{value1}}" --define "{{variable2}} {{value2}}"
```
{% endraw %}