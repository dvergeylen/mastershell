---
layout: default
title: "aws-vault"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aws-vault">
  <a href="/en/common/aws-vault.html">aws-vault</a> <a href="#aws-vault"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A vault for securely storing and accessing AWS credentials in development environments.
> More information: <https://github.com/99designs/aws-vault>.

#### Add credentials to the secure keystore:
```shell
aws-vault add {{profile}}
```
#### Execute a command with AWS credentials in the environment:
```shell
aws-vault exec {{profile}} -- {{aws s3 ls}}
```
#### Open a browser window and login to the AWS Console:
```shell
aws-vault login {{profile}}
```
#### List profiles, along with their credentials and sessions:
```shell
aws-vault list
```
#### Rotate AWS credentials:
```shell
aws-vault rotate {{profile}}
```
#### Remove credentials from the secure keystore:
```shell
aws-vault remove {{profile}}
```
{% endraw %}