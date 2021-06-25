---
layout: default
title: "bfg"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bfg">
  <a href="/en/common/bfg.html">bfg</a> <a href="#bfg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remove large files or passwords from Git history like git-filter-branch.
> Note: if your repository is connected to a remote, you will need to force push to it.
> More information: <https://rtyley.github.io/bfg-repo-cleaner/>.

#### Remove a file with sensitive data but leave the latest commit untouched:
```shell
bfg --delete-files {{file_with_sensitive_data}}
```
#### Remove all text mentioned in the specified file wherever it can be found in the repository's history:
```shell
bfg --replace-text {{path/to/file.txt}}
```
{% endraw %}