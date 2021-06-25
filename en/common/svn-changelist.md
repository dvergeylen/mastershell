---
layout: default
title: "svn changelist"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="svn-changelist">
  <a href="/en/common/svn-changelist.html">svn changelist</a> <a href="#svn-changelist"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Associate a changelist with a set of files.
> More information: <http://svnbook.red-bean.com/en/1.7/svn.advanced.changelists.html>.

#### Add files to a changelist, creating the changelist if it does not exist:
```shell
svn changelist {{changelist_name}} {{path/to/file1}} {{path/to/file2}}
```
#### Remove files from a changelist:
```shell
svn changelist --remove {{path/to/file1}} {{path/to/file2}}
```
#### Remove the whole changelist at once:
```shell
svn changelist --remove --recursive --changelist {{changelist_name}} .
```
#### Add the contents of a space-separated list of directories to a changelist:
```shell
svn changelist --recursive {{changelist_name}} {{path/to/directory1}} {{path/to/directory2}}
```
#### Commit a changelist:
```shell
svn commit --changelist {{changelist_name}}
```
{% endraw %}