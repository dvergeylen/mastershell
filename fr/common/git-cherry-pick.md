---
layout: default
title: "git cherry-pick"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-cherry-pick">
  <a href="/fr/common/git-cherry-pick.html">git cherry-pick</a> <a href="#git-cherry-pick"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Appliquer les modifications introduites par les commits existants à la branche actuelle.
> Pour appliquer les changements a une autre branche, utiliser d'abord `git checkout` pour basculer sur la branche désirée.
> Plus d'informations : <https://git-scm.com/docs/git-cherry-pick>.

#### Applique un commit à la branche courante :
```shell
git cherry-pick {{commit}}
```
#### Appliquer une plage de commits à la branche courante (voir aussi `git rebase --onto`) :
```shell
git cherry-pick {{start_commit}}~..{{end_commit}}
```
#### Appliquer plusieurs commits non séquentiels à la branche courante :
```shell
git cherry-pick {{commit_1}} {{commit_2}}
```
#### Appliquer les changements d'un commit à la branche courante sans créer de commit :
```shell
git cherry-pick -n {{commit}}
```
{% endraw %}