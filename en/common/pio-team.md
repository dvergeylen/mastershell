---
layout: default
title: "pio team"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="pio-team">
  <a href="/en/common/pio-team.html">pio team</a> <a href="#pio-team"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage PlatformIO teams.
> More information: <https://docs.platformio.org/en/latest/core/userguide/team/>.

#### Create a new team with the specified description:
```shell
pio team create --description {{description}} {{organization_name}}:{{team_name}}
```
#### Delete a team:
```shell
pio team destroy {{organization_name}}:{{team_name}}
```
#### Add a new user to a team:
```shell
pio team add {{organization_name}}:{{team_name}} {{username}}
```
#### Remove a user from a team:
```shell
pio team remove {{organization_name}}:{{team_name}} {{username}}
```
#### List all teams that the user is part of and their members:
```shell
pio team list
```
#### List all teams in an organization:
```shell
pio team list {{organization_name}}
```
#### Rename a team:
```shell
pio team update --name {{new_team_name}} {{organization_name}}:{{team_name}}
```
#### Change the description of a team:
```shell
pio team update --description {{new_description}} {{organization_name}}:{{team_name}}
```
{% endraw %}