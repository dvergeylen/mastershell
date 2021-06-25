---
layout: default
title: "amass db"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="amass-db">
  <a href="/en/common/amass-db.html">amass db</a> <a href="#amass-db"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interact with an Amass database.
> More information: <https://github.com/OWASP/Amass/blob/master/doc/user_guide.md#the-db-subcommand>.

#### List all performed enumerations in the database:
```shell
amass db -dir {{path/to/database_directory}} -list
```
#### Show results for a specified enumeration index and domain name:
```shell
amass db -dir {{path/to/database_directory}} -d {{domain_name}} -enum {{index_from_list}} -show
```
#### List all found subdomains of a domain within an enumeration:
```shell
amass db -dir {{path/to/database_directory}} -d {{domain_name}} -enum {{index_from_list}} -names
```
#### Show a summary of the found subdomains within an enumeration:
```shell
amass db -dir {{path/to/database_directory}} -d {{domain_name}} -enum {{index_from_list}} -summary
```
{% endraw %}