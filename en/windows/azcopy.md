---
layout: default
title: "azcopy"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="azcopy">
  <a href="/en/windows/azcopy.html">azcopy</a> <a href="#azcopy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A file transfer tool for uploading to Azure Cloud Storage Accounts.
> More information: <https://docs.microsoft.com/azure/storage/common/storage-use-azcopy-v10>.

#### Log in to an Azure Tenant:
```shell
azopy login
```
#### Upload a local file:
```shell
azcopy copy '{{path/to/source/file}}' 'https://{{storage_account_name}}.blob.core.windows.net/{{container_name}}/{{blob_name}}'
```
#### Upload files with `.txt` and `.jpg` extensions:
```shell
azcopy copy '{{path/to/source}}' 'https://{{storage_account_name}}.blob.core.windows.net/{{container_name}}' --include-pattern '{{*.txt;*.jpg}}'
```
#### Copy a container directly between two Azure storage accounts:
```shell
azcopy copy 'https://{{source_storage_account_name}}.blob.core.windows.net/{{container_name}}' 'https://{{destination_storage_account_name}}.blob.core.windows.net/{{container_name}}'
```
#### Synchronize a local directory and delete files in the destination if they no longer exist in the source:
```shell
azcopy sync '{{path/to/source}}' 'https://{{storage_account_name}}.blob.core.windows.net/{{container_name}}' --recursive --delete-destination=true
```
#### Display detailed usage information:
```shell
azcopy --help
```
{% endraw %}