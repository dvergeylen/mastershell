---
layout: default
title: "rbt"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="rbt">
  <a href="/en/common/rbt.html">rbt</a> <a href="#rbt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> RBTools is a set of command-line tools for working with Review Board and RBCommons.
> More information: <https://www.reviewboard.org/docs/rbtools/dev/>.

#### Post changes to Review Board:
```shell
rbt post {{change_number}}
```
#### Display the diff that will be sent to Review Board:
```shell
rbt diff
```
#### Land a change in a local branch or on a review request:
```shell
rbt land {{branch_name}}
```
#### Patch your tree with a change on a review request:
```shell
rbt patch {{review_request_id}}
```
#### Set up RBTool to talk to a repository:
```shell
rbt setup-repo
```
{% endraw %}