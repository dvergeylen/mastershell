---
layout: default
title: "ansible-playbook"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ansible-playbook">
  <a href="/it/common/ansible-playbook.html">ansible-playbook</a> <a href="#ansible-playbook"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Esegui task definiti nel playbook di un computer remoto via SSH.
> Maggiori informazioni: <https://docs.ansible.com/ansible/latest/cli/ansible-playbook.html>.

#### Esegui tasks nel playbook:
```shell
ansible-playbook {{playbook}}
```
#### Esegui task nel playbook con un inventory personalizzato:
```shell
ansible-playbook {{playbook}} -i {{inventory}}
```
#### Esegui task nel playvook con variabili aggiuntive definite da linea di comando:
```shell
ansible-playbook {{playbook}} -e "{{variabile1}}={{valore1}} {{variabile2}}={{valore2}} ..."
```
#### Esegui task nel playbook con variabili aggiuntive definite in un file JSON:
```shell
ansible-playbook {{playbook}} -e "@{{variabili.json}}"
```
{% endraw %}