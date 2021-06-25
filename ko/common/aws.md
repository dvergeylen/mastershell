---
layout: default
title: "aws"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aws">
  <a href="/ko/common/aws.html">aws</a> <a href="#aws"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Amazon Web Services의 공식 CLI tool입니다.
> 더 많은 정보: <https://aws.amazon.com/cli>.

#### 모든 IAM 사용자 목록:
```shell
aws iam list-users
```
#### 특정 지역의 모든 ec2 인스턴스 나열:
```shell
aws ec2 describe-instances --region {{us-east-1}}
```
#### 특정 SQS 대기열에서 메시지 수신:
```shell
aws sqs receive-message --queue-url {{https://queue.amazonaws.com/546123/Test}}
```
#### 특정 SNS 주제에 메시지 게시:
```shell
aws sns publish --topic-arn {{arn:aws:sns:us-east-1:54633:testTopic}} --message "Message"
```
#### AWS 명령어에 대한 도움말을 보려면:
```shell
aws {{command}} help
```
{% endraw %}