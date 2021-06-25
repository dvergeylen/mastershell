---
layout: default
title: "aws-google-auth"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aws-google-auth">
  <a href="/de/common/aws-google-auth.html">aws-google-auth</a> <a href="#aws-google-auth"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI, um temporäre AWS credentials (STS) über Google Apps als Single Sign-On Dienstleister zu erhalten.
> Weitere Informationen: <https://github.com/cevoaustralia/aws-google-auth>.

#### Einloggen mit Google SSO über IDP- und SP-Kennung für die Dauer einer Stunde:
```shell
aws-google-auth -u {{beispiel@beispiel.com}} -I {{$GOOGLE_IDP_ID}} -S {{$GOOGLE_SP_ID}} -d {{3600}}
```
#### Einloggen mit der Option eine Rolle auszuwählen (im Falle mehrerer verfügbarer SAML Rollen):
```shell
aws-google-auth -u {{beispiel@beispiel.com}} -I {{$GOOGLE_IDP_ID}} -S {{$GOOGLE_SP_ID}} -d {{3600}} -a
```
#### Löse Aliasse von AWS Accounts auf:
```shell
aws-google-auth -u {{beispiel@beispiel.com}} -I {{$GOOGLE_IDP_ID}} -S {{$GOOGLE_SP_ID}} -d {{3600}} -a --resolve-aliases
```
#### Zeige Hilfs-Informationen:
```shell
aws-google-auth -h
```
{% endraw %}