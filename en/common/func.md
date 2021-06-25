---
layout: default
title: "func"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="func">
  <a href="/en/common/func.html">func</a> <a href="#func"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Azure Functions Core Tools: Develop and test Azure Functions locally.
> Local functions can connect to live Azure services, and can deploy a function app to an Azure subscription.
> More information: <https://docs.microsoft.com/azure/azure-functions/functions-run-local>.

#### Create a new functions project:
```shell
func init {{project}}
```
#### Create a new function:
```shell
func new
```
#### Run functions locally:
```shell
func start
```
#### Publish your code to a function app in Azure:
```shell
func azure functionapp publish {{function}}
```
#### Download all settings from an existing function app:
```shell
func azure functionapp fetch-app-settings {{function}}
```
#### Get the connection string for a specific storage account:
```shell
func azure storage fetch-connection-string {{storage_account}}
```
{% endraw %}