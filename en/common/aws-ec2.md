---
layout: default
title: "aws ec2"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aws-ec2">
  <a href="/en/common/aws-ec2.html">aws ec2</a> <a href="#aws-ec2"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI for AWS EC2.
> Provides secure and resizable computing capacity in the AWS cloud to enable faster development and deployment of applications.
> More information: <https://awscli.amazonaws.com/v2/documentation/api/latest/reference/ec2/index.html>.

#### Show list of all available EC2 commands:
```shell
aws ec2 help
```
#### Show help for specific EC2 subcommand:
```shell
aws ec2 {{subcommand}} help
```
#### Display information about a specific instance:
```shell
aws ec2 describe-instances --instance-ids {{instance_id}}
```
#### Display information about all instances:
```shell
aws ec2 describe-instances
```
#### Display information about all EC2 volumes:
```shell
aws ec2 describe-volumes
```
#### Delete an EC2 volume:
```shell
aws ec2 delete-volume --volume-id {{volume_id}}
```
#### Create a snapshot from an EC2 volume:
```shell
aws ec2 create-snapshot --volume-id {{volume_id}}
```
#### List available AMIs (Amazon Machine Images):
```shell
aws ec2 describe-images
```
{% endraw %}