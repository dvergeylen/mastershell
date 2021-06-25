---
layout: default
title: "git request-pull"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-request-pull">
  <a href="/fr/common/git-request-pull.html">git request-pull</a> <a href="#git-request-pull"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Générer une requête demandant au projet en amont d'inclure les modifications dans son arborescence.
> Plus d'informations : <https://git-scm.com/docs/git-request-pull>.

#### Produire une requête résumant les changements entre la version v1.1 et le master :
```shell
git request-pull {{v1.1}} {{https://example.com/project}} {{master}}
```
#### Produire une requête résumant les changements entre la version v1.1 sur la branche master et la branche locale foo :
```shell
git request-pull {{v0.1}} {{https://example.com/project}} {{master:foo}}
```
{% endraw %}