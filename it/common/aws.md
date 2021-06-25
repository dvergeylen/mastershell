---
layout: default
title: "aws"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aws">
  <a href="/it/common/aws.html">aws</a> <a href="#aws"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Il tool da linea di comando ufficiale per Amazon Web Services.
> Maggiori informazioni: <https://aws.amazon.com/cli>.

#### Lista tutti gli utenti IAM (Identity and Access Management):
```shell
aws iam list-users
```
#### Lista tutte le instanze EC2 per una specifica regione:
```shell
aws ec2 describe-instances --region {{us-east-1}}
```
#### Ricevi un messaggio da una specifica coda SQS:
```shell
aws sqs receive-message --queue-url {{https://queue.amazonaws.com/546123/Test}}
```
#### Pubblica un messaggio SNS su uno specifico argomento:
```shell
aws sns publish --topic-arn {{arn:aws:sns:us-east-1:54633:Agomento}} --message "Message"
```
#### Mostra la pagina di aiuto per uno specifico comando AWS:
```shell
aws {{comando}} help
```
{% endraw %}