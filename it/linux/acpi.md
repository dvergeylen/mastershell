---
layout: default
title: "acpi"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="acpi">
  <a href="/it/linux/acpi.html">acpi</a> <a href="#acpi"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mostra lo stato e le informazioni termiche della batteria.
> Maggiori informazioni: <https://sourceforge.net/projects/acpiclient/files/acpiclient/>.

#### Mostra le informazioni sulla batteria:
```shell
acpi
```
#### Mostra le informazioni termiche:
```shell
acpi -t
```
#### Mostra le informazioni sul dispositivo di raffreddamento:
```shell
acpi -c
```
#### Mostra le informazioni termiche in gradi Fahrenheit:
```shell
acpi -tf
```
#### Mostra tutte le informazioni:
```shell
acpi -V
```
#### Estrae le informazioni da `/proc` invece che da `/sys`:
```shell
acpi -p
```
{% endraw %}