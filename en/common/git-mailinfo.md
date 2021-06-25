---
layout: default
title: "git mailinfo"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-mailinfo">
  <a href="/en/common/git-mailinfo.html">git mailinfo</a> <a href="#git-mailinfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Extract patch and authorship information from a single email message.
> More information: <https://git-scm.com/docs/git-mailinfo>.

#### Extract the patch and author data from an email message:
```shell
git mailinfo {{message|patch}}
```
#### Extract but remove leading and trailing whitespace:
```shell
git mailinfo -k {{message|patch}}
```
#### Remove everything from the body before a scissors line (e.g. "-->* --") and retrieve the message or patch:
```shell
git mailinfo --scissors {{message|patch}}
```
{% endraw %}