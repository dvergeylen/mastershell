---
layout: default
title: "csvsql"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="csvsql">
  <a href="/de/common/csvsql.html">csvsql</a> <a href="#csvsql"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generiere SQL-Anweisungen für eine CSV-Datei oder führe diese Anweisungen direkt in einer Datenbank aus.
> Teil von csvkit.
> Weitere Informationen: <https://csvkit.readthedocs.io/en/latest/scripts/csvsql.html>.

#### Generiere eine `CREATE TABLE`-SQL-Anweisung für eine CSV-Datei:
```shell
csvsql {{pfad/zu/datei.csv}}
```
#### Importiere eine CSV-Datei in eine SQL-Datenbank:
```shell
csvsql --insert --db "{{mysql://benutzer:passwort@host/datenbank}}" {{pfad/zu/datei.csv}}
```
#### Führe eine SQL-Abfrage auf einer CSV-Datei aus:
```shell
csvsql --query "{{select * from 'datei'}}" {{datei.csv}}
```
{% endraw %}