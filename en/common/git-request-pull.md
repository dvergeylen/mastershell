---
layout: default
title: "git request-pull"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-request-pull">
  <a href="/en/common/git-request-pull.html">git request-pull</a> <a href="#git-request-pull"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate a request asking the upstream project to pull changes into its tree.
> More information: <https://git-scm.com/docs/git-request-pull>.

#### Produce a request summarizing the changes between the v1.1 release and a specified branch:
```shell
git request-pull {{v1.1}} {{https://example.com/project}} {{branch_name}}
```
#### Produce a request summarizing the changes between the v0.1 release on the `foo` branch and the local `bar` branch:
```shell
git request-pull {{v0.1}} {{https://example.com/project}} {{foo:bar}}
```
{% endraw %}