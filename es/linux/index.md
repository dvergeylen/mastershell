---
layout: default
title: "linux"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
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

{% raw %}
<h2 id="apt-add-repository">
  <a href="/es/linux/apt-add-repository.html">apt-add-repository</a> <a href="#apt-add-repository"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gestiona las definiciones del repositorio apt.
> Más información: <https://manpages.debian.org/latest/software-properties-common/apt-add-repository.1.html>.

#### Añade un nuevo repositorio apt:
```shell
apt-add-repository {{repositorio}}
```
#### Elimina un repositorio apt:
```shell
apt-add-repository --remove {{repositorio}}
```
#### Actualiza la caché de paquetes tras añadir un repositorio:
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
> Más información: <https://manpages.debian.org/latest/apt/apt-cache.8.html>.

#### Busca un paquete en tus fuentes actuales:
```shell
apt-cache search {{consulta}}
```
#### Muestra información de un paquete:
```shell
apt-cache show {{paquete}}
```
#### Muestra si un paquete está instalado y actualizado:
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
> Busca archivos en paquetes apt, incluyendo los que aún no fueron instalados.
> Más información: <https://manpages.debian.org/latest/apt-file/apt-file.1.html>.

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
> Herramienta de gestión de paquete para distribuciones basadas en Debian.
> Buscar paquetes utilizando `apt-cache`.
> Más información: <https://manpages.debian.org/latest/apt/apt-get.8.html>.

#### Actualiza la lista de paquetes y versiones disponibles (se recomienda ejecutar este comando antes que cualquier otro comando `apt-get`):
```shell
apt-get update
```
#### Instala un paquete o actualizarlo a su última versión disponible:
```shell
apt-get install {{paquete}}
```
#### Elimina un paquete:
```shell
apt-get remove {{paquete}}
```
#### Elimina un paquete y sus archivos de configuración:
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
> Herramienta para la gestión de claves para el Gestor de Paquetes APT (APT Package Manager) en Debian y Ubuntu.
> Más información: <https://manpages.debian.org/latest/apt/apt-key.8.html>.

#### Muestra las claves de confianza:
```shell
apt-key list
```
#### Añade una clave al almacén de claves de confianza):
```shell
apt-key add {{archivo_clave_pública.asc}}
```
#### Borrar una clave del almacén de claves de confianza:
```shell
apt-key del {{id_clave}}
```
#### Añadir un clave remota al almacén de claves de confianza:
```shell
wget -qO - {{https://host.tld/archivo.clave}} | apt-key add -
```
#### Añadir una clave de un servidor de claves con el identificador de la clave:
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
> Más información: <https://manpages.debian.org/latest/apt/apt-mark.8.html>.

#### Marca un paquete como instalado automáticamente:
```shell
sudo apt-mark auto {{nombre_paquete}}
```
#### Mantiene un paquete en su versión actual y evita que se actualice:
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
> Herramienta de gestión de paquete para distribuciones basadas en Debian.
> Se recomienda sustituirlo por apt-get cuando se use interactivamente en Ubuntu 16.04 o versiones posteriores.
> Más información: <https://manpages.debian.org/latest/apt/apt.8.html>.

#### Actualiza la lista de paquetes y versiones disponibles (se recomienda ejecutar este comando antes que cualquier otro comando `apt`):
```shell
sudo apt update
```
#### Busca un paquete:
```shell
apt search {{paquete}}
```
#### Muestra la información de un paquete:
```shell
apt show {{paquete}}
```
#### Instala un paquete o lo actualiza a su última versión disponible:
```shell
sudo apt install {{paquete}}
```
#### Elimina un paquete (si se utiliza `purge` también elimina sus archivos de configuración):
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
> Herramienta de gestión de paquetes para Debian y Ubuntu.
> Más información: <https://manpages.debian.org/latest/aptitude/aptitude.8.html>.

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
#### Buscar un paquete instalado (`?installed` es un término de búsqueda de `aptitude`):
```shell
aptitude search '?installed({{paquete}})'
```
#### Elimina un paquete y todos los paquetes que dependen de él:
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
#### Mantiente un paquete instalado para que no sea actualizado automáticamente:
```shell
aptitude hold '?installed({{paquete}})'
```
{% endraw %}{% raw %}
<h2 id="archey">
  <a href="/es/linux/archey.html">archey</a> <a href="#archey"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Herramienta sencilla para mostrar información del sistema con estilo.

#### Muestra información del sistema:
```shell
archey
```
{% endraw %}{% raw %}
<h2 id="bpytop">
  <a href="/es/linux/bpytop.html">bpytop</a> <a href="#bpytop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra información en tiempo real sobre procesos ejecutándose, con gráficos. Similar a `gtop` y `htop`.
