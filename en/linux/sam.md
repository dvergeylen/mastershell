---
layout: default
title: "sam"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="sam">
  <a href="/en/linux/sam.html">sam</a> <a href="#sam"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> AWS Serverless Application Model (SAM) CLI.
> More information: <https://github.com/awslabs/aws-sam-cli>.

#### Initialize a serverless application:
```shell
sam init
```
#### Initialize a serverless application with a specific runtime:
```shell
sam init --runtime {{python3.7}}
```
#### Package a SAM application:
```shell
sam package
```
#### Build your Lambda function code:
```shell
sam build
```
#### Run your serverless application locally:
```shell
sam local start-api
```
#### Deploy an AWS SAM application:
```shell
sam deploy
```
{% endraw %}