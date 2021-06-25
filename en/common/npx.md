---
layout: default
title: "npx"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="npx">
  <a href="/en/common/npx.html">npx</a> <a href="#npx"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Execute binaries from `npm` packages.
> More information: <https://www.npmjs.com/package/npx>.

#### Execute the binary from a given npm module:
```shell
npx {{module_name}}
```
#### In case a package has multiple binaries, specify the package name along with the binary:
```shell
npx -p {{package_name}} {{module_name}}
```
#### View help contents:
```shell
npx --help
```
{% endraw %}