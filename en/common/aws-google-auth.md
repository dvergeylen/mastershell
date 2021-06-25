---
layout: default
title: "aws-google-auth"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aws-google-auth">
  <a href="/en/common/aws-google-auth.html">aws-google-auth</a> <a href="#aws-google-auth"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line tool to acquire AWS temporary (STS) credentials using Google Apps as a federated (Single Sign-On) provider.
> More information: <https://github.com/cevoaustralia/aws-google-auth>.

#### Log in with Google SSO using the IDP and SP identifiers and set the credentials duration to one hour:
```shell
aws-google-auth -u {{example@example.com}} -I {{$GOOGLE_IDP_ID}} -S {{$GOOGLE_SP_ID}} -d {{3600}}
```
#### Log in [a]sking which role to use (in case of several available SAML roles):
```shell
aws-google-auth -u {{example@example.com}} -I {{$GOOGLE_IDP_ID}} -S {{$GOOGLE_SP_ID}} -d {{3600}} -a
```
#### Resolve aliases for AWS accounts:
```shell
aws-google-auth -u {{example@example.com}} -I {{$GOOGLE_IDP_ID}} -S {{$GOOGLE_SP_ID}} -d {{3600}} -a --resolve-aliases
```
#### Show help information:
```shell
aws-google-auth -h
```
{% endraw %}