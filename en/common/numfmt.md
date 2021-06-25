---
layout: default
title: "numfmt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="numfmt">
  <a href="/en/common/numfmt.html">numfmt</a> <a href="#numfmt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Convert numbers to and from human-readable strings.
> More information: <https://www.gnu.org/software/coreutils/numfmt>.

#### Convert 1.5K (SI Units) to 1500:
```shell
numfmt --from={{si}} {{1.5K}}
```
#### Convert 5th field (1-indexed) to IEC Units without converting header:
```shell
ls -l | numfmt --header={{1}} --field={{5}} --to={{iec}}
```
#### Convert to IEC units, pad with 5 characters, left aligned:
```shell
du -s * | numfmt --to={{iec}} --format="{{%-5f}}"
```
{% endraw %}