> Más información: <https://github.com/aristocratos/bpytop>.

#### Inicia bpytop:
```shell
bpytop
```
#### Inicia en modo mínimalista sin recuadros de memoria y redes:
```shell
bpytop -m
```
#### Muestra la versión:
```shell
bpytop -v
```
#### Cambia a modo minimalista:
```shell
m
```
#### Busca procesos o programas ejecutándose:
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

#### Busca fórmulas disponibles:
```shell
brew search {{texto}}
```
#### Instala la última versión de una fórmula (usar `--devel` para la versión de desarrollo):
```shell
brew install {{formula}}
```
#### Lista todas las fórmulas instaladas:
```shell
brew list
```
#### Actualizar una fórmula instalada (si no se indica ninguna, todas las fórmulas son actualizadas):
```shell
brew upgrade {{formula}}
```
#### Actualiza a la última versión de Linuxbrew y de todas las fórmulas desde GitHub:
```shell
brew update
```
#### Mostrar las fórmulas que tienen una versión más reciente disponible:
```shell
brew outdated
```
#### Mostrar la información de una fórmula (versión, ruta de instalación, dependencias, etc.):
```shell
brew info {{fórmula}}
```
#### Revisar la instalación local de Linuxbrew en busca de problemas potenciales:
```shell
brew doctor
```
{% endraw %}{% raw %}
<h2 id="cal">
  <a href="/es/linux/cal.html">cal</a> <a href="#cal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra el calendario, con el día actual resaltado.

#### Muestra el calendario para el mes actual:
```shell
cal
```
#### Muestra el mes anterior, actual y próximo:
```shell
cal -3
```
#### Usa el Lunes como primer día de la semana:
```shell
cal --monday
```
#### Muestra el calendario para un año concreto (4 dígitos):
```shell
cal {{year}}
```
#### Muestra el calendario para un año y mes concretos:
```shell
cal {{month}} {{year}}
```
{% endraw %}{% raw %}
<h2 id="calc">
  <a href="/es/linux/calc.html">calc</a> <a href="#calc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Una calculadora de precisión arbitraria en la terminal.

#### Iniciar calc en modo interactivo:
```shell
calc
```
#### Realizar un cálculo en modo no-interactivo:
```shell
calc -p '{{85 * (36 / 4)}}'
```
{% endraw %}{% raw %}
<h2 id="clamav">
  <a href="/es/linux/clamav.html">clamav</a> <a href="#clamav"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Antivirus de código abierto.
> Diseñado especialment para escanear correos electrónicos, pero puede ser usado en otros contextos.
> Más información: <https://www.clamav.net>.

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
> Reproductor de música para la línea de comandos.
> Usa las teclas de dirección para navegar, `<enter/return>` para seleccionar, y los números 1-8 para cambiar entra las diferentes vistas.

#### Abre cmus en un directorio concreto:
```shell
cmus {{ruta/al/directorio}}
```
#### Añade un archivo/directorio a la librería:
```shell
:add {{ruta/al/archivo_o_directorio}}
```
#### Pausa/reproduce la canción actual:
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
> Más información: <https://github.com/brndnmtthws/conky>.

