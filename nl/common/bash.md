---
layout: default
title: "bash"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bash">
  <a href="/nl/common/bash.html">bash</a> <a href="#bash"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bourne-Again SHell.
> `sh`-ondersteunende commandoregel-interpreteerder.
> Meer informatie: <https://gnu.org/software/bash>.

#### Start interactieve shell:
```shell
bash
```
#### Voer een commando uit:
```shell
bash -c "{{commando}}"
```
#### Voer commando's van bestand uit:
```shell
bash {{bestand.sh}}
```
#### Voer commando's van bestand uit, en print alle uitgevoerde commando's naar de terminal:
```shell
bash -x {{bestand.sh}}
```
#### Voer commando's van bestand uit, en stop bij de eerste fout:
```shell
bash -e {{bestand.sh}}
```
#### Voer commando's van stdin uit:
```shell
bash -s
```
#### Print de versieinformatie van bash (gebruik `echo $BASH_VERSION` om alleen de versie te krijgen zonder licentie):
```shell
bash --version
```
{% endraw %}