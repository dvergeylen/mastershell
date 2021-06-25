---
layout: default
title: "git update-ref"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="git-update-ref">
  <a href="/it/common/git-update-ref.html">git update-ref</a> <a href="#git-update-ref"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Crea, aggiorna e cancella riferimenti Git.
> Maggiori informazioni: <https://git-scm.com/docs/git-update-ref>.

#### Cancella un riferimento, utile per resettare il primo commit in modo soft:
```shell
git update-ref -d {{HEAD}}
```
#### Aggiorna un riferimento con un messaggio:
```shell
git update-ref -m {{messaggio}} {{HEAD}} {{4e95e05}}
```
{% endraw %}