#### Ejecuta con la configuración por defecto:
```shell
conky
```
#### Crea una nueva configuración por defecto:
```shell
conky -C > ~/.conkyrc
```
#### Ejecuta conky con un archivo de configuración concreto:
```shell
conky -c {{ruta/a/la/configuración}}
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
> Escribe los mensajes del núcleo a la salida estándar.

#### Muestra los mensajes del núcleo:
```shell
dmesg
```
#### Muestra los mensajes de error del núcleo:
```shell
dmesg --level err
```
#### Muestra los mensajes del núcleo y sigue leyedos los nuevos, similar a `tail -f` (disponible en los núcleos 3.5.0 y posteriores):
```shell
dmesg -w
```
#### Muestra cuanta memoria física hay disponible en este sistema:
```shell
dmesg | grep -i memory
```
#### Muestra los mensajes del núcleo, página a página:
```shell
dmesg | less
```
#### Muestra los mensajes del núcleo con una estampilla temporal (disponible en los núcleos 3.5.0 y posteriores):
```shell
dmesg -T
```
#### Muestra los mensajes del núcleo de forma legible para humanos (disponible en los núcleos 3.5.0 y posteriores):
```shell
dmesg -H
```
#### Colorea la salida (disponible en los núcleos 3.5.0 y posteriores):
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
> Más información: <https://dnf.readthedocs.io>.

#### Actualiza todos los paquetes a la última versión disponible:
```shell
sudo dnf update
```
#### Busca un paquete usando palabras clave:
```shell
dnf search {{palabra_clave}}
```
#### Muestra información acerca de un paquete:
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
> Cambia saltos de línea con formato DOS a saltos de línea con formato Unix.
> Reemplaza CRLF con CR.

#### Cambia los saltos de línea de un archivo:
```shell
dos2unix {{nombre_de_archivo}}
```
#### Crea una copia con saltos de línea en formato Unix:
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
> Más información: <https://manned.org/groupdel>.

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
> Detiene, apaga o reinicia la máquina.

#### Detiene la máquina:
```shell
halt
```
#### Apaga la máquina:
```shell
halt --poweroff
```
#### Reinicia la máquina:
```shell
halt --reboot
```
{% endraw %}{% raw %}
<h2 id="line">
  <a href="/es/linux/line.html">line</a> <a href="#line"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lee una única línea de entrada.

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
> Proporciona información específica de la distribución y LSB (Linux Standard Base).

#### Muestra toda la información disponible:
```shell
lsb_release -a
```
#### Muestra una descripción del sistema operativo (normalmente el nombre completo):
```shell
lsb_release -d
```
#### Muestra solo el nombre del sistema operativo (ID) sin el campo nombre:
```shell
lsb_release -i -s
```
#### Muestra el número de versión y el nombre en clave de la distribución sin el campo de nombre:
```shell
lsb_release -rcs
```
{% endraw %}{% raw %}
<h2 id="lsmod">
  <a href="/es/linux/lsmod.html">lsmod</a> <a href="#lsmod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra el estado de los módulos cargados en el kernel de linux.
> Vease tambien `modprobe`, el cual carga módulos de kernel.

#### Lista todos los módulos de kernel cargados:
```shell
lsmod
```
{% endraw %}{% raw %}
<h2 id="lsusb">
  <a href="/es/linux/lsusb.html">lsusb</a> <a href="#lsusb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra información sobre puertos y dispositivos USB.

#### Lista todos los dispositivos USB disponibles:
```shell
lsusb
```
#### Lista la jerarquía de dispositivos USB en forma de árbol:
```shell
lsusb -t
```
#### Lista los dispositivos USB de forma verbosa:
```shell
lsusb --verbose
```
#### Lista información detallada acerca de un dispositivo USB determinado:
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
> Arregla problemas habituales de una partición NTFS.

#### Arregla una partición NTFS dada:
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
> Apaga la máquina.

#### Apaga la máquina:
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
> Reinicia la máquina.

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
> Utilidad para generar un nombre, apellido, calle y número, junto a ubicación geográfica consistente (un conjunto válido de ciudad, estado y código postal).
> Más información: <https://manpages.ubuntu.com/manpages/focal/man6/rig.6.html>.

#### Muestra un nombre aleatorio (masculino o femenino) y una dirección:
```shell
rig
```
#### Muestra un nombre [m]asculino, (o [f]emenino) aleatorio y una dirección:
```shell
rig -{{m|f}}
```
#### Usa archivos de datos de un directorio específico (por defecto es `/usr/share/rig`):
```shell
rig -d {{ruta/al/directorio}}
```
#### Especifica el número de identidades a generar:
```shell
rig -c {{numero}}
```
#### Especifica el número de identidades femininas a generar:
```shell
rig -f -c {{numero}}
```
{% endraw %}{% raw %}
<h2 id="shutdown">
  <a href="/es/linux/shutdown.html">shutdown</a> <a href="#shutdown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Detiene, apaga o reinicia la máquina.

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
#### Cancela una operación de apagado/reinicio pendiente:
```shell
shutdown -c
```
{% endraw %}{% raw %}
<h2 id="top">
  <a href="/es/linux/top.html">top</a> <a href="#top"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Muestra información dinámica en tiempo real sobre procesos ejecutándose.

#### Inicia top:
```shell
top
```
#### No muestra ningún proceso inactivo o zombie:
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
> Más información: <https://manned.org/userdel>.

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
> Abre un archivo o URL en la aplicación predeterminada del usuario.
> Más información: <https://man.archlinux.org/man/xdg-open.1>.

#### Abre el directorio actual en el explorador de archivos predeterminado:
```shell
xdg-open .
```
#### Abre una URL en el navegador predeterminado:
```shell
xdg-open {{https://www.ejemplo.es}}
```
#### Abre una image en el visor de imágenes predeterminado:
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
{% endraw %}