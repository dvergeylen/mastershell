---
layout: default
title: "aws s3api"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="aws-s3api">
  <a href="/en/common/aws-s3api.html">aws s3api</a> <a href="#aws-s3api"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create and delete Amazon S3 buckets and edit bucket properties.
> More information: <https://awscli.amazonaws.com/v2/documentation/api/latest/reference/s3api/index.html>.

#### Create a bucket:
```shell
aws s3api create-bucket --bucket {{bucket_name}}
```
#### Delete a bucket:
```shell
aws s3api delete-bucket --bucket {{bucket_name}}
```
#### List buckets:
```shell
aws s3api list-buckets
```
#### List the objects inside of a bucket and only show each object's key and size:
```shell
aws s3api list-objects --bucket {{bucket_name}} --query '{{Contents[].{Key: Key, Size: Size}}}'
```
#### Add an object to a bucket:
```shell
aws s3api put-object --bucket {{bucket_name}} --key {{object_key}} --body {{path/to/file}}
```
#### Download object from a bucket (The output file is always the last argument):
```shell
aws s3api get-object --bucket {{bucket_name}} --key {{object_key}} {{path/to/output_file}}
```
#### Apply an Amazon S3 bucket policy to a specified bucket:
```shell
aws s3api put-bucket-policy --bucket {{bucket_name}} --policy file://{{path/to/bucket_policy.json}}
```
#### Download the Amazon S3 bucket policy from a specified bucket:
```shell
aws s3api get-bucket-policy --bucket {{bucket_name}} --query Policy --output {{json|table|text|yaml|yaml-stream}} > {{path/to/bucket_policy}}
```
{% endraw %}