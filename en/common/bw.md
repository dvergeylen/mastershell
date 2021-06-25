---
layout: default
title: "bw"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bw">
  <a href="/en/common/bw.html">bw</a> <a href="#bw"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A CLI to access and manage a Bitwarden vault.
> More information: <https://help.bitwarden.com/article/cli/>.

#### Log in to a Bitwarden user account:
```shell
bw login
```
#### Log out of a Bitwarden user account:
```shell
bw logout
```
#### Search and display items from Bitwarden vault:
```shell
bw list items --search {{github}}
```
#### Display a particular item from Bitwarden vault:
```shell
bw get item {{github}}
```
#### Create a folder in Bitwarden vault:
```shell
{{echo -n '{"name":"My Folder1"}' | base64}} | bw create folder
```
{% endraw %}