---
layout: default
title: "xdg-user-dirs-update"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="xdg-user-dirs-update">
  <a href="/en/common/xdg-user-dirs-update.html">xdg-user-dirs-update</a> <a href="#xdg-user-dirs-update"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Update XDG user directories.
> More information: <https://manpages.ubuntu.com/manpages/bionic/man1/xdg-user-dirs-update.1.html>.

#### Change XDG's DESKTOP directory to the specified directory (must be absolute):
```shell
xdg-user-dirs-update --set DESKTOP "{{path/to/directory}}"
```
#### Write the result to the specified dry-run-file instead of the `user-dirs.dirs` file:
```shell
xdg-user-dirs-update --dummy-output "{{path/to/dry_run_file}}" --set {{xdg_user_directory}} "{{path/to/directory}}"
```
{% endraw %}