---
layout: default
title: "ES"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#common">Common</a>
  * <a href="#7z">7z</a>
  * <a href="#[">[</a>
  * <a href="#aapt">aapt</a>
  * <a href="#ab">ab</a>
  * <a href="#adb">adb</a>
  * <a href="#alias">alias</a>
  * <a href="#asciinema">asciinema</a>
  * <a href="#awk">awk</a>
  * <a href="#base64">base64</a>
  * <a href="#bash">bash</a>
  * <a href="#bat">bat</a>
  * <a href="#cat">cat</a>
  * <a href="#cd">cd</a>
  * <a href="#chmod">chmod</a>
  * <a href="#chown">chown</a>
  * <a href="#clear">clear</a>
  * <a href="#cp">cp</a>
  * <a href="#cpdf">cpdf</a>
  * <a href="#cut">cut</a>
  * <a href="#docker">docker</a>
  * <a href="#docker-compose">docker-compose</a>
  * <a href="#dotnet">dotnet</a>
  * <a href="#dotnet-build">dotnet build</a>
  * <a href="#dotnet-publish">dotnet publish</a>
  * <a href="#dotnet-restore">dotnet restore</a>
  * <a href="#fortune">fortune</a>
  * <a href="#git-add">git add</a>
  * <a href="#git-am">git am</a>
  * <a href="#git-bisect">git bisect</a>
  * <a href="#git-blame">git blame</a>
  * <a href="#git-branch">git branch</a>
  * <a href="#git-check-ignore">git check-ignore</a>
  * <a href="#git-checkout">git checkout</a>
  * <a href="#git-cherry-pick">git cherry-pick</a>
  * <a href="#git-clean">git clean</a>
  * <a href="#git-clone">git clone</a>
  * <a href="#git-commit">git commit</a>
  * <a href="#git-config">git config</a>
  * <a href="#git-diff">git diff</a>
  * <a href="#git-fetch">git fetch</a>
  * <a href="#git-format-patch">git format-patch</a>
  * <a href="#git-gc">git gc</a>
  * <a href="#git-init">git init</a>
  * <a href="#git-lfs">git lfs</a>
  * <a href="#git-log">git log</a>
  * <a href="#git-ls-tree">git ls-tree</a>
  * <a href="#git-merge">git merge</a>
  * <a href="#git-mv">git mv</a>
  * <a href="#git-pr">git pr</a>
  * <a href="#git-pull">git pull</a>
  * <a href="#git-push">git push</a>
  * <a href="#git-rebase">git rebase</a>
  * <a href="#git-reflog">git reflog</a>
  * <a href="#git-remote">git remote</a>
  * <a href="#git-reset">git reset</a>
  * <a href="#git-restore">git restore</a>
  * <a href="#git-rev-list">git rev-list</a>
  * <a href="#git-rev-parse">git rev-parse</a>
  * <a href="#git-revert">git revert</a>
  * <a href="#git-rm">git rm</a>
  * <a href="#git-shortlog">git shortlog</a>
  * <a href="#git-show">git show</a>
  * <a href="#git-sizer">git sizer</a>
  * <a href="#git-stash">git stash</a>
  * <a href="#git-status">git status</a>
  * <a href="#git-submodule">git submodule</a>
  * <a href="#git-svn">git svn</a>
  * <a href="#git-switch">git switch</a>
  * <a href="#git-tag">git tag</a>
  * <a href="#git-worktree">git worktree</a>
  * <a href="#git-grep">git-grep</a>
  * <a href="#git-imerge">git-imerge</a>
  * <a href="#gradle">gradle</a>
  * <a href="#grep">grep</a>
  * <a href="#history">history</a>
  * <a href="#history-expansion">history expansion</a>
  * <a href="#htop">htop</a>
  * <a href="#keybase">keybase</a>
  * <a href="#ls">ls</a>
  * <a href="#mkdir">mkdir</a>
  * <a href="#more">more</a>
  * <a href="#mv">mv</a>
  * <a href="#mysql">mysql</a>
  * <a href="#mysqldump">mysqldump</a>
  * <a href="#nano">nano</a>
  * <a href="#nmap">nmap</a>
  * <a href="#nms">nms</a>
  * <a href="#rm">rm</a>
  * <a href="#tar">tar</a>
  * <a href="#tee">tee</a>
  * <a href="#tmux">tmux</a>
  * <a href="#touch">touch</a>
  * <a href="#unrar">unrar</a>
  * <a href="#wc">wc</a>
  * <a href="#xkill">xkill</a>
  * <a href="#yes">yes</a>

* <a href="#linux">Linux</a>
  * <a href="#apt">apt</a>
  * <a href="#apt-add-repository">apt-add-repository</a>
  * <a href="#apt-cache">apt-cache</a>
  * <a href="#apt-file">apt-file</a>
  * <a href="#apt-get">apt-get</a>
  * <a href="#apt-key">apt-key</a>
  * <a href="#apt-mark">apt-mark</a>
  * <a href="#aptitude">aptitude</a>
  * <a href="#archey">archey</a>
  * <a href="#bpytop">bpytop</a>
  * <a href="#brew">brew</a>
  * <a href="#cal">cal</a>
  * <a href="#calc">calc</a>
  * <a href="#clamav">clamav</a>
  * <a href="#cmus">cmus</a>
  * <a href="#conky">conky</a>
  * <a href="#dmesg">dmesg</a>
  * <a href="#dnf">dnf</a>
  * <a href="#dos2unix">dos2unix</a>
  * <a href="#free">free</a>
  * <a href="#groupdel">groupdel</a>
  * <a href="#halt">halt</a>
  * <a href="#line">line</a>
  * <a href="#lsb_release">lsb_release</a>
  * <a href="#lsmod">lsmod</a>
  * <a href="#lsusb">lsusb</a>
  * <a href="#ntfsfix">ntfsfix</a>
  * <a href="#pkgrm">pkgrm</a>
  * <a href="#poweroff">poweroff</a>
  * <a href="#pwdx">pwdx</a>
  * <a href="#reboot">reboot</a>
  * <a href="#rig">rig</a>
  * <a href="#shutdown">shutdown</a>
  * <a href="#top">top</a>
  * <a href="#userdel">userdel</a>
  * <a href="#xdg-open">xdg-open</a>

* <a href="#osx">Osx</a>
  * <a href="#afinfo">afinfo</a>
  * <a href="#afplay">afplay</a>
  * <a href="#airport">airport</a>
  * <a href="#apachectl">apachectl</a>
  * <a href="#archey">archey</a>
  * <a href="#as">as</a>
  * <a href="#asr">asr</a>
  * <a href="#brew">brew</a>
  * <a href="#rubocop">rubocop</a>
  * <a href="#spotify">spotify</a>


# Linux
{% raw %}
<h2 id="apt-add-repository">
  <a href="/es/linux/apt-add-repository.html">apt-add-repository</a> <a href="#apt-add-repository"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestiona las definiciones del repositorio apt.
> M??s informaci??n: <https://manpages.debian.org/latest/software-properties-common/apt-add-repository.1.html>.

#### A??ade un nuevo repositorio apt:
```shell
apt-add-repository {{repositorio}}
```
#### Elimina un repositorio apt:
```shell
apt-add-repository --remove {{repositorio}}
```
#### Actualiza la cach?? de paquetes tras a??adir un repositorio:
```shell
apt-add-repository --update {{repositorio}}
```
#### Activar las fuentes de paquetes:
```shell
apt-add-repository --enable-source {{repositorio}}
```
{% endraw %}{% raw %}
<h2 id="apt-cache">
  <a href="/es/linux/apt-cache.html">apt-cache</a> <a href="#apt-cache"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Herramienta de consulta de paquetes para Debian y Ubuntu.
> M??s informaci??n: <https://manpages.debian.org/latest/apt/apt-cache.8.html>.

#### Busca un paquete en tus fuentes actuales:
```shell
apt-cache search {{consulta}}
```
#### Muestra informaci??n de un paquete:
```shell
apt-cache show {{paquete}}
```
#### Muestra si un paquete est?? instalado y actualizado:
```shell
apt-cache policy {{paquete}}
```
#### Muestra las dependencias de un paquete:
```shell
apt-cache depends {{paquete}}
```
#### Muestra los paquetes que dependen de un paquete en particular:
```shell
apt-cache rdepends {{paquete}}
```
{% endraw %}{% raw %}
<h2 id="apt-file">
  <a href="/es/linux/apt-file.html">apt-file</a> <a href="#apt-file"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Busca archivos en paquetes apt, incluyendo los que a??n no fueron instalados.
> M??s informaci??n: <https://manpages.debian.org/latest/apt-file/apt-file.1.html>.

#### Actualiza los metadatos de la base de datos:
```shell
sudo apt update
```
#### Busca paquetes que contengan el archivo o ruta especificada:
```shell
apt-file search {{ruta/al/archivo}}
```
#### Muestra el contenido del paquete especificado:
```shell
apt-file list {{nombre_paquete}}
```
{% endraw %}{% raw %}
<h2 id="apt-get">
  <a href="/es/linux/apt-get.html">apt-get</a> <a href="#apt-get"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Herramienta de gesti??n de paquete para distribuciones basadas en Debian.
> Buscar paquetes utilizando `apt-cache`.
> M??s informaci??n: <https://manpages.debian.org/latest/apt/apt-get.8.html>.

#### Actualiza la lista de paquetes y versiones disponibles (se recomienda ejecutar este comando antes que cualquier otro comando `apt-get`):
```shell
apt-get update
```
#### Instala un paquete o actualizarlo a su ??ltima versi??n disponible:
```shell
apt-get install {{paquete}}
```
#### Elimina un paquete:
```shell
apt-get remove {{paquete}}
```
#### Elimina un paquete y sus archivos de configuraci??n:
```shell
apt-get purge {{paquete}}
```
#### Actualiza todos los paquetes instalados a sus nuevas versiones disponibles:
```shell
apt-get upgrade
```
#### Elimina todos los paquetes innecesarios:
```shell
apt-get autoremove
```
#### Actualiza paquetes instalados (como `upgrade`), pero elimina paquete obsoletos e instala paquetes adiciones para satisfacer nuevas dependencias:
```shell
apt-get dist-upgrade
```
{% endraw %}{% raw %}
<h2 id="apt-key">
  <a href="/es/linux/apt-key.html">apt-key</a> <a href="#apt-key"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Herramienta para la gesti??n de claves para el Gestor de Paquetes APT (APT Package Manager) en Debian y Ubuntu.
> M??s informaci??n: <https://manpages.debian.org/latest/apt/apt-key.8.html>.

#### Muestra las claves de confianza:
```shell
apt-key list
```
#### A??ade una clave al almac??n de claves de confianza):
```shell
apt-key add {{archivo_clave_p??blica.asc}}
```
#### Borrar una clave del almac??n de claves de confianza:
```shell
apt-key del {{id_clave}}
```
#### A??adir un clave remota al almac??n de claves de confianza:
```shell
wget -qO - {{https://host.tld/archivo.clave}} | apt-key add -
```
#### A??adir una clave de un servidor de claves con el identificador de la clave:
```shell
apt-key adv --keyserver {{pgp.mit.edu}} --recv {{id_clave}}
```
{% endraw %}{% raw %}
<h2 id="apt-mark">
  <a href="/es/linux/apt-mark.html">apt-mark</a> <a href="#apt-mark"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Herramienta para cambiar el estado de los paquetes instalados.
> M??s informaci??n: <https://manpages.debian.org/latest/apt/apt-mark.8.html>.

#### Marca un paquete como instalado autom??ticamente:
```shell
sudo apt-mark auto {{nombre_paquete}}
```
#### Mantiene un paquete en su versi??n actual y evita que se actualice:
```shell
sudo apt-mark hold {{nombre_paquete}}
```
#### Permite que un paquete pueda ser actualizado de nuevo:
```shell
sudo apt-mark unhold {{nombre_paquete}}
```
#### Muestra los paquetes instalados manualmente:
```shell
apt-mark showmanual
```
#### Muestra los paquetes mantenidos que no son actualizados:
```shell
apt-mark showhold
```
{% endraw %}{% raw %}
<h2 id="apt">
  <a href="/es/linux/apt.html">apt</a> <a href="#apt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Herramienta de gesti??n de paquete para distribuciones basadas en Debian.
> Se recomienda sustituirlo por apt-get cuando se use interactivamente en Ubuntu 16.04 o versiones posteriores.
> M??s informaci??n: <https://manpages.debian.org/latest/apt/apt.8.html>.

#### Actualiza la lista de paquetes y versiones disponibles (se recomienda ejecutar este comando antes que cualquier otro comando `apt`):
```shell
sudo apt update
```
#### Busca un paquete:
```shell
apt search {{paquete}}
```
#### Muestra la informaci??n de un paquete:
```shell
apt show {{paquete}}
```
#### Instala un paquete o lo actualiza a su ??ltima versi??n disponible:
```shell
sudo apt install {{paquete}}
```
#### Elimina un paquete (si se utiliza `purge` tambi??n elimina sus archivos de configuraci??n):
```shell
sudo apt remove {{paquete}}
```
#### Actualiza todos los paquetes a sus nuevas versiones disponibles:
```shell
sudo apt upgrade
```
#### Muestra todos los paquetes:
```shell
apt list
```
#### Muestra los paquetes instalados:
```shell
apt list --installed
```
{% endraw %}{% raw %}
<h2 id="aptitude">
  <a href="/es/linux/aptitude.html">aptitude</a> <a href="#aptitude"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Herramienta de gesti??n de paquetes para Debian y Ubuntu.
> M??s informaci??n: <https://manpages.debian.org/latest/aptitude/aptitude.8.html>.

#### Sincroniza la lista de paquetes y versiones disponible (se recomienda ejecutar este comando antes que cualquier otro comando `aptitude`):
```shell
aptitude update
```
#### Instalar un nuevo paquete y sus dependencias:
```shell
aptitude install {{paquete}}
```
#### Buscar un paquete:
```shell
aptitude search {{paquete}}
```
#### Buscar un paquete instalado (`?installed` es un t??rmino de b??squeda de `aptitude`):
```shell
aptitude search '?installed({{paquete}})'
```
#### Elimina un paquete y todos los paquetes que dependen de ??l:
```shell
aptitude remove {{paquete}}
```
#### Actualiza todos los paquetes sus nuevas versiones disponibles:
```shell
aptitude upgrade
```
#### Actualiza paquetes instalados (como `aptitude upgrade`), elimina los paquetes obsoletos e instala paquetes adicionales para satisfacer sus dependencias:
```shell
aptitude full-upgrade
```
#### Mantiente un paquete instalado para que no sea actualizado autom??ticamente:
```shell
aptitude hold '?installed({{paquete}})'
```
{% endraw %}{% raw %}
<h2 id="archey">
  <a href="/es/linux/archey.html">archey</a> <a href="#archey"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Herramienta sencilla para mostrar informaci??n del sistema con estilo.

#### Muestra informaci??n del sistema:
```shell
archey
```
{% endraw %}{% raw %}
<h2 id="bpytop">
  <a href="/es/linux/bpytop.html">bpytop</a> <a href="#bpytop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra informaci??n en tiempo real sobre procesos ejecut??ndose, con gr??ficos. Similar a `gtop` y `htop`.
> M??s informaci??n: <https://github.com/aristocratos/bpytop>.

#### Inicia bpytop:
```shell
bpytop
```
#### Inicia en modo m??nimalista sin recuadros de memoria y redes:
```shell
bpytop -m
```
#### Muestra la versi??n:
```shell
bpytop -v
```
#### Cambia a modo minimalista:
```shell
m
```
#### Busca procesos o programas ejecut??ndose:
```shell
f
```
#### Cambia ajustes:
```shell
M
```
{% endraw %}{% raw %}
<h2 id="brew">
  <a href="/es/linux/brew.html">brew</a> <a href="#brew"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestor de paquetes Homebrew para Linux.

#### Busca f??rmulas disponibles:
```shell
brew search {{texto}}
```
#### Instala la ??ltima versi??n de una f??rmula (usar `--devel` para la versi??n de desarrollo):
```shell
brew install {{formula}}
```
#### Lista todas las f??rmulas instaladas:
```shell
brew list
```
#### Actualizar una f??rmula instalada (si no se indica ninguna, todas las f??rmulas son actualizadas):
```shell
brew upgrade {{formula}}
```
#### Actualiza a la ??ltima versi??n de Linuxbrew y de todas las f??rmulas desde GitHub:
```shell
brew update
```
#### Mostrar las f??rmulas que tienen una versi??n m??s reciente disponible:
```shell
brew outdated
```
#### Mostrar la informaci??n de una f??rmula (versi??n, ruta de instalaci??n, dependencias, etc.):
```shell
brew info {{f??rmula}}
```
#### Revisar la instalaci??n local de Linuxbrew en busca de problemas potenciales:
```shell
brew doctor
```
{% endraw %}{% raw %}
<h2 id="cal">
  <a href="/es/linux/cal.html">cal</a> <a href="#cal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra el calendario, con el d??a actual resaltado.

#### Muestra el calendario para el mes actual:
```shell
cal
```
#### Muestra el mes anterior, actual y pr??ximo:
```shell
cal -3
```
#### Usa el Lunes como primer d??a de la semana:
```shell
cal --monday
```
#### Muestra el calendario para un a??o concreto (4 d??gitos):
```shell
cal {{year}}
```
#### Muestra el calendario para un a??o y mes concretos:
```shell
cal {{month}} {{year}}
```
{% endraw %}{% raw %}
<h2 id="calc">
  <a href="/es/linux/calc.html">calc</a> <a href="#calc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Una calculadora de precisi??n arbitraria en la terminal.

#### Iniciar calc en modo interactivo:
```shell
calc
```
#### Realizar un c??lculo en modo no-interactivo:
```shell
calc -p '{{85 * (36 / 4)}}'
```
{% endraw %}{% raw %}
<h2 id="clamav">
  <a href="/es/linux/clamav.html">clamav</a> <a href="#clamav"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Antivirus de c??digo abierto.
> Dise??ado especialment para escanear correos electr??nicos, pero puede ser usado en otros contextos.
> M??s informaci??n: <https://www.clamav.net>.

#### Actualiza definiciones de virus:
```shell
freshclam
```
#### Escanea un archivo en busca de virus:
```shell
clamscan {{ruta/al/archivo}}
```
#### Escanea directorios recursivamente y mostrar los archivos infectados:
```shell
clamscan --recursive --infected {{ruta/al/directorio}}
```
#### Escanea directorios recursivamente y poner los archivos infectados en cuarentena:
```shell
clamscan --recursive --move={{directorio}}
```
{% endraw %}{% raw %}
<h2 id="cmus">
  <a href="/es/linux/cmus.html">cmus</a> <a href="#cmus"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Reproductor de m??sica para la l??nea de comandos.
> Usa las teclas de direcci??n para navegar, `<enter/return>` para seleccionar, y los n??meros 1-8 para cambiar entra las diferentes vistas.

#### Abre cmus en un directorio concreto:
```shell
cmus {{ruta/al/directorio}}
```
#### A??ade un archivo/directorio a la librer??a:
```shell
:add {{ruta/al/archivo_o_directorio}}
```
#### Pausa/reproduce la canci??n actual:
```shell
c
```
#### Activa/desactiva modo aleatorio:
```shell
s
```
#### Cierra cmus:
```shell
q
```
{% endraw %}{% raw %}
<h2 id="conky">
  <a href="/es/linux/conky.html">conky</a> <a href="#conky"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Monitor de sistema ligero para X.
> M??s informaci??n: <https://github.com/brndnmtthws/conky>.

#### Ejecuta con la configuraci??n por defecto:
```shell
conky
```
#### Crea una nueva configuraci??n por defecto:
```shell
conky -C > ~/.conkyrc
```
#### Ejecuta conky con un archivo de configuraci??n concreto:
```shell
conky -c {{ruta/a/la/configuraci??n}}
```
#### Ejecuta en segundo plano (*daemon*):
```shell
conky -d
```
#### Alinea conky en el escritorio:
```shell
conky -a {{{arriba,abajo,en_medio}_{izquierda,derecha,en_medio}}}
```
#### Pausa de 5 segundos al inciar antes de ejecutarlo:
```shell
conky -p {{5}}
```
{% endraw %}{% raw %}
<h2 id="dmesg">
  <a href="/es/linux/dmesg.html">dmesg</a> <a href="#dmesg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Escribe los mensajes del n??cleo a la salida est??ndar.

#### Muestra los mensajes del n??cleo:
```shell
dmesg
```
#### Muestra los mensajes de error del n??cleo:
```shell
dmesg --level err
```
#### Muestra los mensajes del n??cleo y sigue leyedos los nuevos, similar a `tail -f` (disponible en los n??cleos 3.5.0 y posteriores):
```shell
dmesg -w
```
#### Muestra cuanta memoria f??sica hay disponible en este sistema:
```shell
dmesg | grep -i memory
```
#### Muestra los mensajes del n??cleo, p??gina a p??gina:
```shell
dmesg | less
```
#### Muestra los mensajes del n??cleo con una estampilla temporal (disponible en los n??cleos 3.5.0 y posteriores):
```shell
dmesg -T
```
#### Muestra los mensajes del n??cleo de forma legible para humanos (disponible en los n??cleos 3.5.0 y posteriores):
```shell
dmesg -H
```
#### Colorea la salida (disponible en los n??cleos 3.5.0 y posteriores):
```shell
dmesg -L
```
{% endraw %}{% raw %}
<h2 id="dnf">
  <a href="/es/linux/dnf.html">dnf</a> <a href="#dnf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Administrador de paquetes para RHEL, CentOS y Fedora (Reemplaza a yum).
> M??s informaci??n: <https://dnf.readthedocs.io>.

#### Actualiza todos los paquetes a la ??ltima versi??n disponible:
```shell
sudo dnf update
```
#### Busca un paquete usando palabras clave:
```shell
dnf search {{palabra_clave}}
```
#### Muestra informaci??n acerca de un paquete:
```shell
dnf info {{paquete}}
```
#### Instala un nuevo paquete:
```shell
sudo dnf install {{paquete}}
```
#### Instala un nuevo paquete respondiendo si a todas las preguntas:
```shell
sudo dnf install -y {{paquete}}
```
#### Lista todos los paquetes instalados:
```shell
dnf list --installed
```
#### Encuentra que paquete provee un archivo determinado:
```shell
dnf provides {{archivo}}
```
{% endraw %}{% raw %}
<h2 id="dos2unix">
  <a href="/es/linux/dos2unix.html">dos2unix</a> <a href="#dos2unix"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cambia saltos de l??nea con formato DOS a saltos de l??nea con formato Unix.
> Reemplaza CRLF con CR.

#### Cambia los saltos de l??nea de un archivo:
```shell
dos2unix {{nombre_de_archivo}}
```
#### Crea una copia con saltos de l??nea en formato Unix:
```shell
dos2unix -n {{nombre_de_archivo}} {{nombre_de_archivo}}
```
{% endraw %}{% raw %}
<h2 id="free">
  <a href="/es/linux/free.html">free</a> <a href="#free"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra la cantidad de memoria libre y usada en el sistema.

#### Muestra la memoria del sistema:
```shell
free
```
#### Muestra la memoria del sistema en Bytes/KB/MB/GB:
```shell
free -{{b|k|m|g}}
```
#### Muestra la memoria del sistema en unidades legibles por humanos:
```shell
free -h
```
#### Actualiza la salida cada 2 segundos:
```shell
free -s {{2}}
```
{% endraw %}{% raw %}
<h2 id="groupdel">
  <a href="/es/linux/groupdel.html">groupdel</a> <a href="#groupdel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Elimina del sistema grupos de usuarios existentes.
> M??s informaci??n: <https://manned.org/groupdel>.

#### Borra un grupo existente:
```shell
groupdel {{nombre_del_grupo}}
```
{% endraw %}{% raw %}
<h2 id="halt">
  <a href="/es/linux/halt.html">halt</a> <a href="#halt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Detiene, apaga o reinicia la m??quina.

#### Detiene la m??quina:
```shell
halt
```
#### Apaga la m??quina:
```shell
halt --poweroff
```
#### Reinicia la m??quina:
```shell
halt --reboot
```
{% endraw %}{% raw %}
<h2 id="line">
  <a href="/es/linux/line.html">line</a> <a href="#line"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lee una ??nica l??nea de entrada.

#### Lee una entrada:
```shell
line
```
{% endraw %}{% raw %}
<h2 id="lsb_release">
  <a href="/es/linux/lsb_release.html">lsb_release</a> <a href="#lsb_release"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Proporciona informaci??n espec??fica de la distribuci??n y LSB (Linux Standard Base).

#### Muestra toda la informaci??n disponible:
```shell
lsb_release -a
```
#### Muestra una descripci??n del sistema operativo (normalmente el nombre completo):
```shell
lsb_release -d
```
#### Muestra solo el nombre del sistema operativo (ID) sin el campo nombre:
```shell
lsb_release -i -s
```
#### Muestra el n??mero de versi??n y el nombre en clave de la distribuci??n sin el campo de nombre:
```shell
lsb_release -rcs
```
{% endraw %}{% raw %}
<h2 id="lsmod">
  <a href="/es/linux/lsmod.html">lsmod</a> <a href="#lsmod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra el estado de los m??dulos cargados en el kernel de linux.
> Vease tambien `modprobe`, el cual carga m??dulos de kernel.

#### Lista todos los m??dulos de kernel cargados:
```shell
lsmod
```
{% endraw %}{% raw %}
<h2 id="lsusb">
  <a href="/es/linux/lsusb.html">lsusb</a> <a href="#lsusb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra informaci??n sobre puertos y dispositivos USB.

#### Lista todos los dispositivos USB disponibles:
```shell
lsusb
```
#### Lista la jerarqu??a de dispositivos USB en forma de ??rbol:
```shell
lsusb -t
```
#### Lista los dispositivos USB de forma verbosa:
```shell
lsusb --verbose
```
#### Lista informaci??n detallada acerca de un dispositivo USB determinado:
```shell
lsusb -D {{dispositivo}}
```
#### Lista solo dispositivos con un ID de ensamblador y producto determinado:
```shell
lsusb -d {{ensamblador}}:{{producto}}
```
{% endraw %}{% raw %}
<h2 id="ntfsfix">
  <a href="/es/linux/ntfsfix.html">ntfsfix</a> <a href="#ntfsfix"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arregla problemas habituales de una partici??n NTFS.

#### Arregla una partici??n NTFS dada:
```shell
sudo ntfsfix {{/dev/sdXN}}
```
{% endraw %}{% raw %}
<h2 id="pkgrm">
  <a href="/es/linux/pkgrm.html">pkgrm</a> <a href="#pkgrm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Elimina un paquete de un sistema CRUX.

#### Elimina un paquete instalado:
```shell
pkgrm {{nombre_del_paquete}}
```
{% endraw %}{% raw %}
<h2 id="poweroff">
  <a href="/es/linux/poweroff.html">poweroff</a> <a href="#poweroff"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Apaga la m??quina.

#### Apaga la m??quina:
```shell
sudo poweroff
```
{% endraw %}{% raw %}
<h2 id="pwdx">
  <a href="/es/linux/pwdx.html">pwdx</a> <a href="#pwdx"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra el directorio de trabajo de un proceso.

#### Muestra el directorio de trabajo actual de un proceso:
```shell
pwdx {{process_id}}
```
{% endraw %}{% raw %}
<h2 id="reboot">
  <a href="/es/linux/reboot.html">reboot</a> <a href="#reboot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Reinicia la m??quina.

#### Reinicia inmediatamente:
```shell
reboot
```
#### Reinicia inmediatamente sin hacer un apagado limpio:
```shell
reboot -f
```
{% endraw %}{% raw %}
<h2 id="rig">
  <a href="/es/linux/rig.html">rig</a> <a href="#rig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilidad para generar un nombre, apellido, calle y n??mero, junto a ubicaci??n geogr??fica consistente (un conjunto v??lido de ciudad, estado y c??digo postal).
> M??s informaci??n: <https://manpages.ubuntu.com/manpages/focal/man6/rig.6.html>.

#### Muestra un nombre aleatorio (masculino o femenino) y una direcci??n:
```shell
rig
```
#### Muestra un nombre [m]asculino, (o [f]emenino) aleatorio y una direcci??n:
```shell
rig -{{m|f}}
```
#### Usa archivos de datos de un directorio espec??fico (por defecto es `/usr/share/rig`):
```shell
rig -d {{ruta/al/directorio}}
```
#### Especifica el n??mero de identidades a generar:
```shell
rig -c {{numero}}
```
#### Especifica el n??mero de identidades femininas a generar:
```shell
rig -f -c {{numero}}
```
{% endraw %}{% raw %}
<h2 id="shutdown">
  <a href="/es/linux/shutdown.html">shutdown</a> <a href="#shutdown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Detiene, apaga o reinicia la m??quina.

#### Detiene inmediatamente:
```shell
shutdown -H now
```
#### Apaga inmediatamente:
```shell
shutdown -h now
```
#### Reinicia inmediatamente:
```shell
shutdown -r now
```
#### Reinicia dentro de 5 minutos:
```shell
shutdown -r +{{5}} &
```
#### Apaga a la 1:00 PM (formato 24h):
```shell
shutdown -h 13:00
```
#### Cancela una operaci??n de apagado/reinicio pendiente:
```shell
shutdown -c
```
{% endraw %}{% raw %}
<h2 id="top">
  <a href="/es/linux/top.html">top</a> <a href="#top"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra informaci??n din??mica en tiempo real sobre procesos ejecut??ndose.

#### Inicia top:
```shell
top
```
#### No muestra ning??n proceso inactivo o zombie:
```shell
top -i
```
#### Muestra solo procesos pertenecientes a un usuario dado:
```shell
top -u {{usuario}}
```
#### Ordena procesos por una columna:
```shell
top -o {{nombre_columna}}
```
#### Muestra los hilos individuales de un proceso dado:
```shell
top -Hp {{id_proceso}}
```
#### Muestra solo los procesos con un(os) PID(s) dado(s), sepadados por comas. (Normalmente no se conoce el PID de antemano. Este ejemplo lo obtiene del nombre del proceso):
```shell
top -p $(pgrep -d ',' {{nombre_proceso}})
```
#### Obtiene ayuda acerca de los comandos interactivos:
```shell
?
```
{% endraw %}{% raw %}
<h2 id="userdel">
  <a href="/es/linux/userdel.html">userdel</a> <a href="#userdel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Elimina un usuario.
> M??s informaci??n: <https://manned.org/userdel>.

#### Elimina un usuario y su directorio personal:
```shell
userdel -r {{nombre_de_usuario}}
```
{% endraw %}{% raw %}
<h2 id="xdg-open">
  <a href="/es/linux/xdg-open.html">xdg-open</a> <a href="#xdg-open"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Abre un archivo o URL en la aplicaci??n predeterminada del usuario.
> M??s informaci??n: <https://man.archlinux.org/man/xdg-open.1>.

#### Abre el directorio actual en el explorador de archivos predeterminado:
```shell
xdg-open .
```
#### Abre una URL en el navegador predeterminado:
```shell
xdg-open {{https://www.ejemplo.es}}
```
#### Abre una image en el visor de im??genes predeterminado:
```shell
xdg-open {{ruta/al/imagen}}
```
#### Abre un PDF en el visor de PDF predeterminado:
```shell
xdg-open {{ruta/al/pdf}}
```
#### Muestra la ayuda:
```shell
xdg-open --help
```
{% endraw %}# Osx
{% raw %}
<h2 id="afinfo">
  <a href="/es/osx/afinfo.html">afinfo</a> <a href="#afinfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Analizador de metadatos de archivos de audio para OS X.
> Comando nativo de OS X.

#### Muestra informaci??n de un archivo de audio dado:
```shell
afinfo {{ruta/al/archivo}}
```
#### Muestra una descripci??n de una l??nea del archivo de audio:
```shell
afinfo -b {{ruta/al/archivo}}
```
#### Muestra informaci??n de metadatos y contenido del InfoDictionary del archivo de audio:
```shell
afinfo -i {{ruta/al/archivo}}
```
#### Imprime la salida en formato XML:
```shell
afinfo -x {{ruta/al/archivo}}
```
#### Muestra advertencias para el archivo de audio, si las hubiera:
```shell
afinfo --warnings {{ruta/al/archivo}}
```
#### Muestra ayuda para un uso completo:
```shell
afinfo -h
```
{% endraw %}{% raw %}
<h2 id="afplay">
  <a href="/es/osx/afplay.html">afplay</a> <a href="#afplay"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Reproductor de audio de l??nea de comandos.

#### Reproduce un archivo de audio (espera hasta que finalice la reproducci??n):
```shell
afplay {{ruta/al/archivo}}
```
#### Reproduce un archivo de audio a una velocidad 2x (velocidad de reproducci??n):
```shell
afplay --rate {{2}} {{ruta/al/archivo}}
```
#### Reproduce un archivo de audio a la mitad de velocidad:
```shell
afplay --rate {{0.5}} {{ruta/al/archivo}}
```
#### Reproduce los primeros N segundos de un archivo de audio:
```shell
afplay --time {{segundos}} {{ruta/al/archivo}}
```
{% endraw %}{% raw %}
<h2 id="airport">
  <a href="/es/osx/airport.html">airport</a> <a href="#airport"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilidad de configuraci??n de red inal??mbrica.

#### Muestra la informaci??n del estado actual de la red inal??mbrica:
```shell
airport -I
```
#### Detecta tr??fico inal??mbrico en el canal 1:
```shell
airport sniff {{1}}
```
#### Busca redes inal??mbricas disponibles:
```shell
airport -s
```
#### Desasociarse de la red actual:
```shell
sudo airport -z
```
{% endraw %}{% raw %}
<h2 id="apachectl">
  <a href="/es/osx/apachectl.html">apachectl</a> <a href="#apachectl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interfaz de control pata Apache HTTP Server para macOS.

#### Inicia la tarea launchd `org.apache.httpd`:
```shell
apachectl start
```
#### Finaliza la tarea launchd:
```shell
apachectl stop
```
#### Finaliza e inicia la tarea launchd:
```shell
apachectl restart
```
{% endraw %}{% raw %}
<h2 id="archey">
  <a href="/es/osx/archey.html">archey</a> <a href="#archey"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Herramienta sencilla para mostrar informaci??n del sistema con estilo.

#### Muestra informaci??n del sistema:
```shell
archey
```
#### Muestra informaci??n del sistema sin colorear la salida:
```shell
archey --nocolor
```
#### Muestra informaci??n del sistema, usando MacPorts en lugar de Hombrew:
```shell
archey --macports
```
#### Muestra informaci??n del sistema sin verificaci??n direcci??n IP:
```shell
archey --offline
```
{% endraw %}{% raw %}
<h2 id="as">
  <a href="/es/osx/as.html">as</a> <a href="#as"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ensamblador portable GNU.
> Principalmente destinado a ensamblar la salida de `gcc` para ser utilizada por` ld`.

#### Ensambla un archivo, escribiendo la salida en `a.out`:
```shell
as {{archivo.s}}
```
#### Ensambla la salida a un archivo especificado:
```shell
as {{archivo.s}} -o {{salida.o}}
```
#### Genera resultados m??s r??pido omitiendo los espacios en blanco y el preprocesamiento de comentarios. (Solo debe usarse para compiladores de confianza):
```shell
as -f {{archivo.s}}
```
#### Incluye una ruta determinada a la lista de directorios para buscar archivos especificados en las directivas `.include`:
```shell
as -I {{ruta/al/directorio}} {{archivo.s}}
```
{% endraw %}{% raw %}
<h2 id="asr">
  <a href="/es/osx/asr.html">asr</a> <a href="#asr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Restaura (copia) una imagen de disco en un volumen.
> El nombre del comando significa Restauraci??n de Software de Apple.

#### Restaura una imagen de disco en un volumen:
```shell
sudo asr restore --source {{nombre_de_imagen}}.dmg --target {{ruta/al/volumen}}
```
#### Borra el volumen deseado antes de restaurar:
```shell
sudo asr restore --source {{nombre_de_imagen}}.dmg --target {{ruta/al/volumen}} --erase
```
#### Omite la verificaci??n despu??s de restaurar:
```shell
sudo asr restore --source {{nombre_de_imagen}}.dmg --target {{ruta/al/volumen}} --noverify
```
#### Clona vol??menes sin el uso de una imagen de disco intermedia:
```shell
sudo asr restore --source {{ruta/al/volumen}} --target {{ruta/al/volumen_clonado}}
```
{% endraw %}{% raw %}
<h2 id="brew">
  <a href="/es/osx/brew.html">brew</a> <a href="#brew"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Administrador de paquetes para macOS.
> M??s informaci??n: <https://brew.sh>.

#### Busca f??rmulas y paquetes disponibles:
```shell
brew search {{text}}
```
#### Instala la ??ltima versi??n estable de una f??rmula (usa `--devel` para versiones de desarrollo):
```shell
brew install {{formula}}
```
#### Muestra todas las f??rmulas instaladas:
```shell
brew list
```
#### Muestra f??rmulas instaladas que no dependen de otras:
```shell
brew leaves
```
#### Actualiza una f??rmula instalada (si no se indica el nombre, se actualizan todas las f??rmulas):
```shell
brew upgrade {{formula}}
```
#### Actualiza a la ??ltima versi??n de Homebrew y todas sus f??rmulas desde GitHub:
```shell
brew update
```
#### Muestra informaci??n acerca de una f??rmula (versi??n, ruta de instalaci??n, dependencias, etc.):
```shell
brew info {{formula}}
```
#### Verifica la instalaci??n local de Homebrew en busca de problemas potenciales:
```shell
brew doctor
```
{% endraw %}{% raw %}
<h2 id="rubocop">
  <a href="/es/osx/rubocop.html">rubocop</a> <a href="#rubocop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Analiza archivos de Ruby.

#### Verifica todos los archivos en el directorio actual (incluyendo subdirectorios):
```shell
rubocop
```
#### Verifica uno o m??s archivos o directorios determinados:
```shell
rubocop {{path/to/file}} {{path/to/directory}}
```
#### Guarda la salida en un archivo:
```shell
rubocop --out {{path/to/file}}
```
#### Muestra la lista de cops (reglas de an??lisis):
```shell
rubocop --show-cops
```
#### Excluye una regla:
```shell
rubocop --except {{cop_1}} {{cop_2}}
```
#### Ejecuta s??lo determinadas reglas:
```shell
rubocop --only {{cop_1}} {{cop_2}}
```
#### Autocorrige archivos (experimental):
```shell
rubocop --auto-correct
```
{% endraw %}{% raw %}
<h2 id="spotify">
  <a href="/es/osx/spotify.html">spotify</a> <a href="#spotify"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Una l??nea de comando para Spotify.
> M??s informaci??n: <https://github.com/hnarayanan/shpotify>.

#### Encuentra una canci??n por su nombre y la reproduce:
```shell
spotify play {{song_name}}
```
#### Encuentra una lista de reproducci??n por su nombre y la reproduce:
```shell
spotify play list {{playlist_name}}
```
#### Pausa (o reanuda) la reproducci??n:
```shell
spotify pause
```
#### Pasa a la siguiente canci??n de una lista de reproducci??n:
```shell
spotify next
```
#### Cambia el volumen:
```shell
spotify vol {{up|down|value}}
```
#### Muestra el estado de reproducci??n y los detalles de la canci??n:
```shell
spotify status
```
{% endraw %}# Common
{% raw %}
<h2 id="7z">
  <a href="/es/common/7z.html">7z</a> <a href="#7z"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Un compresor de archivos con un alto ratio de compresi??n.
> M??s informaci??n: <https://www.7-zip.org/>.

#### Comprime un archivo o un directorio:
```shell
7z a {{archivo_comprimido.7z}} {{ruta/al/archivo_o_directorio_a_comprimir}}
```
#### Encriptar un archivo comprimido existente (incluyendo cabeceras):
```shell
7z a {{archivo_encriptado.7z}} -p{{contrase??a}} -mhe=on {{archivo_comprimido.7z}}
```
#### Extraer un archivo comprimido en formato `.7z` con la estructura original que ten??a antes de comprimir:
```shell
7z x {{archivo_comprimido.7z}}
```
#### Extraer un archivo comprimido en una ruta definida por el usuario:
```shell
7z x {{archivo_comprimido.7z}} -o {{ruta/donde/extraer}}
```
#### Extrae un archivo comprimido a stdout:
```shell
7z x {{archivo_comprimido.7z}} -so
```
#### Comprime usando un tipo de archivo comprimido espec??fico:
```shell
7z a -t{{zip|gzip|bzip2|tar}} {{archivo_comprimido.7z}} {{ruta/al/archivo_o_directorio_a_comprimir}}
```
#### Lista los tipos de archivo comprimido disponibles:
```shell
7z i
```
#### Lista el contenido de un archivo comprimido:
```shell
7z l {{archivo_comprimido.7z}}
```
{% endraw %}{% raw %}
<h2 id="[">
  <a href="/es/common/[.html">[</a> <a href="#["><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Eval??a una condicion.
> Retorna 0 si la condici??n se cumple, 1 si esta no se cumple.
> M??s informaci??n: <https://www.gnu.org/software/coreutils/test>.

#### Prueba si una variable dada es igual a una cadena dada:
```shell
[ "{{$VARIABLE}}" == "{{/bin/zsh}}" ]
```
#### Prueba si una variable dada est?? vac??a:
```shell
[ -z "{{$BRANCH_DE_GIT}}" ]
```
#### Prueba si un archivo existe:
```shell
[ -f "{{ruta/al/archivo}}" ]
```
#### Prueba si un directorio no existe:
```shell
[ ! -d "{{ruta/al/directorio}}" ]
```
#### Sentencia if-else:
```shell
[ {{condicion}} ] && {{echo "verdadero"}} || {{echo "falso"}}
```
{% endraw %}{% raw %}
<h2 id="aapt">
  <a href="/es/common/aapt.html">aapt</a> <a href="#aapt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Herramienta para empaquetado de activos de Android.
> Compila y empaqueta recursos de una app de Android.
> M??s informaci??n: <https://elinux.org/Android_aapt>.

#### Lista los archivos contenidos en un archivo APK:
```shell
aapt list {{ruta/al/app.apk}}
```
#### Muestra la metadata de una app (versi??n, permisos, etc.):
```shell
aapt dump badging {{ruta/al/app.apk}}
```
#### Crea un nuevo archivo APK con archivos de un directorio especificado:
```shell
aapt package -F {{ruta/al/app.apk}} {{ruta/al/directorio}}
```
{% endraw %}{% raw %}
<h2 id="ab">
  <a href="/es/common/ab.html">ab</a> <a href="#ab"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Herramienta comparativa del servidor Apache HTTP.
> M??s informaci??n: <https://httpd.apache.org/docs/current/programs/ab.html>.

#### Ejecuta 100 solicitudes HTTP GET a una URL dada:
```shell
ab -n {{100}} {{url}}
```
#### Ejecuta 100 solicitudes HTTP GET, en lotes simult??neos de a 10, a una URL:
```shell
ab -n {{100}} -c {{10}} {{url}}
```
#### Ejecuta 100 solicitudes HTTP POST a una URL, utilizando la carga JSON de un archivo:
```shell
ab -n {{100}} -T {{application/json}} -p {{ruta/al/archivo.json}} {{url}}
```
#### Utiliza HTTP [K]eep Alive, es decir, realiza m??ltiples solitudes dentro de una sesi??n HTTP:
```shell
ab -k {{url}}
```
#### Establece el m??ximo n??mero de segundos utilizados para la comparaci??n.
```shell
ab -t {{60}} {{url}}
```
{% endraw %}{% raw %}
<h2 id="adb">
  <a href="/es/common/adb.html">adb</a> <a href="#adb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge: comunica con una instancia de un emulador Android o conecta dispositivos Android.
> M??s informaci??n: <https://developer.android.com/studio/command-line/adb>.

#### Verifica si el proceso del servidor adb est?? ejecutandose y lo inicia:
```shell
adb start-server
```
#### Termina el proceso del servidor adb:
```shell
adb kill-server
```
#### Inicia una terminal remota en la instance del emulador/dispositivo de destino:
```shell
adb shell
```
#### Instala una aplicaci??n Android a un emulador/dispositivo:
```shell
adb install -r {{ruta/al/archivo.apk}}
```
#### Copia un archivo/directorio desde el dispositivo de destino:
```shell
adb pull {{ruta/al/archivo_o_directorio_en_el_dispositivo}} {{ruta/al/directorio_de_destino_local}}
```
#### Copia un archivo/directorio al dispositivo de destino:
```shell
adb push {{ruta/al/archivo_o_directorio_local}} {{ruta/al/directorio_de_destino_en_el_dispositivo}}
```
#### Obtiene una lista de dispositivos conectados:
```shell
adb devices
```
{% endraw %}{% raw %}
<h2 id="alias">
  <a href="/es/common/alias.html">alias</a> <a href="#alias"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Crea alias -- palabras que son remplazadas por una cadena de comando(s).
> Los alias son temporales en la sesi??n de shell actual, a no ser que est??n definidos en el archivo de configuraci??n de la shell, ej. `~/.bashrc`.
> M??s informaci??n: <https://tldp.org/LDP/abs/html/aliases.html>.

#### Listar todos los alias:
```shell
alias
```
#### Crear un alias gen??rico:
```shell
alias {{nombre}}="{{comando}}"
```
#### Ver el comando asociado a un alias:
```shell
alias {{nombre}}
```
#### Eliminar un alias (con el comando asociado):
```shell
unalias {{nombre}}
```
#### Convertir `rm` en un comando interactivo:
```shell
alias {{rm}}="{{rm -i}}"
```
#### Crear `la` como un atajo para `ls -a`:
```shell
alias {{la}}="{{ls -a}}"
```
{% endraw %}{% raw %}
<h2 id="asciinema">
  <a href="/es/common/asciinema.html">asciinema</a> <a href="#asciinema"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Graba y reproduce sesiones de terminal, y opcionalmente compartelas en asciinema.org.
> M??s informaci??n: <https://asciinema.org/>.

#### Asocia el programa local de `asciinema` con una cuenta de asciinema.org:
```shell
asciinema auth
```
#### Crea una nueva grabaci??n (una vez acabada, se pregutar?? al usuario si la quiere cuardar en local, o subirla):
```shell
asciinema rec
```
#### Crea una nueva grabaci??n y la guarda en un archivo local:
```shell
asciinema rec {{ruta/hacia/archivo}}.cast
```
#### Reproduce una grabaci??n desde un archivo local:
```shell
asciinema play {{ruta/hacia/archivo}}.cast
```
#### Reproduce una grabaci??n desde asciinema.org:
```shell
asciinema play https://asciinema.org/a/{{cast_id}}
```
#### Crea una nueva grabaci??n, limitando el tiempo de espera m??ximo a 2.5 segundos:
```shell
asciinema rec -i {{2.5}}
```
#### Imprime la salida completa de un archivo local de grabaci??n:
```shell
asciinema cat {{ruta/hacia/archivo}}.cast
```
#### Sube un archivo local de grabaci??n a asciinema.org:
```shell
asciinema upload {{ruta/hacia/archivo}}.cast
```
{% endraw %}{% raw %}
<h2 id="awk">
  <a href="/es/common/awk.html">awk</a> <a href="#awk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Un lenguaje de programaci??n vers??til para trabajar con archivos.
> M??s informaci??n: <https://github.com/onetrueawk/awk>.

#### Imprime la quinta columna (tambi??n conocido como campo) en un archivo separado por espacios:
```shell
awk '{print $5}' {{archivo}}
```
#### Imprime la segunda columna de las l??neas que contengan "algo" en un archivo separado por espacios:
```shell
awk '/{{algo}}/ {print $2}' {{archivo}}
```
#### Imprime la ??ltima columna de cada l??nea de un archivo, usando la coma (en vez de espacio) como separador de campo:
```shell
awk -F ',' '{print $NF}' {{archivo}}
```
#### Suma los valores en de la primera columna de un archivo e imprime el total:
```shell
awk '{s+=$1} END {print s}' {{archivo}}
```
#### Suma los valores en de la primera columna de un archivo e imprime el total de froma bonita:
```shell
awk '{s+=$1; print $1} END {print "--------"; print s}' {{archivo}}
```
#### Imprime cada tres l??neas, empezando por la primera:
```shell
awk 'NR%3==1' {{archivo}}
```
#### Imprime todos los valores desde la tercera columna:
```shell
awk '{for (i=3; i <= NF; i++) printf $i""FS; print""}' {{archivo}}
```
#### Imprime diferentes valores dependiendo de condiciones:
```shell
awk '{if ($1 == "foo") print "Coincidencia completa foo"; else if ($1 ~ "bar") print "Coincidencia parcial bar"; else print "Baz"}' {{archivo}}
```
{% endraw %}{% raw %}
<h2 id="base64">
  <a href="/es/common/base64.html">base64</a> <a href="#base64"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Codifica o decodifica un archivo o la entrada estandar hacia/desde Base64, a la salida estandar.
> M??s informaci??n: <https://www.gnu.org/software/coreutils/base64>.

#### Codifica un archivo:
```shell
base64 {{nombre_de_archivo}}
```
#### Decodifica un archivo:
```shell
base64 --decode {{nombre_de_archivo}}
```
#### Codifica stdin:
```shell
{{comando}} | base64
```
#### Decodifica stdin:
```shell
{{comando}} | base64 --decode
```
{% endraw %}{% raw %}
<h2 id="bash">
  <a href="/es/common/bash.html">bash</a> <a href="#bash"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bourne-Again SHell.
> Int??rprete de l??nea de comandos compatible con `sh`.
> M??s informaci??n: <https://gnu.org/software/bash>.

#### Inicia un int??rprete de comandos interactivo:
```shell
bash
```
#### Ejecuta un comando:
```shell
bash -c "{{comando}}"
```
#### Ejecuta comandos desde un archivo:
```shell
bash {{archivo.sh}}
```
#### Ejecuta comandos desde un archivo, mostrando todos los comando ejecutados en la terminal:
```shell
bash -x {{archivo.sh}}
```
#### Ejecuta comandos desde un archivo, deteni??ndose en el primer error:
```shell
bash -e {{archivo.sh}}
```
#### Ejecuta comandos desde stdin (entrada est??ndar):
```shell
bash -s
```
#### Imprime la informaci??n de la versi??n de bash (use `echo $BASH_VERSION` para ver s??lo la versi??n sin la informaci??n sobre la licencia):
```shell
bash --version
```
{% endraw %}{% raw %}
<h2 id="bat">
  <a href="/es/common/bat.html">bat</a> <a href="#bat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Imprime y concatena archivos.
> Un clon de `cat` con resaltado de sintaxis e integraci??n con Git.
> M??s informaci??n: <https://github.com/sharkdp/bat>.

#### Imprime los contenidos de un archivo a la salida est??ndar:
```shell
bat {{archivo}}
```
#### Concatena varios archivos creando un nuevo archivo:
```shell
bat {{archivo1}} {{archivo2}} > {{archivo_final}}
```
#### A??ade m??ltiples archivos al final de un archivo objetivo:
```shell
bat {{archivo1}} {{archivo2}} >> {{archivo_final}}
```
#### Numera las lineas del archivo:
```shell
bat -n {{archivo}}
```
#### Muestra un archivo JSON con resaltado de sintaxis:
```shell
bat --language json {{archivo.json}}
```
#### Muestra todos los lenguajes permitidos:
```shell
bat --list-languages
```
{% endraw %}{% raw %}
<h2 id="cat">
  <a href="/es/common/cat.html">cat</a> <a href="#cat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Imprime y concatena archivos.
> M??s informaci??n: <https://www.gnu.org/software/coreutils/cat>.

#### Imprime el contenido de un archivo por la salida est??ndar:
```shell
cat {{archivo}}
```
#### Concatena m??ltiples archivos dentro de un archivo determinado:
```shell
cat {{archivo1}} {{archivo2}} > {{archivo_final}}
```
#### A??ade m??ltiples archivos dentro de un archivo determinado:
```shell
cat {{archivo1}} {{archivo2}} >> {{archivo_final}}
```
#### Muestra el n??mero de l??neas de un archivo:
```shell
cat -n {{archivo}}
```
#### Muestra los car??cteres no imprimibles y espacios en blanco (con el prefijo `M-` si no es ASCII):
```shell
cat -v -t -e {{archivo}}
```
{% endraw %}{% raw %}
<h2 id="cd">
  <a href="/es/common/cd.html">cd</a> <a href="#cd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cambiar el directorio de trabajo.
> M??s informaci??n: <https://man.archlinux.org/man/cd.n>.

#### Accede al directorio especificado:
```shell
cd {{ruta/al/directorio}}
```
#### Accede al directorio *home* del usuario actual:
```shell
cd
```
#### Accede al directorio padre del directorio actual:
```shell
cd ..
```
#### Accede al directorio elegido previamente:
```shell
cd -
```
{% endraw %}{% raw %}
<h2 id="chmod">
  <a href="/es/common/chmod.html">chmod</a> <a href="#chmod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cambiar los permisos de acceso de un archivo o directorio.
> M??s informaci??n: <https://www.gnu.org/software/coreutils/chmod>.

#### Otorga al [u]suario que es propietario del archivo permiso para [x] ejecutarlo:
```shell
chmod u+x {{archivo}}
```
#### Otorga al usuario derechos para leer (r) y escribir (w) un archivo o directorio:
```shell
chmod u+rw {{archivo_o_directorio}}
```
#### Elimina los derechos de ejecuci??n del [g]rupo:
```shell
chmod g-x {{archivo}}
```
#### Otorga a todos los usuarios (a) derechos para leer y ejecutar:
```shell
chmod a+rx {{archivo}}
```
#### Otorga a [o]tros (que no est??n en el grupo del propietario) los mismos derechos que los del grupo:
```shell
chmod o=g {{archivo}}
```
#### Otorga al [g]rupo y a [o]tros el derecho para escribir (w) un directorio y su contenido:
```shell
chmod -R g+w,o+w {{directorio}}
```
{% endraw %}{% raw %}
<h2 id="chown">
  <a href="/es/common/chown.html">chown</a> <a href="#chown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cambia la propiedad de usuario y grupo sobre archivos y directorios.
> M??s informaci??n: <https://www.gnu.org/software/coreutils/chown>.

#### Cambia el usuario propietario de un archivo/directorio:
```shell
chown {{usuario}} {{ruta/hacia/archivo_o_directorio}}
```
#### Cambia el usuario y grupo propietario de un archivo/directorio:
```shell
chown {{usuario}}:{{grupo}} {{ruta/hacia/archivo_o_directorio}}
```
#### Cambia de forma recursiva el propietario sobre un directorio y su contenido:
```shell
chown -R {{usuario}} {{ruta/hacia/directorio}}
```
#### Cambia el propietario de un enlace simb??lico:
```shell
chown -h {{usuario}} {{ruta/hacia/enlace_simbolico}}
```
#### Copia la informaci??n de propiedad del archivo/directorio de referencia a otro:
```shell
chown --reference={{ruta/hacia/archivo_o_directorio_de_referencia}} {{ruta/hacia/archivo_o_directorio}}
```
{% endraw %}{% raw %}
<h2 id="clear">
  <a href="/es/common/clear.html">clear</a> <a href="#clear"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Limpia la pantalla de la terminal.
> M??s informaci??n: <https://manned.org/clear>.

#### Limpia la pantalla de la terminal (equivale a presionar Control-L en la interfaz de l??nea de comandos Bash):
```shell
clear
```
#### Limpia la pantalla pero mantiene el buffer de desplazamiento:
```shell
clear -x
```
#### Indica el tipo de terminal a limpiar (por defecto se utiliza el valor de la variable de entorno `TERM`):
```shell
clear -T {{tipo_de_terminal}}
```
#### Muestra la versi??n de `ncurses` utilizada por `clear`:
```shell
clear -V
```
{% endraw %}{% raw %}
<h2 id="cp">
  <a href="/es/common/cp.html">cp</a> <a href="#cp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Copia archivos y directorios.
> M??s informaci??n: <https://www.gnu.org/software/coreutils/cp>.

#### Copia un archivo a otra ruta:
```shell
cp {{ruta/hacia/archivo_original.ext}} {{ruta/hacia/archivo_copia.ext}}
```
#### Copia un archivo a un directorio, manteniendo el nombre del archivo:
```shell
cp {{ruta/hacia/archivo_original.ext}} {{ruta/hacia/directorio_destino}}
```
#### Copia de forma recursiva un directorio y su contenido a otra ruta (si la ruta de destino existe, el directorio se copiar?? dentro):
```shell
cp -R {{ruta/hacia/directorio_original}} {{ruta/hacia/directorio_copia}}
```
#### Copia de forma recursiva y verbosa un directorio (muestra un listado de los archivos copiados):
```shell
cp -vR {{ruta/hacia/directorio_original}} {{ruta/hacia/directorio_copia}}
```
#### Copia archivos de texto a otra ruta de forma interactiva (pregunta al usuario antes de sobreescribir):
```shell
cp -i {{*.txt}} {{ruta/hacia/directorio_destino}}
```
#### Copia enlaces simb??licos sin mantener la referencia al original:
```shell
cp -L {{enlace}} {{ruta/hacia/directorio_destino}}
```
{% endraw %}{% raw %}
<h2 id="cpdf">
  <a href="/es/common/cpdf.html">cpdf</a> <a href="#cpdf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interfaz de l??nea de comandos para manipular documentos PDF existentes de diferentes maneras.
> M??s informaci??n: <https://www.coherentpdf.com/cpdfmanudel/cpdfmanudel.html>.

#### Selecciona las p??ginas 1, 2, 3 y 6 del documento fuente y escribirlas en el documento objetivo:
```shell
cpdf {{ruta/al/documento_fuente.pdf}} {{1-3,6}} -o {{ruta/al/documento_objetivo.pdf}}
```
#### Fusiona dos documentos en uno nuevo:
```shell
cpdf -merge {{ruta/al/documento_fuente_uno.pdf}} {{ruta/al/documento_fuente_dos.pdf}} -o {{ruta/al/documento_objetivo.pdf}}
```
#### Muestra los marcadores del documento:
```shell
cpdf -list-bookmarks {{ruta/al/documento.pdf}}
```
#### Divide un documento en trozos de diez p??ginas, escribiendo `fragmento001.pdf`, `fragmento002.pdf`, etc:
```shell
cpdf -split {{ruta/al/documento.pdf}} -o {{ruta/al/fragmento%%%.pdf}} -chunk 10
```
#### Encripta un documento utilizando encriptado 128bit y establece `fred` como la contrase??a del propietario y `joe` como la contrase??a de usuario:
```shell
cpdf -encrypt 128bit fred joe {{ruta/al/documento_fuente.pdf}} -o {{ruta/al/documento_encriptado.pdf}}
```
#### Desencripta un documento utilizando la contrase??a del propietario (`fred`):
```shell
cpdf -decrypt {{ruta/al/documento_encriptado.pdf}} owner=fred -o {{ruta/al/documento_desencriptado.pdf}}
```
#### Muestra las anotaciones de un documento:
```shell
cpdf -list-annotations {{ruta/al/documento.pdf}}
```
#### Crea un nuevo documento, con metadatos, a partir de uno que ya existe:
```shell
cpdf -set-metadata {{ruta/de/los/metadatos.xml}} {{ruta/al/documento_fuente.pdf}} -o {{ruta/al/documento_objetivo.pdf}}
```
{% endraw %}{% raw %}
<h2 id="cut">
  <a href="/es/common/cut.html">cut</a> <a href="#cut"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Recorta campos provenientes de la entrada est??ndar o de archivos.
> M??s informaci??n: <https://www.gnu.org/software/coreutils/cut>

#### Recorta los primeros 16 caracteres de cada l??nea de la entrada est??ndar:
```shell
cut -c {{1-16}}
```
#### Recorta los primeros 16 caracteres de cada l??nea de los archivos especificados:
```shell
cut -c {{1-16}} {{archivo}}
```
#### Recorta todo desde el tercer caracter hasta el final de cada l??nea:
```shell
cut -c {{3-}}
```
#### Recorta el quinto campo de cada l??nea, usando los dos puntos como delimitadores de campos (por defecto el delimitador es tab):
```shell
cut -d'{{:}}' -f{{5}}
```
#### Recorta el segundo y d??cimo campo de cada l??nea, usando los punto y coma como delimitadores:
```shell
cut -d'{{;}}' -f{{2,10}}
```
#### Recorta los campos del tercero al ??ltimo de cada l??nea, usando los espacios como delimintadores:
```shell
cut -d'{{ }}' -f{{3-}}
```
{% endraw %}{% raw %}
<h2 id="docker-compose">
  <a href="/es/common/docker-compose.html">docker-compose</a> <a href="#docker-compose"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ejecuta y gestiona m??ltiples contenedores Docker.
> M??s informaci??n: <https://docs.docker.com/compose/reference/overview/>.

#### Lista los contenedores en ejecuci??n:
```shell
docker-compose ps
```
#### Crea e inicia todos los contenedores en segundo plano usando el archivo `docker-compose.yml` en el directorio actual:
```shell
docker-compose up -d
```
#### Inicia todos los contenedores y reconstruye si es ncesario:
```shell
docker-compose up --build
```
#### Inicia todos los contenedores usando un archivo compose alternativo:
```shell
docker-compose --file {{ruta/al/directorio}} up
```
#### Detiene todos los contenedores en ejecuci??n:
```shell
docker-compose stop
```
#### Detiene y elimina todos los contenedores, redes, im??genes y vol??menes:
```shell
docker-compose down --rmi all --volumes
```
#### Sigue los registros de todos los contenedores:
```shell
docker-compose logs --follow
```
{% endraw %}{% raw %}
<h2 id="docker">
  <a href="/es/common/docker.html">docker</a> <a href="#docker"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Administra contenedores e im??genes de Docker.
> M??s informaci??n: <https://docs.docker.com/engine/reference/commandline/cli/>.

#### Lista los contenedores de Docker en ejecuci??n:
```shell
docker ps
```
#### Lista todos los contenedores de Docker (en ejecuci??n y detenidos):
```shell
docker ps -a
```
#### Inicia un contenedor desde una imagen con un nombre personalizado:
```shell
docker run --name {{nombre_de_contenedor}} {{imagen}}
```
#### Inicia o detiene un contenedor existente:
```shell
docker {{start|stop}} {{nombre_de_contenedor}}
```
#### Descarga una imagen desde un registro de Docker:
```shell
docker pull {{imagen}}
```
#### Inicia una l??nea de Comandos dentro de un contenedor en ejecuci??n:
```shell
docker exec -it {{nombre_de_contenedor}} {{sh}}
```
#### Elimina un contenedor detenido:
```shell
docker rm {{nombre_de_contenedor}}
```
#### Obtiene y sigue los registros de un contenedor:
```shell
docker logs -f {{nombre_de_contenedor}}
```
{% endraw %}{% raw %}
<h2 id="dotnet-build">
  <a href="/es/common/dotnet-build.html">dotnet build</a> <a href="#dotnet-build"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compila una aplicaci??n .NET y sus dependencias.
> M??s informaci??n: <https://docs.microsoft.com/dotnet/core/tools/dotnet-build>.

#### Compila el proyecto o soluci??n en el directorio actual:
```shell
dotnet build
```
#### Compila un proyecto o soluci??n .NET en el modo de depuraci??n:
```shell
dotnet build {{ruta/al/proyecto_o_soluci??n}}
```
#### Compila en modo de lanzamiento:
```shell
dotnet build --configuration {{Release}}
```
#### Compila sin restaurar las dependencias:
```shell
dotnet build --no-restore
```
#### Compila con un nivel espec??fico de verbosidad:
```shell
dotnet build --verbosity {{quiet|minimal|normal|detailed|diagnostic}}
```
#### Compila para un tiempo de ejecuci??n espec??fico:
```shell
dotnet build --runtime {{identificador_del_tiempo_de_ejecuci??n}}
```
#### Especifica el directorio de salida:
```shell
dotnet build --output {{ruta/al/directorio}}
```
{% endraw %}{% raw %}
<h2 id="dotnet-publish">
  <a href="/es/common/dotnet-publish.html">dotnet publish</a> <a href="#dotnet-publish"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Publica una aplicaci??n .NET y sus dependencias en una carpeta para la implementaci??n en un sistema de hospedaje.
> M??s informaci??n: <https://docs.microsoft.com/dotnet/core/tools/dotnet-publish>.

#### Compila un proyecto .NET en modo de lanzamiento:
```shell
dotnet publish --configuration {{Release}} {{ruta/al/archivo_del_proyecto}}
```
#### Publica el entorno de ejecuci??n de .NET Core con la aplicaci??n para un entorno de ejecuci??n espec??fico:
```shell
dotnet publish --self-contained true --runtime {{identificador_del_entorno_en_tiempo_de_ejecuci??n}} {{ruta/al/archivo_del_proyecto}}
```
#### Empaqueta la aplicaci??n en un archivo ejecutable unico de una plataforma espec??fica:
```shell
dotnet publish --runtime {{identificador_del_entorno_en_tiempo_de_ejecucuci??n}} -p:PublishSingleFile=true {{ruta/al/archivo_del_proyecto}}
```
#### Recorta las bibliotecas no usadas para reducir el tama??o de la aplicaci??n:
```shell
dotnet publish --self-contained true --runtime {{identificador_del_entorno_de_tiempo_de_ejecuci??n}} -p:PublishTrimmed={{true}} {{ruta/al/archivo_del_proyecto}}
```
#### Compila un proyecto .NET sin restaurar las dependencias:
```shell
dotnet publish --no-restore {{ruta/al/archivo_del_proyecto}}
```
#### Especifica el directorio de salida:
```shell
dotnet publish --output {{ruta/al/directorio}} {{ruta/al/archivo_del_proyecto}}
```
{% endraw %}{% raw %}
<h2 id="dotnet-restore">
  <a href="/es/common/dotnet-restore.html">dotnet restore</a> <a href="#dotnet-restore"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Restarua las dependencias y herramientas de un proyecto .NET.
> M??s informaci??n: <https://docs.microsoft.com/dotnet/core/tools/dotnet-restore>.

#### Restaura dependencias para un proyecto o soluci??n .NET en el directorio actual:
```shell
dotnet restore
```
#### Restaura dependencias para un proyecto o soluci??n .NET en una ubicaci??n espec??fica:
```shell
dotnet restore {{ruta/al/proyecto_o_soluci??n}}
```
#### Restaura depedencias sin almacenar las solicitudes HTTP en cach??:
```shell
dotnet restore --no-cache
```
#### Obliga a todas las dependencias a ser resueltas incluso si la ??ltima restauraci??n fue exitosa:
```shell
dotnet restore --force
```
#### Restaura dependencias usando los or??genes con error como advertencias:
```shell
dotnet restore --ignore-failed-sources
```
#### Restaura dependencias con un nivel espec??fico de verbosidad:
```shell
dotnet restore --verbosity {{quiet|minimal|normal|detailed|diagnostic}}
```
{% endraw %}{% raw %}
<h2 id="dotnet">
  <a href="/es/common/dotnet.html">dotnet</a> <a href="#dotnet"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Herramienta multiplataforma de l??nea de comandos para .NET Core.
> M??s informaci??n: <https://docs.microsofot.com/dotnet/core/tools>.

#### Inicializa un proyecto .NET nuevo:
```shell
dotnet new {{nombre_de_la_plantilla}}
```
#### Restaura los paquetes NuGet:
```shell
dotnet restore
```
#### Compila y ejectura el proyecto .NET en el directorio actual:
```shell
dotnet run
```
#### Ejecuta una aplicaci??n dotnet empaquetada (solo necesita el entorno en tiempo de ejecuci??n, el resto de los comandos requieren el SDK de .NET Core instalado):
```shell
dotnet {{ruta/a/la/aplicaci??n.dll}}
```
{% endraw %}{% raw %}
<h2 id="fortune">
  <a href="/es/common/fortune.html">fortune</a> <a href="#fortune"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Imprime por pantalla una cita aleatoria (al estilo de una galleta de la suerte).
> M??s informaci??n: <https://man.archlinux.org/man/fortune.6>.

#### Imprime por pantalla una cita:
```shell
fortune
```
#### Imprime por pantalla una cita ofensiva:
```shell
fortune -o
```
#### Imprime por pantalla una cita larga:
```shell
fortune -l
```
#### Imprime por pantalla una cita corta:
```shell
fortune -s
```
#### Muestra una lista de los archivos de citas disponibles:
```shell
fortune -f
```
#### Imprime por pantalla una cita de uno de los archivos mostrados en `fortune -f`:
```shell
fortune {{archivo}}
```
{% endraw %}{% raw %}
<h2 id="git-add">
  <a href="/es/common/git-add.html">git add</a> <a href="#git-add"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A??ade los archivos cambiados al ??ndice.
> M??s informaci??n: <https://git-scm.com/docs/git-add>.

#### A??ade un archivo al ??ndice:
```shell
git add {{ruta/al/archivo}}
```
#### A??ade todos los archivos (rastreados o no rastreados):
```shell
git add -A
```
#### A??ade los archivos ya rastreados:
```shell
git add -u
```
#### A??ade tambi??n los archivos ignorados:
```shell
git add -f
```
#### A??ade partes de archivos interactivamente:
```shell
git add -p
```
#### A??ade partes de un archivo dado interactivamente:
```shell
git add -p {{ruta/al/archivo}}
```
#### A??ade un archivo interactivamente:
```shell
git add -i
```
{% endraw %}{% raw %}
<h2 id="git-am">
  <a href="/es/common/git-am.html">git am</a> <a href="#git-am"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Aplica archivos de parche. ??til cuando se reciben commits por correo electr??nico.
> V??ase tambi??n `git format-patch`, comando que genera archivo de parche.
> M??s informaci??n: <https://git-scm.com/docs/git-am>.

#### Aplica un archivo de parche:
```shell
git am {{ruta/al/archivo.patch}}
```
#### Aborta el proceso de aplicar un archivo de parche:
```shell
git am --abort
```
#### Aplica todo lo posible de un archivo de parche y guarda los fragmentos fallidos para rechazar archivos:
```shell
git am --reject {{ruta/al/archivo.patch}}
```
{% endraw %}{% raw %}
<h2 id="git-bisect">
  <a href="/es/common/git-bisect.html">git bisect</a> <a href="#git-bisect"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utiliza la b??squeda binaria para encontrar el commit que introdujo un error.
> Git salta de un lado a otro del gr??fico de commits para hasta alcanzar progresivamente el commit defectuoso.
> M??s informaci??n: <https://git-scm.com/docs/git-bisect>.

#### Comienza un sesi??n de bisecado en un rango de commits delimitada por un commit err??neo conocido y por uno sano conocido (normalmente m??s antiguo):
```shell
git bisect start {{commit_erroneo}} {{commit_bueno}}
```
#### Para cada commit que `git bisect` selecciona, marcarlo como "malo" o "bueno" despu??s de probarlo para el problema:
```shell
git bisect {{bueno|malo}}
```
#### Despu??s de que `git bisect` determine con precisi??n el commit defectuoso, termina la sesi??n de bisecado y vuelve a la rama anterior:
```shell
git bisect reset
```
#### Salta un commit durante una sesi??n de bisecado (p. ej., uno que falla las pruebas debido a un problema diferente):
```shell
git bisect skip
```
{% endraw %}{% raw %}
<h2 id="git-blame">
  <a href="/es/common/git-blame.html">git blame</a> <a href="#git-blame"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra el hash del commit y el ??ltimo autor de cada l??nea de un archivo.
> M??s informaci??n: <https://git-scm.com/docs/git-blame>.

#### Muestra el archivo con el nombre del autor y el hash del commit en cada l??nea:
```shell
git blame {{archivo}}
```
#### Muestra el archivo con correo electr??nico del autor y hash del commit en cada l??nea:
```shell
git blame -e {{archivo}}
```
{% endraw %}{% raw %}
<h2 id="git-branch">
  <a href="/es/common/git-branch.html">git branch</a> <a href="#git-branch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Comando Git principal para trabajar con ramas.
> M??s informaci??n: <https://git-scm.com/docs/git-branch>.

#### Muestra las ramas locales. La rama actual est?? resaltada por `*`:
```shell
git branch
```
#### Muestra todas las ramas (locales y remotas):
```shell
git branch -a
```
#### Muestra el nombre de la rama actual:
```shell
git branch --show-current
```
#### Crea una nueva rama basada en el commit actual:
```shell
git branch {{nombre_de_la_rama}}
```
#### Crea una nueva rama basada en un commit espec??fico:
```shell
git branch {{nombre_de_rama}} {{hash_del_commit}}
```
#### Renombra una rama (no debe haber sido fusionada para hacer esto):
```shell
git branch -m {{antiguo_nombre_de_la_rama}} {{nuevo_nombre_de_la_rama}}
```
#### Borra una rama local (no debe haber sido fusionada para hacer esto):
```shell
git branch -d {{nombre_de_la_rama}}
```
#### Borra una rama remota:
```shell
git push {{nombre_remoto}} --delete {{nombre_de_la_rama_remota}}
```
{% endraw %}{% raw %}
<h2 id="git-check-ignore">
  <a href="/es/common/git-check-ignore.html">git check-ignore</a> <a href="#git-check-ignore"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Analiza y depura los archivos que Git debe ignorar / excluir (.gitignore).
> M??s informaci??n: <https://git-scm.com/docs/git-check-ignore>.

#### Comprueba si un archivo o directorio es ignorado:
```shell
git check-ignore {{ruta/al/archivo_o_directorio}}
```
#### Comprueba si varios archivos o directorios son ignorados:
```shell
git check-ignore {{ruta/al/archivo}} {{ruta/al/directorio}}
```
#### Usa nombres de rutas, uno por l??nea, a partir de la entrada estandar (stdin):
```shell
git check-ignore --stdin < {{ruta/al/archivo_lista}}
```
#### No comprueba el ??ndice (se utiliza para depurar por qu?? las rutas fueron rastreadas y no ignoradas):
```shell
git check-ignore --no-index {{ruta/de_los/archivos_o_directorios}}
```
#### Incluye detalles sobre el patr??n de coincidencia para cada ruta:
```shell
git check-ignore --verbose {{ruta/de_los/archivos_o_directorios}}
```
{% endraw %}{% raw %}
<h2 id="git-checkout">
  <a href="/es/common/git-checkout.html">git checkout</a> <a href="#git-checkout"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Comprueba una rama o rutas con el arbol de trabajo.
> M??s informaci??n: <https://git-scm.com/docs/git-checkout>.

#### Crea una nueva rama y cambiarse a esta:
```shell
git checkout -b {{nombre_de_la_rama}}
```
#### Crea una nueva rama a partir de una referencia espec??fica (rama, remoto/rama, las etiquetas son ejemplos de referencias v??lidas) y cambiarse a esta:
```shell
git checkout -b {{nombre_de_la_rama}} {{referencia}}
```
#### Cambia a una rama local existente:
```shell
git checkout {{nombre_de_la_rama}}
```
#### Cambia a la rama previamente comprobada:
```shell
git checkout -
```
#### Cambia a una rama remota existente:
```shell
git checkout --track {{nombre_remoto}}/{{nombre_de_la_rama}}
```
#### Descarta todos los cambios sin marcar en el directorio actual (v??ase `git reset` para m??s comandos para deshacer):
```shell
git checkout .
```
#### Decarta los cambios no marcados de un archivo espec??fico:
```shell
git checkout {{nombre_del_archivo}}
```
#### Sustituir un archivo en el directorio actual con la versi??n de este en un commit de una rama espec??fica:
```shell
git checkout {{nombre_de_la_rama}} -- {{nombre_del_archivo}}
```
{% endraw %}{% raw %}
<h2 id="git-cherry-pick">
  <a href="/es/common/git-cherry-pick.html">git cherry-pick</a> <a href="#git-cherry-pick"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Aplica los cambios introducidos por commits existentes a la rama actual.
> Para aplicar cambios a otra rama, primero utiliza `git checkout` para cambiar a la rama deseada.
> M??s informaci??n: <https://git-scm.com/docs/git-cherry-pick>.

#### Aplica un commit a la rama actual:
```shell
git cherry-pick {{commit}}
```
#### Aplica un rango de commits de la rama actual (v??ase tambi??n `git rebase --onto`):
```shell
git cherry-pick {{commit_inicial}}~..{{commit_final}}
```
#### Aplica m??ltiples commits no secuenciales a la rama actual:
```shell
git cherry-pick {{commit_1}} {{commit_2}}
```
#### A??ade los cambios de un commit al directorio de trabajo, sin crear un commit:
```shell
git cherry-pick -n {{commit}}
```
{% endraw %}{% raw %}
<h2 id="git-clean">
  <a href="/es/common/git-clean.html">git clean</a> <a href="#git-clean"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Elimina archivos sin rastrear del ??rbol de trabajo.
> M??s informaci??n: <https://git-scm.com/docs/git-clean>.

#### Elimina archivos que no son rastreados por Git:
```shell
git clean
```
#### Elimina interactivamente archivos que no son rastreados por Git:
```shell
git clean -i
```
#### Muestra que archivos ser??an borrados sin llegar a borrarlos:
```shell
git clean --dry-run
```
#### Elimina forzosamente los archivos que no son rastreados por Git:
```shell
git clean -f
```
#### Elimina forzosamente los directorios que no son rastreados por Git:
```shell
git clean -fd
```
#### Elimina archivos sin rastrear, incluyendo los archivos ignorados en `.gitignore` y los excluidos en `.git/info/exclude`:
```shell
git clean -x
```
{% endraw %}{% raw %}
<h2 id="git-clone">
  <a href="/es/common/git-clone.html">git clone</a> <a href="#git-clone"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Clona un repositorio existente.
> M??s informaci??n: <https://git-scm.com/docs/git-clone>.

#### Clona un repositorio existente:
```shell
git clone {{ubicacion_remota_del_repositorio}}
```
#### Clona un repositorio existente en un directorio espec??fico:
```shell
git clone {{ubicacion_remota_del_repositorio}} {{ruta/al/directorio}}
```
#### Clona un repositorio existente y sus subm??dulos:
```shell
git clone --recursive {{ubicacion_remota_del_repositorio}}
```
#### Clona un repositorio local:
```shell
git clone -l {{ruta/al/repositorio/local}}
```
#### Clona silenciosamente:
```shell
git clone -q {{ubicacion_remota_del_repositorio}}
```
#### Clona un repositorio existente solo descargando los 10 commits m??s recientes de la rama por defecto (??til para ahorrar tiempo):
```shell
git clone --depth {{10}} {{ubicacion_remota_del_repositorio}}
```
#### Clona un repositorio existente solo descargando un branch espec??fico:
```shell
git clone --branch {{nombre}} --single-branch {{ubicacion_remota_del_repositorio}}
```
{% endraw %}{% raw %}
<h2 id="git-commit">
  <a href="/es/common/git-commit.html">git commit</a> <a href="#git-commit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Realiza commits de los archivos al repositorio.
> M??s informaci??n: <https://git-scm.com/docs/git-commit>.

#### Realiza un commit de los archivos marcados al repositorio con un mensaje:
```shell
git commit -m "{{mensaje}}"
```
#### Realiza un commit de los archivos marcados con un mensaje le??do desde un archivo:
```shell
git commit --file {{ruta/al/archivo_del_mensaje_del_commit}}
```
#### Marca autom??ticamente todos los archivos modificados y realiza un commit con un mensaje:
```shell
git commit -a -m "{{mensaje}}"
```
#### Sustituye el ??ltimo commit con los cambios marcados actualmente, cambiando el hash del commit:
```shell
git commit --amend
```
#### Realiza un commit para archivos espec??ficos (marcados previamente):
```shell
git commit {{ruta/al/archivo1}} {{ruta/al/archivo2}}
```
{% endraw %}{% raw %}
<h2 id="git-config">
  <a href="/es/common/git-config.html">git config</a> <a href="#git-config"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestiona opciones personalizadas para la configuraci??n de repositorios Git.
> Estas configuraciones pueden ser locales (para el repositorio actual) o globales (para el usuario actual).
> M??s informaci??n: <https://git-scm.com/docs/git-config>.

#### Muestra solo las entradas de la configuraci??n local (almacenadas en `.git/config` en el repositorio actual):
```shell
git config --list --local
```
#### Muestra solo las entradas de la configuraci??n global (almacenadas en `~/.gitconfig`):
```shell
git config --list --global
```
#### Muestra todas las entradas de configuraci??n que han sido definidas local o globalmente:
```shell
git config --list
```
#### Muestra el valor de una entrada espec??fica de la configuraci??n:
```shell
git config alias.unstage
```
#### Establece el valor global para una entrada espec??fica de la configuraci??n:
```shell
git config --global alias.unstage "reset HEAD --"
```
#### Revierte una entrada de la configuraci??n global a su valor por defecto:
```shell
git config --global --unset alias.unstage
```
#### Edita la configuraci??n de Git para el repositorio actual en el editor por defecto:
```shell
git config --edit
```
#### Edita la configuraci??n global de Git en el editor por defecto:
```shell
git config --global --edit
```
{% endraw %}{% raw %}
<h2 id="git-diff">
  <a href="/es/common/git-diff.html">git diff</a> <a href="#git-diff"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra los cambios de los archivos rastreados.
> M??s informaci??n: <https://git-scm.com/docs/git-diff>.

#### Muestra los cambios sin marcar ni commit:
```shell
git diff
```
#### Muestra todos los cambios sin commit, pero incluye los marcados:
```shell
git diff HEAD
```
#### Muestra solo los cambios marcados pero que no tienen commit:
```shell
git diff --staged
```
#### Muestra los cambios de todos los commits a partir de una fecha/tiempo espec??fico (una expresi??n de fecha, por ej., "1 week 2 days" o una fecha ISO):
```shell
git diff 'HEAD@{3 months|weeks|days|hours|seconds ago}
```
#### Muestra solo los nombres de los archivos cambiados con un commit espec??fico:
```shell
git diff --name-only {{commit}}
```
#### Muestra un resumen de la creaci??n, renombre y modos de cambio con un commit espec??fico:
```shell
git diff --summary {{commit}}
```
#### Compara un ??nico archivo entre dos ramas o commits:
```shell
git diff {{rama_1}}..{{rama_2}} [--] {{ruta/al/archivo}}
```
#### Compara diferentes archivos de la rama actual con otra rama:
```shell
git diff {{rama}}:{{ruta/al/archivo}} {{ruta/al/archivo2}}
```
{% endraw %}{% raw %}
<h2 id="git-fetch">
  <a href="/es/common/git-fetch.html">git fetch</a> <a href="#git-fetch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Descarga objetos y referencias de un repositorio remoto.
> M??s informaci??n: <https://git-scm.com/docs/git-fetch>.

#### Recibe los ??ltimos cambios del repositorio remoto upstream por defecto (si se ha establecido):
```shell
git fetch
```
#### Recibe las ramas nuevas de un repositorio remoto upstream espec??fico:
```shell
git fetch {{remote_name}}
```
#### Recibe los ??ltimos cambios de todos los repositorios remotos upstream:
```shell
git fetch --all
```
#### Recibe tambi??n las etiquetas de un repositorio upstream:
```shell
git fetch --tags
```
#### Elimina las referencias locales a ramas remotas que han sido eliminadas de upstream:
```shell
git fetch --prune
```
{% endraw %}{% raw %}
<h2 id="git-format-patch">
  <a href="/es/common/git-format-patch.html">git format-patch</a> <a href="#git-format-patch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Prepara archivos .patch. Es ??til cuando se env??an commits por correo electr??nico.
> V??ase tambi??n `git-am`, comando que puede aplicar los archivos .patch generados.
> M??s informaci??n: <https://git-scm.com/docs/git-format-patch>.

#### Crea un archivo `.patch` con nombre autom??tico para todos los cambios que no est??n en el push:
```shell
git format-patch {{origen}}
```
#### Escribe un archivo `.patch` para todos los commits entre dos revisiones a stdout:
```shell
git format-patch {{revisi??n_1}}..{{revisi??n_2}}
```
#### Escribe un archivo `.patch` para los 3 ??ltimos commits:
```shell
git format-patch -{{3}}
```
{% endraw %}{% raw %}
<h2 id="git-gc">
  <a href="/es/common/git-gc.html">git gc</a> <a href="#git-gc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Optimiza el repositorio local eliminando archivos innecesarios.
> M??s informaci??n: <https://git-scm.com/docs/git-gc>.

#### Optimiza el repositorio:
```shell
git gc
```
#### Optimiza agresivamente (tarda m??s):
```shell
git gc --aggressive
```
#### No elimina objetos sueltos (por defecto los elimina):
```shell
git gc --no-prune
```
#### Suprime toda la salida:
```shell
git gc --quiet
```
#### Muestra todas sus funcionalidades:
```shell
git gc --help
```
{% endraw %}{% raw %}
<h2 id="git-grep">
  <a href="/es/common/git-grep.html">git-grep</a> <a href="#git-grep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Encuentra dentro de archivos en cualquier parte del historial del repositorio.
> Acepta una gran cantidad de opciones, de la misma manera que el comando `grep`.
> M??s informaci??n: <https://git-scm.com/docs/git-grep>.

#### Busca una cadena en los archivos rastreados:
```shell
git grep {{cadena_a_buscar}}
```
#### Busca una cadena en archivos que coincidan con un patr??n entre los archivos rastreados:
```shell
git grep {{cadena_a_buscar}} -- {{patr??n_de_archivos}}
```
#### Busca una cadena en los archivos rastreados, incluyendo submodulos:
```shell
git grep --recurse-submodules {{cadena_a_buscar}}
```
#### Busca una cadena en un punto espec??fico del historial:
```shell
git grep {{cadena_a_buscar}} {{HEAD~2}}
```
#### Busca una cadena a trav??s de todas las ramas:
```shell
git grep {{cadena_a_buscar}} $(git rev-list --all)
```
{% endraw %}{% raw %}
<h2 id="git-imerge">
  <a href="/es/common/git-imerge.html">git-imerge</a> <a href="#git-imerge"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ejecuta una fusi??n o rebase entre dos ramas Git incrementalmente.
> Los conflictos entre las ramas se rastrean a pares de commits individuales para simplificar la resoluci??n de conflictos.
> M??s informaci??n: <https://github.com/mhagger/git-imerge>.

#### Inicia un rebase de tipo imerge (primero comprueba la rama a ser rebasada):
```shell
git imerge rebase {{rama_a_rebasar}}
```
#### Inicia una fusi??n de tipo imerge (primero comprueba la rama en la que fusionar):
```shell
git imerge merge {{rama_a_fusionar}}
```
#### Muestra una diagrama ASCII para la fusi??n o rebase en proceso:
```shell
git imerge diagram
```
#### Continua la operaci??n imerge despu??s de resolver los conflictos (primero a??ade con `git add` los archivos conflictivios):
```shell
git imerge continue --no-edit
```
#### Concluye una operaci??n imerge despu??s de que todos los conflictos se hayan resuelto:
```shell
git imerge finish
```
#### Aborta una operaci??n imerge y vuelve a la rama anterior:
```shell
git-imerge remove && git checkout {{rama_anterior}}
```
{% endraw %}{% raw %}
<h2 id="git-init">
  <a href="/es/common/git-init.html">git init</a> <a href="#git-init"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Inicializa un nuevo repositorio Git local.
> M??s informaci??n: <https://git-scm.com/docs/git-init>.

#### Inicializa un nuevo repositorio local:
```shell
git init
```
#### Inicializa un repositorio con un nombre especifico para la rama inicial:
```shell
git init --initial-branch={{nombre_de_la_rama}}
```
#### Inicializa un repositorio usando SHA256 como hash del objeto (requiere la versi??n 2.29+ de Git):
```shell
git init --object-format={{sha256}}
```
#### Inicializa un repositorio vac??o, adecuado para usarlo como remoto a trav??s de ssh:
```shell
git init --bare
```
{% endraw %}{% raw %}
<h2 id="git-lfs">
  <a href="/es/common/git-lfs.html">git lfs</a> <a href="#git-lfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Trabaja con archivos grandes en repositorios de Git.
> M??s informaci??n: <https://git-lfs.github.com>.

#### Inicializa Git LFS:
```shell
git lfs install
```
#### Rastrea archivos que coinciden con un patr??n:
```shell
git lfs track '{{*.bin}}'
```
#### Cambia la URL a la que apunta Git LFS (??til si el servidor LFS est?? separado del servidor Git):
```shell
git config -f .lfsconfig lfs.url {{url_del_punto_de_acceso_LFS}}
```
#### Muestra los patrones rastreados:
```shell
git lfs track
```
#### Muestra los archivos que han sido a??adidos con un commit:
```shell
git lfs ls-files
```
#### Introduce todos los objetos LFS en el servidor remoto (??til si se encuentran errores):
```shell
git lfs push --all {{nombre_remoto}} {{nombre_de_la_rama}}
```
#### Trae todos los objetos de Git LFS:
```shell
git lfs fetch
```
#### Verifica todos los objetos de Git LFS:
```shell
git lfs checkout
```
{% endraw %}{% raw %}
<h2 id="git-log">
  <a href="/es/common/git-log.html">git log</a> <a href="#git-log"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra un historial de commits.
> M??s informaci??n: <https://git-scm.com/docs/git-log>.

#### Muestra la secuencia de commits comenzando desde el actual, en orden cronol??gico inverso, del respositorio de Git en el directorio de trabajo actual:
```shell
git log
```
#### Muestra el historial de un archivo o directorio espec??fico, incluyendo las diferencias:
```shell
git log -p {{ruta/al/archivo_o_directorio}}
```
#### Muestra un resumen de los archivos, o archivo, cambiados en cada commit:
```shell
git log --stat
```
#### Muestra un gr??fico de los commits en la rama actual, utilizando solo la primer l??nea del mensaje de cada uno:
```shell
git log --oneline --graph
```
#### Muestra un gr??fico de todos los commits, etiquetas y ramas en todo el repositorio:
```shell
git log --oneline --decorate --all --graph
```
#### Muestra solo los commits cuyo mensaje incluye una cadena dada (no diferencia entre may??sculas y min??sculas):
```shell
git log -i --grep {{cadena_a_buscar}}
```
#### Muestra los ??ltimos N commits de cierto autor:
```shell
git log -n {{numero}} --author={{autor}}
```
#### Muestra los commits entre dos fechas:
```shell
git log --before={{fecha}} --after={{fecha}}
```
{% endraw %}{% raw %}
<h2 id="git-ls-tree">
  <a href="/es/common/git-ls-tree.html">git ls-tree</a> <a href="#git-ls-tree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra los contenidos de un objeto ??rbol.
> M??s informaci??n: <https://git-scm.com/docs/git-ls-tree>.

#### Muestra el contenido del ??rbol en una rama:
```shell
git ls-tree {{nombre_de_la_rama}}
```
#### Muestra el contenido del ??rbol en un commit (recursivo en sub??rboles):
```shell
git ls-tree -r {{hash_del_commit}}
```
#### Muestra solo los nombres de archivos del ??rbol en un commit:
```shell
git ls-tree --name-only {{hash_del_commit}}
```
{% endraw %}{% raw %}
<h2 id="git-merge">
  <a href="/es/common/git-merge.html">git merge</a> <a href="#git-merge"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Fusiona ramas.
> M??s informaci??n: <https://git-scm.com/docs/git-merge>.

#### Fusiona una rama con la rama actual:
```shell
git merge {{nombre_de_la_rama}}
```
#### Edita el mensaje de fusi??n:
```shell
git merge -e {{nombre_de_la_rama}}
```
#### Fusiona una rama y crea un commit para la fusi??n:
```shell
git merge --no-ff {{nombre_de_la_rama}}
```
#### Cancela una fusi??n en caso de conflictos:
```shell
git merge --abort
```
{% endraw %}{% raw %}
<h2 id="git-mv">
  <a href="/es/common/git-mv.html">git mv</a> <a href="#git-mv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mueve o renombra archivos y actualiza el ??ndice Git.
> M??s informaci??n: <https://git-scm.com/docs/git-mv>.

#### Mueve el archivo dentro del repositorio y a??ade el movimiento al siguiente commit:
```shell
git mv {{ruta/al/archivo}} {{nueva/ruta/al/archivo}}
```
#### Renombra un archivo y a??ade el renombre al siguiente commit:
```shell
git mv {{nombre_de_archivo}} {{nuevo_nombre_de_archivo}}
```
#### Sobrescribir el archivo en la ruta objetivo si existe:
```shell
git mv --force {{archivo}} {{objetivo}}
```
{% endraw %}{% raw %}
<h2 id="git-pr">
  <a href="/es/common/git-pr.html">git pr</a> <a href="#git-pr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Comprueba las solicitudes de extracci??n de cambios (*pull requests*) de GitHub localmente.
> M??s informaci??n: <https://github.com/tj/git-extras/blob/master/Commands.md#git-pr>.

#### Comprueba una pull request espec??fica:
```shell
git pr {{n??mero_pr}}
```
#### Comprueba una pull request para un remoto espec??fico:
```shell
git pr {{n??mero_pr}} {{remoto}}
```
#### Comprueba una pull request a partir de su URL:
```shell
git pr {{url}}
```
#### Limpia las ramas antiguas de pull requests:
```shell
git pr clean
```
{% endraw %}{% raw %}
<h2 id="git-pull">
  <a href="/es/common/git-pull.html">git pull</a> <a href="#git-pull"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Obtener rama de un repositorio remoto y fusionarlo con el repositorio local.
> M??s informaci??n: <https://git-scm.com/docs/git-pull>.

#### Descargar cambios del repositorio remoto por defecto y fusionarlo:
```shell
git pull
```
#### Descargar cambios del repositorio remoto por defecto y usar avance r??pido (*fast forward*):
```shell
git pull --rebase
```
#### Descargar cambios de un repositorio remoto y una rama espec??fica para fusionarlos en HEAD:
```shell
git pull {{nombre_remoto}} {{rama}}
```
{% endraw %}{% raw %}
<h2 id="git-push">
  <a href="/es/common/git-push.html">git push</a> <a href="#git-push"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Enviar (*push*) los commits al repositorio remoto.
> M??s informaci??n: <https://git-scm.com/docs/git-push>.

#### Envia los cambios locales en la rama actual a la misma rama en el remoto:
```shell
git push
```
#### Envia los cambios locales de una rama espec??fica a la misma rama en el remoto:
```shell
git push {{nombre_remoto}} {{rama_local}}
```
#### Publica la rama actual en el repositorio remoto y establece el nombre remoto de la rama:
```shell
git push {{nombre_remoto}} -u {{rama_remota}}
```
#### Envia los cambios de todas las ramas locales a sus respectivas ramas en el repositorio remoto:
```shell
git push --all {{nombre_remoto}}
```
#### Elimina una rama en el repositorio remoto:
```shell
git push {{nombre_remoto}} --delete {{rama_remota}}
```
#### Elimina las ramas remotas que no est??n en el repositorio local:
```shell
git push --prune {{nombre_remoto}}
```
#### Publica las etiquetas que a??n no est??n en el repositorio remoto:
```shell
git push --tags
```
{% endraw %}{% raw %}
<h2 id="git-rebase">
  <a href="/es/common/git-rebase.html">git rebase</a> <a href="#git-rebase"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Vuelve a aplicar commits de una rama en lo m??s alto de otra rama.
> Se utiliza com??nmente para "mover" una rama entera a otra base, ya que crea copias de los commits en una nueva ubicaci??n.
> M??s informaci??n: <https://git-scm.com/docs/git-rebase>.

#### Reorganiza la rama actual en lo m??s alto de otra rama:
```shell
git rebase {{rama_de_reorganizaci??n}}
```
#### Inicia un rebase interactivo que permite reordenar los commits, omitirlos, combinarlos o modificarlos:
```shell
git rebase -i {{rama_base_objetivo_o_hash_del_commit}}
```
#### Contin??a un rebase que fue interrumpido por una fusi??n fallida despu??s de editar los archivos con conflictos:
```shell
git rebase --continue
```
#### Contin??a un rebase que fue pausado para fusionar conflictos saltando el commit conflictivo:
```shell
git rebase --skip
```
#### Cancela un rebase en proceso (por ej., si es interrumpido por un conflicto de fusi??n):
```shell
git rebase --abort
```
#### Mueve parte de la rama actual a una nueva base proporcionando la base antigua para empezar:
```shell
git rebase --onto {{base_nueva}} {{base_antigua}}
```
#### Reaplica los ??ltimos 5 commits en su lugar, evita que puedan ser reordenados, omitidos, combinados o modificados:
```shell
git rebase -i {{HEAD~5}}
```
#### Resuelve autom??ticamente cualquier conflicto favoreciendo la versi??n de la rama en la que se esta trabajando (en este caso la palabra `theirs` tiene un significado invertido):
```shell
git rebase -X theirs {{rama_de_reorganizaci??n}}
```
{% endraw %}{% raw %}
<h2 id="git-reflog">
  <a href="/es/common/git-reflog.html">git reflog</a> <a href="#git-reflog"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra un registro de cambios de las referencias (*reflog*) locales como HEAD, ramas o etiquetas.
> M??s informaci??n: <https://git-scm.com/docs/git-reflog>.

#### Muestra un registro de referencias para HEAD:
```shell
git reflog
```
#### Muestra el registro de referencias para una rama:
```shell
git reflog {{nombre_de_la_rama}}
```
#### Muestra solo las ??ltimas 5 entradas en el registro de referencias:
```shell
git reflog -n {{5}}
```
{% endraw %}{% raw %}
<h2 id="git-remote">
  <a href="/es/common/git-remote.html">git remote</a> <a href="#git-remote"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestiona el conjunto de repositorios rastreados ("remotos").
> M??s informaci??n: <https://git-scm.com/docs/git-remote>.

#### Muestra una lista de los remotos existentes, sus nombres y URL:
```shell
git remote -v
```
#### Muestra informaci??n de un remoto:
```shell
git remote show {{nombre_remoto}}
```
#### A??ade un remoto:
```shell
git remote add {{nombre_remoto}} {{url_remoto}}
```
#### Cambiar la URL de un remoto (utiliza `--add` para mantener la URL existente):
```shell
git remote set-url {{nombre_remoto}} {{nueva_url}}
```
#### Elimina un remoto:
```shell
git remote remove {{nombre_remoto}}
```
#### Renombra un remoto:
```shell
git remote rename {{nombre_antiguo}} {{nombre_nuevo}}
```
{% endraw %}{% raw %}
<h2 id="git-reset">
  <a href="/es/common/git-reset.html">git reset</a> <a href="#git-reset"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Deshace commits o desmarca cambios mediante el reseteo del actual HEAD de Git al estado especificado.
> Si se pasa una ruta, funciona como "desmarcar", si se pasa el hash de un commit o una rama, funciona como "deshacer" el commit.
> M??s informaci??n: <https://git-scm.com/docs/git-reset>.

#### Desmarcar todo:
```shell
git reset
```
#### Desmarcar un archivo o archivos espec??ficos:
```shell
git reset {{ruta/al/archivo_o_archivos}}
```
#### Interactivamente desmarca partes de un archivo:
```shell
git reset --patch {{ruta/al/archivo}}
```
#### Deshace el ??ltimo commit, manteniendo sus cambios,y cualquier otro cambios sin commit,en el sistema de archivo:
```shell
git reset HEAD~
```
#### Deshace los ??ltimos dos commits al a??adir sus cambios al ??ndice (por ej., marcado para commit):
```shell
git reset --soft HEAD~2
```
#### Descartar cualquier cambio sin commit, marcado o no (se puede `git checkout` solo para los cambios sin marcar):
```shell
git reset --hard
```
#### Resetea el repositorio a un commit espec??fico y descarta a partir de este los cambios con y sin commit, y los marcados:
```shell
git reset --hard {{commit}}
```
{% endraw %}{% raw %}
<h2 id="git-restore">
  <a href="/es/common/git-restore.html">git restore</a> <a href="#git-restore"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Restaura los archivos del ??rbol de trabajo. Requiere la version 2.23+ de Git.
> V??ase tambi??n `git checkout` y `git reset`.
> M??s informaci??n: <https://git-scm.com/docs/git-restore>.

#### Restaura un archivo sin marcar a la versi??n del commit actual (HEAD):
```shell
git restore {{ruta/al/archivo}}
```
#### Restaura un archivo sin marcar a la versi??n de un commit espec??fico:
```shell
git restore --source {{commit}} {{ruta/al/archivo}}
```
#### Descarta los cambios sin commit para los archivos rastreados:
```shell
git restore :/
```
#### Desmarca un archivo:
```shell
git restore --staged {{ruta/al/archivo}}
```
#### Desmarca todos los archivos:
```shell
git restore --staged :/
```
#### Descarta todos los cambios de los archivos, marcados o no:
```shell
git restore --worktree --staged :/
```
#### Selecciona interactivamente secciones de archivos para restaurar:
```shell
git restore --patch
```
{% endraw %}{% raw %}
<h2 id="git-rev-list">
  <a href="/es/common/git-rev-list.html">git rev-list</a> <a href="#git-rev-list"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra las revisiones (commits) en orden cronol??gico inverso.
> M??s informaci??n: <https://git-scm.com/docs/git-rev-list>.

#### Muestra todos los commits de la rama actual:
```shell
git rev-list {{HEAD}}
```
#### Muestra los commits m??s recientes a partir de una fecha y una rama espec??fica:
```shell
git rev-list --since={{'2019-12-01 00:00:00'}} {{nombre_de_rama}}
```
#### Muestra todos los commits fusionados en un commit espec??fico:
```shell
git rev-list --merges {{commit}}
```
{% endraw %}{% raw %}
<h2 id="git-rev-parse">
  <a href="/es/common/git-rev-parse.html">git rev-parse</a> <a href="#git-rev-parse"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra metados relativos a revisiones espec??ficas.
> M??s informaci??n: <https://git-scm.com/docs/git-rev-parse>.

#### Obtiene el hash del commit de una rama:
```shell
git rev-parse {{nombre_de_la_rama}}
```
#### Obtiene el nombre de la rama actual:
```shell
git rev-parse --abbrev-ref {{HEAD}}
```
#### Obtiene la ruta absoluta al directorio ra??z:
```shell
git rev-parse --show-toplevel
```
{% endraw %}{% raw %}
<h2 id="git-revert">
  <a href="/es/common/git-revert.html">git revert</a> <a href="#git-revert"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Crea nuevos commits que revierten el efecton de los anteriores.
> M??s informaci??n: <https://git-scm.com/docs/git-revert>.

#### Revierte el commit m??s reciente:
```shell
git revert {{@}}
```
#### Revierte el quinto ??ltimo commit:
```shell
git revert HEAD~{{4}}
```
#### Revierte m??ltiples commits:
```shell
git revert {{rama~5..rama~2}}
```
#### No crea nuevos commits, solo cambia el ??rbol de trabajo:
```shell
git revert -n {{0c01a9..9a1743}}
```
{% endraw %}{% raw %}
<h2 id="git-rm">
  <a href="/es/common/git-rm.html">git rm</a> <a href="#git-rm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Elimina archivos del ??ndice del repositorio y del sistema de archivos local.
> M??s informaci??n: <https://git-scm.com/docs/git-rm>.

#### Elimina un archivo del ??ndice de un repositorio y del sistema de archivos local:
```shell
git rm {{archivo}}
```
#### Elimina un directorio:
```shell
git rm -r {{directorio}}
```
#### Elimina un archivo del ??ndice del repositorio, pero mantiene intacto el archivo local:
```shell
git rm --cached {{archivo}}
```
{% endraw %}{% raw %}
<h2 id="git-shortlog">
  <a href="/es/common/git-shortlog.html">git shortlog</a> <a href="#git-shortlog"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Resume la salida de `git log`.
> M??s informaci??n: <https://git-scm.com/docs/git-shortlog>.

#### Muestra un resumen de todos los commits realizados, agrupados alfab??ticamente por autor:
```shell
git shortlog
```
#### Muestra un resumen de todos los commits realizados, agrupados por el n??mero de commits realizados:
```shell
git shortlog -n
```
#### Muestra un resumen de todos los commits realizados, agrupados por la identidad de quien realiza el commit (usuario y correo electr??nico):
```shell
git shortlog -c
```
#### Muestra un resumen de los ??ltimos 5 commits (i. e., un rango de revisiones espec??fico):
```shell
git shortlog HEAD~{{5}}..HEAD
```
#### Muestra todos los usuarios, correos electr??nicos y n??mero de commits en la rama actual:
```shell
git shortlog -sne
```
#### Muestra todos los usuarios, correos electr??nicos y n??mero de commits en todas las ramas:
```shell
git shortlog -sne --all
```
{% endraw %}{% raw %}
<h2 id="git-show">
  <a href="/es/common/git-show.html">git show</a> <a href="#git-show"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra varios tipos de objetos Git (commits, etiquetas, etc??tera).
> M??s informaci??n: <https://git-scm.com/docs/git-show>.

#### Muestra informaci??n sobre el ??ltimo commit (hash, mensaje, cambios y otros metadatos):
```shell
git show
```
#### Muestra informaci??n de un commit espec??fico:
```shell
git show {{commit}}
```
#### Muestra informaci??n del commit asociado a una determinada etiqueta:
```shell
git show {{etiqueta}}
```
#### Muestra informaci??n del tercer commit desde la punta de una rama:
```shell
git show {{rama}}~{{3}}
```
#### Muestra el mensaje de un commit en una ??nica l??nea, eliminando el resultado de la diferencia:
```shell
git show --oneline -s {{commit}}
```
#### Muestra solo estad??sticas (caracteres agregados o removidos) de los archivos modificados:
```shell
git show --stat {{commit}}
```
#### Muestra solo la lista de archivos agregados, renombrados o eliminados:
```shell
git show --summary {{commit}}
```
#### Muestra el contenido de una archivo en una revisi??n espec??fica (por ej., una rama, una etiqueta o un commit):
```shell
git show {{revisi??n}}:{{ruta/al/archivo}}
```
{% endraw %}{% raw %}
<h2 id="git-sizer">
  <a href="/es/common/git-sizer.html">git sizer</a> <a href="#git-sizer"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Calcula diferentes m??tricas del repositorio Git y te informa de cualquier que puede causar problemas o inconvenientes.
> M??s informaci??n: <https://github.com/github/git-sizer>.

#### Reporta solo estad??sticas que tienen un nivel de preocupaci??n mayor que 0:
```shell
git sizer
```
#### Reporta todas las estad??sticas:
```shell
git sizer -v
```
#### Muestra opciones adicionales:
```shell
git sizer -h
```
{% endraw %}{% raw %}
<h2 id="git-stash">
  <a href="/es/common/git-stash.html">git stash</a> <a href="#git-stash"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Guarda cambios locales de Git en un ??rea temporal.
> M??s informaci??n: <https://git-scm.com/docs/git-stash>.

#### Guarda cambios actuales, excepto los archivos nuevos (sin rastrear):
```shell
git stash [push -m {{mensaje_opcional_del_guardado}}]
```
#### Guarda cambios actuales, incluyendo los archivos nuevos (sin rastrear):
```shell
git stash -u
```
#### Selecciona interactivamente las partes de archivos cambiados que deben ser guardadas:
```shell
git stash -p
```
#### Muestra todos los guardados (muestra el nombre del guardado, la rama relacionada y el mensaje):
```shell
git stash list
```
#### Aplica un guardado (por defecto aplica el ??ltimo, llamado stash@{0}):
```shell
git stash apply {{nombre_opcional_del_guardado_o_commit}}
```
#### Aplica un guardado (por defecto es stash@{0} y lo traslada desde la lista de guardado si no causa conflictos:
```shell
git stash pop {{nombre_opcional_del_guardado}}
```
#### Elimina un guardado (por defecto es stash@{0}):
```shell
git stash drop {{nombre_opcional_del_guardado}}
```
#### Elimina todos los guardados:
```shell
git stash clear
```
{% endraw %}{% raw %}
<h2 id="git-status">
  <a href="/es/common/git-status.html">git status</a> <a href="#git-status"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra los cambios realizados en los archivos del repositorio Git.
> Lista los archivos cambiados, a??adidos y eliminados compar??ndolos con el ??ltimo commit.
> M??s informaci??n: <https://git-scm.com/docs/git-status>.

#### Muestra los archivos cambiados que a??n no han sido a??adidos a un commit:
```shell
git status
```
#### Muestra la salida en formato breve:
```shell
git status -s
```
#### No muestra los archivos sin rastrear en la salida:
```shell
git status --untracked-files=no
```
#### Muestra la salida en formato breve junto a la informaci??n del branch:
```shell
git status --short --branch
```
{% endraw %}{% raw %}
<h2 id="git-submodule">
  <a href="/es/common/git-submodule.html">git submodule</a> <a href="#git-submodule"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Inspecciona, actualiza y gestiona los subm??dulos.
> M??s informaci??n: <https://git-scm.com/docs/git-submodule>.

#### Instala los subm??dulos espec??ficos de un repositorio:
```shell
git submodule update --init --recursive
```
#### A??ade un repositorio como un subm??dulo:
```shell
git submodule add {{url_del_repositorio}}
```
#### A??ade un repositorio Git como submulo en un directorio espec??fico:
```shell
git submodule add {{url_del_repositorio}} {{ruta/al/directorio}}
```
#### Actualiza cada subm??dulo a su ??ltimo commit:
```shell
git submodule foreach git pull
```
{% endraw %}{% raw %}
<h2 id="git-svn">
  <a href="/es/common/git-svn.html">git svn</a> <a href="#git-svn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Operacion bidreccional entre un repositorio Subversi??n y otro Git.
> M??s informaci??n: <https://git-scm.com/docs/git-svn>.

#### Clona un repositorio SVN:
```shell
git svn clone {{https://ejemplo.com/repositorio_subversion}} {{directorio_local}}
```
#### Clona un repositorio SVN a partir un n??mero de revisi??n espec??fico:
```shell
git svn clone -r{{1234}}:HEAD {{https://svn.ejemplo.net/subversion/repo}} {{directorio_local}}
```
#### Actualiza el clon local apartir del repositorio SVN:
```shell
git svn rebase
```
#### Obtiene las actualizaci??n del repositorio SVN remoto sin cambiar el HEAD de Git:
```shell
git svn fetch
```
#### Realiza un commit al repositorio SVN:
```shell
git svn dcommit
```
{% endraw %}{% raw %}
<h2 id="git-switch">
  <a href="/es/common/git-switch.html">git switch</a> <a href="#git-switch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Alterna entre ramas Git. Requiere una versi??n 2.23+ de Git.
> V??ase tambi??n `git checkout`.
> M??s informaci??n: <https://git-scm.com/docs/git-switch>.

#### Cambia a una rama existente:
```shell
git switch {{nombre_de_la_rama}}
```
#### Crea una nueva rama y se cambia a esta:
```shell
git switch --create {{nombre_de_la_rama}}
```
#### Crea una nueva rama basada en un commit espec??fico y se cambia a esta:
```shell
git switch --create {{nombre_de_la_rama}} {{commit}}
```
#### Cambia a la rama anterior:
```shell
git switch -
```
#### Cambia a una rama y actualiza todos los subm??dulos para coincidir:
```shell
git switch --recurse-submodules {{nombre_de_la_rama}}
```
#### Cambia a una rama y autom??ticamente fusiona la rama actual y cualquier cambio sin commit en ella:
```shell
git switch --merge {{nombre_de_la_rama}}
```
{% endraw %}{% raw %}
<h2 id="git-tag">
  <a href="/es/common/git-tag.html">git tag</a> <a href="#git-tag"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Crea, muestra, borra o verifica etiquetas.
> Una etiqueta es una referencia est??tica a un commit espec??fico.
> M??s informaci??n: <https://git-scm.com/docs/git-tag>.

#### Muestra todas las etiquetas:
```shell
git tag
```
#### Crea una etiqueta con el nombre especificado a partir del commit actual:
```shell
git tag {{nombre_de_la_etiqueta}}
```
#### Crea una etiqueta con el nombre especificado a partir del commit se??alado:
```shell
git tag {{nombre_de_la_etiqueta}} {{commit}}
```
#### Crea una etiqueta anotada con el mensaje especificado:
```shell
git tag {{nombre_de_la_etiqueta}} -m {{mensaje_de_la_etiqueta}}
```
#### Elimina la etiqueta con el nombre especificado:
```shell
git tag -d {{nombre_de_la_etiqueta}}
```
#### Obtiene las etiquetas actualizadas de upstreams:
```shell
git fetch --tags
```
#### Muestra todas las etiquetas cuyos ancestros incluyan un commit espec??fico:
```shell
git tag --contains {{commit}}
```
{% endraw %}{% raw %}
<h2 id="git-worktree">
  <a href="/es/common/git-worktree.html">git worktree</a> <a href="#git-worktree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestiona m??ltiples ??rboles de trabajo adjuntos al mismo repositorio.
> M??s informaci??n: <https://git-scm.com/docs/git-worktree>.

#### Crea un nuevo directorio con la rama espec??ficada y se cambia ??l:
```shell
git worktree add {{ruta/al/directorio}} {{rama}}
```
#### Crea un nuevo directorio con un nueva rama y se cambia a ??l:
```shell
git worktree add {{ruta/al/directorio}} -b {{rama_nueva}}
```
#### Muestra todos los directorios de trabajo adjuntos a este repositorio:
```shell
git worktree list
```
#### Elimina un ??rbol de trabajo (despu??s de eliminar el directorio del ??rbol de trabajo):
```shell
git worktree prune
```
{% endraw %}{% raw %}
<h2 id="gradle">
  <a href="/es/common/gradle.html">gradle</a> <a href="#gradle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gradle es un sistema de c??digo abierto para automatizar la compilaci??n de proyectos.
> M??s informaci??n: <https://gradle.org>.

#### Compila un proyecto:
```shell
gradle build
```
#### Excluye la tarea *test*:
```shell
gradle build -x {{test}}
```
#### Ejecuta en modo offline para prevenir que gradle acceda a la red durante una compilaci??n:
```shell
gradle build --offline
```
#### Limpia el directorio de compilaci??n:
```shell
gradle clean
```
#### Compila y genera un paquete:
```shell
gradle assembleRelease
```
{% endraw %}{% raw %}
<h2 id="grep">
  <a href="/es/common/grep.html">grep</a> <a href="#grep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Encuentra coincidencias en el texto introducido.
> Soporta patrones simples y expresiones regulares.
> M??s informaci??n: <https://www.gnu.org/software/grep/manual/grep.html>

#### Busca un patr??n dentro de un archivo:
```shell
grep {{patron}} {{ruta/al/archivo}}
```
#### Busca un patr??n exacto:
```shell
grep -F {{patron_exacto}} {{ruta/al/archivo}}
```
#### Busca un patr??n [R]ecursivamente en el directorio actual, mostrando los correspondientes [n]??meros de l??nea, [I]gnorando archivos binarios:
```shell
grep -RIn {{patron}} .
```
#### Usa expresiones regulares extendidas (soportando `?`, `+`, `{}`, `()` y `|`), sin importar may??sculas o min??sculas:
```shell
grep -Ei {{patron}} {{ruta/al/archivo}}
```
#### Imprime 3 l??neas de [C]ontexto alrededor, anteriores ([B]), o posteriores ([A]) tras la coincidencia:
```shell
grep -{{C|B|A}} 3 {{patron}} {{ruta/al/archivo}}
```
#### Imprime el nombre del archivo con la l??nea correspondiente a cada coincidencia:
```shell
grep -Hn {{patron}} {{ruta/al/archivo}}
```
#### Usa la entrada est??ndar en vez de un archivo:
```shell
cat {{ruta/al/archivo}} | grep {{patron}}
```
#### Encuentra coincidencias in[v]ersas al patr??n (aquellas l??neas que no lo contengan):
```shell
grep -v {{patron}}
```
{% endraw %}{% raw %}
<h2 id="history-expansion">
  <a href="/es/common/histexpand.html">history expansion</a> <a href="#history-expansion"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Reutiliza y expande el historial de la shell en `sh`, `bash`, `zsh`, `rbash` y `ksh`.
> M??s informaci??n: <https://www.gnu.org/software/bash/manual/html_node/History-Interaction>.

#### Ejecuta el ??ltimo comando:
```shell
!!
```
#### Ejecuta el ??ltimo comando como administrador:
```shell
sudo !!
```
#### Ejecuta un comando con el ??ltimo argumento del ??ltimo comando:
```shell
{{comando}} !$
```
#### Ejecuta un comando con el primer argumento del comando anterior:
```shell
{{comando}} !^
```
#### Ejecuta el comando `n` l??neas atr??s en el historial:
```shell
!-{{n}}
```
#### Ejecuta el ??ltimo comando con el prefijo `cadena`:
```shell
!{{cadena}}
```
#### Ejecuta el ??ltimo comando, reemplazando `cadena1` por `cadena2`:
```shell
^{{cadena1}}^{{cadena2}}^
```
#### Realiza una expansi??n del historial, pero muestra el comando que se ejecutar??a en lugar de ejecutarlo realmente:
```shell
{{!-n}}:p
```
{% endraw %}{% raw %}
<h2 id="history">
  <a href="/es/common/history.html">history</a> <a href="#history"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Historial de la l??nea de comandos.
> M??s informaci??n: <https://www.gnu.org/software/bash/manual/html_node/Bash-History-Builtins.html>.

#### Muestra el historial de comandos junto a su n??mero de l??nea:
```shell
history
```
#### Muestra los ??ltimos 20 comandos:
```shell
history {{20}}
```
#### Limpia el historial de comandos (solo para la shell actual):
```shell
history -c
```
#### Sobrescribe el archivo hist??rico con el historial de la shell actual (com??nmente se combina con `history -c` para limpiar el historial):
```shell
history -w
```
#### Borra la entrada del historial en el ??ndice especificado:
```shell
history -d {{indice}}
```
{% endraw %}{% raw %}
<h2 id="htop">
  <a href="/es/common/htop.html">htop</a> <a href="#htop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra informaci??n din??mica en tiempo real sobre los procesos ejecut??ndose. Una versi??n mejorada de `top`.

#### Inicia htop:
```shell
htop
```
#### Inicia htop mostrando solo procesos pertenecientes a un usuario dado:
```shell
htop -u {{usuario}}
```
#### Ordena procesos por columna (use `--sort-key help` para ver una lista de columnas):
```shell
htop -s {{nombre_columna}}
```
#### Recibe ayuda sobre comandos interactivos:
```shell
?
```
{% endraw %}{% raw %}
<h2 id="keybase">
  <a href="/es/common/keybase.html">keybase</a> <a href="#keybase"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Directorio de claves que conecta identidades en redes sociales a claves encriptadas de una manera p??blicamente auditable.
> M??s informaci??n: <https://keybase.io/docs/command_line>.

#### Sigue a otro usuario:
```shell
keybase follow {{nombre_de_usuario}}
```
#### A??ade una nueva prueba:
```shell
keybase prove {{servicio}} {{nombre_de_usuario_en_el_servicio}}
```
#### Firma un archivo:
```shell
keybase sign --infile {{archivo_de_entrada}} --outfile {{archivo_de_salida}}
```
#### Verifica un archivo firmado:
```shell
keybase verify --infile {{archivo_de_entrada}} --outfile {{archivo_de_salida}}
```
#### Encripta un archivo:
```shell
keybase encrypt --infile {{archivo_de_entrada}} --outfile {{archivo_de_salida}} {{receptor}}
```
#### Desencripta un archivo:
```shell
keybase decrypt --infile {{archivo_de_entrada}} --outfile {{archivo_de_salida}}
```
#### Revoca el dispositivo actual, se desconecta y borra los datos locales:
```shell
keybase deprovision
```
{% endraw %}{% raw %}
<h2 id="ls">
  <a href="/es/common/ls.html">ls</a> <a href="#ls"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lista los contenidos de directorios.
> M??s informaci??n: <https://www.gnu.org/software/coreutils/ls>.

#### Lista un archivo por l??nea:
```shell
ls -1
```
#### Lista todos los archivos, incluyendo archivos ocultos:
```shell
ls -a
```
#### Lista todos los archivos, a??adiendo `/` al final de los nombres de directorios:
```shell
ls -F
```
#### Lista todos los archivos con formato largo (permisos, propietario, tama??o y fecha de modificaci??n):
```shell
ls -la
```
#### Lista con formato largo y tama??o legible por humanos (KiB, MiB, GiB):
```shell
ls -lh
```
#### Lista con formato largo y tama??o en orden descendente:
```shell
ls -lS
```
#### Lista todos los archivos con formato largo, ordenado por fecha de modificaci??n (archivos m??s viejos en primer lugar):
```shell
ls -ltr
```
{% endraw %}{% raw %}
<h2 id="mkdir">
  <a href="/es/common/mkdir.html">mkdir</a> <a href="#mkdir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Crea un directorio.
> M??s informaci??n: <https://www.gnu.org/software/coreutils/mkdir>.

#### Crea un directorio en el directorio actual o en una ruta dada:
```shell
mkdir {{directorio}}
```
#### Crea directorios recursivamente (??til para crear directorios anidados):
```shell
mkdir -p {{ruta/al/directorio}}
```
{% endraw %}{% raw %}
<h2 id="more">
  <a href="/es/common/more.html">more</a> <a href="#more"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Abre un archivo para lectura interactiva, permitiendo navegar y buscar.
> M??s informaci??n: <https://manned.org/more>.

#### Abre un archivo:
```shell
more {{ruta/al/archivo}}
```
#### Abre un archivo mostrando desde una l??nea especifica:
```shell
more +{{numero_linea}} {{ruta/al/archivo}}
```
#### Muestra la ayuda:
```shell
more --help
```
#### Avanza hacia la siguiente p??gina:
```shell
<Espacio>
```
#### Busca una cadena (presione `n` para ir a la siguiente coincidencia):
```shell
/{{cadena}}
```
#### Salir:
```shell
q
```
#### Muestra la ayuda sobre comandos interactivos:
```shell
h
```
{% endraw %}{% raw %}
<h2 id="mv">
  <a href="/es/common/mv.html">mv</a> <a href="#mv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mueve o renombra archivos y directorios.
> M??s informaci??n: <https://www.gnu.org/software/coreutils/mv>.

#### Mueve archivos en ubicaciones arbitrarias:
```shell
mv {{origen}} {{destino}}
```
#### Mueve sin solicitar confirmaci??n antes de sobrescribir archivos existentes:
```shell
mv -f {{origen}} {{destino}}
```
#### Solicita confirmaci??n antes de sobrescribir archivos existentes, independientemente de los permisos del archivo:
```shell
mv -i {{origen}} {{destino}}
```
#### No sobrescribe archivos existentes en el destino:
```shell
mv -n {{origen}} {{destino}}
```
#### Mueve archivos en modo detallado, mostrando los archivos despu??s de moverlos:
```shell
mv -v {{origen}} {{destino}}
```
{% endraw %}{% raw %}
<h2 id="mysql">
  <a href="/es/common/mysql.html">mysql</a> <a href="#mysql"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Herramienta de l??nea de comandos para gestionar bases de datos MySQL.
> M??s informaci??n: <https://www.mysql.com/>.

#### Conecta a una base de datos:
```shell
mysql {{nombre_base_de_datos}}
```
#### Conecta a una base de datos con el usuario `usuario` y se le pedir?? la contrase??a:
```shell
mysql -u {{usuario}} --password {{nombre_base_de_datos}}
```
#### Conecta a una base de datos en otra m??quina:
```shell
mysql -h {{maquina_remota}} {{nombre_base_de_datos}}
```
#### Conecta a una base de datos a trav??s de un socket unix:
```shell
mysql --socket {{ruta/al/socket.sock}}
```
#### Ejecuta comandos SQL contenidos en un script:
```shell
mysql -e "source {{archivo.sql}}" {{nombre_base_de_datos}}
```
#### Restaura una base de datos a partir de una copia de seguridad creada con `mysqldump` (y se le pedir?? la contrase??a al usuario):
```shell
mysql --user {{usuario}} --password {{nombre_base_de_datos}} < {{ruta/al/backup.sql}}
```
#### Restaura todas las bases de datos en una copia de seguridad (y se le pedir?? la contrase??a al usuario):
```shell
mysql --user {{usuario}} --password < {{ruta/al/backup.sql}}
```
{% endraw %}{% raw %}
<h2 id="mysqldump">
  <a href="/es/common/mysqldump.html">mysqldump</a> <a href="#mysqldump"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Crea una copia de seguridad de bases de datos MySQL.
> Vea tambi??n `mysql` para restaurar bases de datos.
> M??s informaci??n: <https://dev.mysql.com/doc/refman/en/mysqldump.html>.

#### Crea un backup (se le pedir?? la contrase??a al usuario):
```shell
mysqldump --user {{usuario}} --password {{nombre_base_de_datos}} -r {{ruta/al/archivo.sql}}
```
#### Crea un backup de todas las bases de datos y redirige la salida a un archivo (se le pedir?? la contrase??a al usuario):
```shell
mysqldump --user {{usuario}} --password --all-databases > {{ruta/al/archivo.sql}}
```
#### Crea un backup de una ??nica tabla de una base de datos (se le pedir?? la contrase??a al usuario):
```shell
mysqldump --user {{usuario}} --password {{nombre_base_de_datos}} {{nombre_tabla}} -r {{ruta/al/archivo.sql}}
```
{% endraw %}{% raw %}
<h2 id="nano">
  <a href="/es/common/nano.html">nano</a> <a href="#nano"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Editor sencillo y f??cil de usar. Un clon libre y mejorado de Pico.
> M??s informaci??n: <https://nano-editor.org>.

#### Inicia nano en la terminal con {nombre_del_archivo}:
```shell
nano {{nombre_del_archivo}}
```
#### Activar desplazamiento suave:
```shell
nano -S {{nombre_del_archivo}}
```
#### Sangra las nuevas l??neas a la sangr??a de las l??neas anteriores:
```shell
nano -i {{nombre_del_archiv}}
```
{% endraw %}{% raw %}
<h2 id="nmap">
  <a href="/es/common/nmap.html">nmap</a> <a href="#nmap"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Herramienta de exploraci??n de redes y esc??ner de seguridad / puertos.
> Algunas caracter??sticas solo funcionan si ejecutamos Nmap con privilegios.
> M??s informaci??n: <https://nmap.org>.

#### Comprueba si una direcci??n IP est?? activa, e intenta averiguar el sistema operativo del servidor correspondiente:
```shell
nmap -O {{ip_o_hostname}}
```
#### Intenta determinar si los hosts est??n activos y cu??les son sus nombres:
```shell
nmap -sn {{ip_o_hostname}} {{opcional_otra_direccion}}
```
#### Como el anterior, pero tambi??n ejecuta un escaneo de 1000 puertos TCP por defecto, si el host est?? activo:
```shell
nmap {{ip_o_hostname}} {{opcional_otra_direccion}}
```
#### Detecta tambi??n scripts, servicios, sistema operativo y traceroute:
```shell
nmap -A {{direccion_o_direcciones}}
```
#### Asume una buena conexi??n y acelera la ejecuci??n:
```shell
nmap -T4 {{direccion_o_direcciones}}
```
#### Escanea una lista espec??fica de puertos (para todos los puertos `1-65535` usar `-p-`):
```shell
nmap -p {{puerto1,puerto2,???,puertoN}} {{direccion_o_direcciones}}
```
#### Realiza un escaneo TCP y UDP (usar `-sU` para solo UDP, `-sZ` para SCTP, `-sO` para IP):
```shell
nmap -sSU {{direccion_o_direcciones}}
```
#### Realiza un escaneo total de puertos, servicios, detecci??n de versiones con todos los scripts NSE por defecto contra un host para determinar debilidades e informaci??n:
```shell
nmap -sC -sV {{direccion_o_direcciones}}
```
{% endraw %}{% raw %}
<h2 id="nms">
  <a href="/es/common/nms.html">nms</a> <a href="#nms"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Herramienta de l??nea de comandos que recrea el famoso efecto de desencriptado de datos de la pel??cula Sneakers (1992).
> M??s informaci??n: <https://github.com/bartobri/no-more-secrets>.

#### Desencripta el texto tras presionar una tecla:
```shell
echo "{{Hola, Mundo!}}" | nms
```
#### Desencripta la salida inmediatamente, sin esperar a que una tecla sea pulsada:
```shell
{{ls -la}} | nms -a
```
#### Desencripta el contenido de un archivo, especificando el color de la salida:
```shell
cat {{ruta/al/archivo}} | nms -a -f {{blue|white|yellow|black|magenta|green|red}}
```
#### Limpia la pantalla antes de desencriptar:
```shell
{{comando}} | nms -a -c
```
{% endraw %}{% raw %}
<h2 id="rm">
  <a href="/es/common/rm.html">rm</a> <a href="#rm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Elimina archivos o directorios.
> M??s informaci??n: <https://www.gnu.org/software/coreutils/rm>.

#### Elimina archivos de ubicaciones arbitrarias:
```shell
rm {{ruta/al/archivo}} {{ruta/al/otro/archivo}}
```
#### Elimina, de forma recursiva, un directorio y todos sus subdirectorios:
```shell
rm -r {{ruta/al/directorio}}
```
#### Elimina un directorio a la fuerza, sin pedir confirmaci??n ni mostrar mensajes de error:
```shell
rm -rf {{ruta/al/directorio}}
```
#### Elimina varios archivos de forma interactiva, solicitando confirmaci??n antes de eliminar cada archivo:
```shell
rm -i {{archivo(s)}}
```
#### Elimina archivos en modo detallado, imprimiendo un mensaje por cada archivo eliminado:
```shell
rm -v {{ruta/hacia/directorio/*}}
```
{% endraw %}{% raw %}
<h2 id="tar">
  <a href="/es/common/tar.html">tar</a> <a href="#tar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Herramienta para archivos.
> A veces combinada con un m??todo de compresi??n, como gzip o bzip2.
> M??s informaci??n: <https://www.gnu.org/software/tar>.

#### Crear un archivo a partir de otros archivos:
```shell
tar cf {{archivo_destino.tar}} {{archivo1}} {{archivo2}} {{archivo3}}
```
#### Crear un archivo comprimido con gzip:
```shell
tar czf {{archivo_destino.tar.gz}} {{archivo1}} {{archivo2}} {{archivo3}}
```
#### Extraer un archivo (comprimido) en el directorio actual:
```shell
tar xf {{archivo.tar[.gz|.bz2|.xz]}}
```
#### Extraer un archivo en un directorio:
```shell
tar xf {{archivo.tar}} -C {{directorio}}
```
#### Crear un archivo comprimido usando el sufijo para determinar el programa de compresi??n:
```shell
tar caf {{archivo_destino.tar.xz}} {{archivo1}} {{archivo2}} {{archivo3}}
```
#### Mostrar el contenido de un archivo tar:
```shell
tar tvf {{archivo.tar}}
```
#### Extraer archivos que coinciden con un patr??n:
```shell
tar xf {{archivo.tar}} --wildcards "{{*.html}}"
```
{% endraw %}{% raw %}
<h2 id="tee">
  <a href="/es/common/tee.html">tee</a> <a href="#tee"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lee desde la entrada est??ndar y escribe a la salida est??ndar a la vez que a archivos o comandos.
> M??s informaci??n: <https://www.gnu.org/software/coreutils/tee>

#### Copia la entrada est??ndar al archivo, reemplazando su contenido, y tambi??n a la salida est??ndar:
```shell
echo {{ejemplo}} | tee {{ruta/al/archivo}}
```
#### Anexa la entrada est??ndar al archivo, sin reemplazar:
```shell
echo {{ejemplo}} | tee -a {{ruta/al/archivo}}
```
#### Imprime la entrada est??ndar a la terminal, y tambi??n lo reenv??a a otro programa para posterior procesamiento:
```shell
echo {{ejemplo}} | tee {{/dev/tty}} | {{xargs printf "[%s]"}}
```
{% endraw %}{% raw %}
<h2 id="tmux">
  <a href="/es/common/tmux.html">tmux</a> <a href="#tmux"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Multiplexa varias consolas virtuales.
> M??s informaci??n: <https://github.com/tmux/tmux>.

#### Inicia una nueva sesi??n de tmux:
```shell
tmux
```
#### Inicia una nueva sesi??n de tmux y le asigna un nombre:
```shell
tmux new -s {{nombre}}
```
#### Muestra las sesiones:
```shell
tmux ls
```
#### Adjunta a una sesi??n:
```shell
tmux a
```
#### Adjunta a una sesi??n con un nombre espec??fico:
```shell
tmux a -t {{nombre}}
```
#### Desconecta de la sesi??n:
```shell
Ctrl + B, D
```
#### Elimina una sesi??n con un nombre espec??fico:
```shell
tmux kill-session -t {{nombre}}
```
#### Elimina una sesi??n cuando se adjunta:
```shell
Ctrl + B, x (luego se pulsa 'y' para confirmar que s??)
```
{% endraw %}{% raw %}
<h2 id="touch">
  <a href="/es/common/touch.html">touch</a> <a href="#touch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cambia el tiempo de accesso y modificaci??n de un archivo (atime, mtime).
> M??s informaci??n: <https://www.gnu.org/software/coreutils/touch>.

#### Crea un archivo nuevo o cambia los tiempos de archivos existentes al tiempo actual:
```shell
touch {{archivo}}
```
#### Establece los tiempos de un archivo a un dia y hora espec??ficos:
```shell
touch -t {{YYYYMMDDHHMM.SS}} {{archivo}}
```
#### Usa los tiempos de un archivo para establecer los tiempos en otro archivo:
```shell
touch -r {{archivo}} {{archivo2}}
```
{% endraw %}{% raw %}
<h2 id="unrar">
  <a href="/es/common/unrar.html">unrar</a> <a href="#unrar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Extrae archivos RAR.

#### Extrae archivos comprimidos respetando la estructura original del archivo:
```shell
unrar x {{archivo_comprimido.rar}}
```
#### Extrae archivos comprimidos en una ruta determinada respetando la estructura original del archivo:
```shell
unrar x {{archivo_comprimido.rar}} {{ruta/donde/extraer}}
```
#### Extrae archivos comprimidos en el directorio actual, perdiendo la estructura original del archivo:
```shell
unrar e {{archivo_comprimido.rar}}
```
#### Comprueba la integridad de cada uno de los archivos dentro del archivo comprimido:
```shell
unrar t {{archivo_comprimido.rar}}
```
#### Muestra el listado de los archivos dentro del archivo comprimido sin descomprimirlo:
```shell
unrar l {{archivo_comprimido.rar}}
```
{% endraw %}{% raw %}
<h2 id="wc">
  <a href="/es/common/wc.html">wc</a> <a href="#wc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cuenta l??neas, palabras, o bytes.
> M??s informaci??n: <https://www.gnu.org/software/coreutils/wc>

#### Cuenta las l??neas en un archivo:
```shell
wc -l {{ruta/al/archivo}}
```
#### Cuenta las palabras en un archivo:
```shell
wc -w {{ruta/al/archivo}}
```
#### Cuenta caracteres (bytes) en un archivo:
```shell
wc -c {{ruta/al/archivo}}
```
#### Cuenta caracteres en un archivo (considerando los caracteres de varios bytes):
```shell
wc -m {{ruta/al/archivo}}
```
#### Usa la entrada estandar para contar l??neas, palabras o caracteres (bytes), en ese orden:
```shell
{{find .}} | wc
```
{% endraw %}{% raw %}
<h2 id="xkill">
  <a href="/es/common/xkill.html">xkill</a> <a href="#xkill"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cierra de manera forzosa una ventana interactivamente en una sesi??n gr??fica.
> V??ase tambi??n `kill` y `killall`.

#### Muestra un cursor para cerrar forzosamente una ventana presionando con el bot??n izquierdo (presiona cualquier otro bot??n del rat??n para cancelar):
```shell
xkill
```
{% endraw %}{% raw %}
<h2 id="yes">
  <a href="/es/common/yes.html">yes</a> <a href="#yes"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Retorna algo repetidamente.
> Este comando es frecuentemente utilizado para aceptar todas las confirmaciones en comandos de instalaci??n (como apt-get).
> M??s informaci??n: <https://www.gnu.org/software/coreutils/yes>.

#### Retornar repetidamente "mensaje":
```shell
yes {{mensaje}}
```
#### Retornar repetidamente "y":
```shell
yes
```
#### Aceptar todas las confirmaciones que muestre el comando `apt-get`:
```shell
yes | sudo apt-get install {{programa}}
```
{% endraw %}