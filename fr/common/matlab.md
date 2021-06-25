---
layout: default
title: "matlab"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="matlab">
  <a href="/fr/common/matlab.html">matlab</a> <a href="#matlab"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Environnement de calcul numérique créé par MathWorks.
> Plus d'informations : <https://fr.mathworks.com/help/matlab/>.

#### Lance MATLAB sans afficher l'écran de démarrage :
```shell
matlab -nosplash
```
#### Exécute une instruction MATLAB :
```shell
matlab -r "{{instruction_matlab}}"
```
#### Exécute un script MATLAB :
```shell
matlab -r "run({{chemin/vers/script.m}})"
```
{% endraw %}