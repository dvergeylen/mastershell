---
layout: default
title: "chgrp"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="chgrp">
  <a href="/it/common/chgrp.html">chgrp</a> <a href="#chgrp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cambia il gruppo proprietario di file e directory.
> Maggiori informazioni: <https://www.gnu.org/software/coreutils/chgrp>.

#### Cambia il gruppo proprietario di un file/directory:
```shell
chgrp {{gruppo}} {{percorso/al/file}}
```
#### Cambia ricorsivamente il gruppo proprietario di una directory e dei suoi contenuti:
```shell
chgrp -R {{gruppo}} {{percorso/a/directory}}
```
#### Cambia il gruppo proprietario di un link simbolico:
```shell
chgrp -h {{gruppo}} {{path/to/symlink}}
```
#### Cambia il gruppo proprietario di un file/directory rendendolo uguale a quello di un altro file di riferimento:
```shell
chgrp --reference={{percorso/al/file_riferimento}} {{percorso/al/file}}
```
{% endraw %}