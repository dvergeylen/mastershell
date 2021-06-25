---
layout: default
title: "aws ecr"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aws-ecr">
  <a href="/en/common/aws-ecr.html">aws ecr</a> <a href="#aws-ecr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Push, pull, and manage container images.
> More information: <https://awscli.amazonaws.com/v2/documentation/api/latest/reference/ecr/index.html>.

#### Authenticate Docker with the default registry (username is AWS):
```shell
aws ecr get-login-password --region {{region}} | {{docker login}} --username AWS --password-stdin {{aws_account_id}}.dkr.ecr.{{region}}.amazonaws.com
```
#### Create a repository:
```shell
aws ecr create-repository --repository-name {{repository}} --image-scanning-configuration scanOnPush={{true|false}} --region {{region}}
```
#### Tag a local image for ECR:
```shell
docker tag {{container_name}}:{{tag}} {{aws_account_id}}.dkr.ecr.{{region}}.amazonaws.com/{{container_name}}:{{tag}}
```
#### Push an image to a repository:
```shell
docker push {{aws_account_id}}.dkr.ecr.{{region}}.amazonaws.com/{{container_name}}:{{tag}}
```
#### Pull an image from a repository:
```shell
docker pull {{aws_account_id}}.dkr.ecr.{{region}}.amazonaws.com/{{container_name}}:{{tag}}
```
#### Delete an image from a repository:
```shell
aws ecr batch-delete-image  --repository-name {{repository}} --image-ids imageTag={{latest}}
```
#### Delete a repository:
```shell
aws ecr delete-repository --repository-name {{repository}} --force
```
#### List images within a repository:
```shell
aws ecr list-images --repository-name {{repository}}
```
{% endraw %}