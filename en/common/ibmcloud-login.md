---
layout: default
title: "ibmcloud login"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="ibmcloud-login">
  <a href="/en/common/ibmcloud-login.html">ibmcloud login</a> <a href="#ibmcloud-login"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Log in to the IBM Cloud.
> More information: <https://cloud.ibm.com/docs/cli?topic=cli-ibmcloud_cli#ibmcloud_login>.

#### Log in by using an interactive prompt:
```shell
ibmcloud login
```
#### Log in to a specific API endpoint (default is `cloud.ibm.com`):
```shell
ibmcloud login -a {{api_endpoint}}
```
#### Log in by providing username, password and the targeted region as parameters:
```shell
ibmcloud login -u {{username}} -p {{password}} -r {{us-south}}
```
#### Log in with an API key, passing it as an argument:
```shell
ibmcloud login --apikey {{api_key_string}}
```
#### Log in with an API key, passing it as a file:
```shell
ibmcloud login --apikey @{{path/to/api_key_file}}
```
#### Log in with a federated ID (single sign-on):
```shell
ibmcloud login --sso
```
{% endraw %}