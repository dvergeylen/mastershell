---
layout: default
title: "git cherry-pick"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-cherry-pick">
  <a href="/it/common/git-cherry-pick.html">git cherry-pick</a> <a href="#git-cherry-pick"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Applica al ramo corrente le modifiche introdotte da commit esistenti.
> Per applicare le modifiche ad un altro ramo, usa prima `git checkout` per passare al ramo desiderato.
> Maggiori informazioni: <https://git-scm.com/docs/git-cherry-pick>.

#### Applica un commit al ramo corrente:
```shell
git cherry-pick {{commit}}
```
#### Applica una sequenza di commit al ramo corrente (vedi anche `git rebase --onto`):
```shell
git cherry-pick {{commit_iniziale}}~..{{commit_finale}}
```
#### Applica un insieme di commit non sequenziali al ramo corrente:
```shell
git cherry-pick {{commit_1}} {{commit_2}}
```
#### Aggiungi le modifiche introdotte da un commit alla cartella di lavoro, ma senza creare un nuovo commit:
```shell
git cherry-pick -n {{commit}}
```
{% endraw %}