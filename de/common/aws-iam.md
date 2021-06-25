---
layout: default
title: "aws iam"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aws-iam">
  <a href="/de/common/aws-iam.html">aws iam</a> <a href="#aws-iam"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI für AWS IAM.
> Weitere Informationen: <https://awscli.amazonaws.com/v2/documentation/api/latest/reference/iam/index.html>.

#### Zeige die AWS IAM Hilfeseite (beinhaltet auch Hinweise für alle Unterbefehle):
```shell
aws iam help
```
#### Liste aller Benutzer auf:
```shell
aws iam list-users
```
#### Liste aller Richtlinien auf:
```shell
aws iam list-policies
```
#### Liste aller Gruppen auf:
```shell
aws iam list-groups
```
#### Liste aller Benutzer zu einer Gruppe auf:
```shell
aws iam get-group --group-name {{gruppe}}
```
#### Liste einer IAM Richtlinie detailliert auf:
```shell
aws iam get-policy --policy-arn arn:aws:iam::aws:policy/{{richtlinie}}
```
#### Liste alle Zugriffsschlüssel auf:
```shell
aws iam list-access-keys
```
#### Liste alle Zugriffsschlüssel für einen Benutzer auf:
```shell
aws iam list-access-keys --user-name {{benutzername}}
```
{% endraw %}