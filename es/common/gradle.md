---
layout: default
title: "gradle"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="gradle">
  <a href="/es/common/gradle.html">gradle</a> <a href="#gradle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gradle es un sistema de código abierto para automatizar la compilación de proyectos.
> Más información: <https://gradle.org>.

#### Compila un proyecto:
```shell
gradle build
```
#### Excluye la tarea *test*:
```shell
gradle build -x {{test}}
```
#### Ejecuta en modo offline para prevenir que gradle acceda a la red durante una compilación:
```shell
gradle build --offline
```
#### Limpia el directorio de compilación:
```shell
gradle clean
```
#### Compila y genera un paquete:
```shell
gradle assembleRelease
```
{% endraw %}