---
layout: default
title: "osx"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
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

{% raw %}
<h2 id="afinfo">
  <a href="/es/osx/afinfo.html">afinfo</a> <a href="#afinfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Analizador de metadatos de archivos de audio para OS X.
> Comando nativo de OS X.

#### Muestra información de un archivo de audio dado:
```shell
afinfo {{ruta/al/archivo}}
```
#### Muestra una descripción de una línea del archivo de audio:
```shell
afinfo -b {{ruta/al/archivo}}
```
#### Muestra información de metadatos y contenido del InfoDictionary del archivo de audio:
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
> Reproductor de audio de línea de comandos.

#### Reproduce un archivo de audio (espera hasta que finalice la reproducción):
```shell
afplay {{ruta/al/archivo}}
```
#### Reproduce un archivo de audio a una velocidad 2x (velocidad de reproducción):
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
> Utilidad de configuración de red inalámbrica.

#### Muestra la información del estado actual de la red inalámbrica:
```shell
airport -I
```
#### Detecta tráfico inalámbrico en el canal 1:
```shell
airport sniff {{1}}
```
#### Busca redes inalámbricas disponibles:
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
> Herramienta sencilla para mostrar información del sistema con estilo.

#### Muestra información del sistema:
```shell
archey
```
#### Muestra información del sistema sin colorear la salida:
```shell
archey --nocolor
```
#### Muestra información del sistema, usando MacPorts en lugar de Hombrew:
```shell
archey --macports
```
#### Muestra información del sistema sin verificación dirección IP:
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
#### Genera resultados más rápido omitiendo los espacios en blanco y el preprocesamiento de comentarios. (Solo debe usarse para compiladores de confianza):
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
> El nombre del comando significa Restauración de Software de Apple.

#### Restaura una imagen de disco en un volumen:
```shell
sudo asr restore --source {{nombre_de_imagen}}.dmg --target {{ruta/al/volumen}}
```
#### Borra el volumen deseado antes de restaurar:
```shell
sudo asr restore --source {{nombre_de_imagen}}.dmg --target {{ruta/al/volumen}} --erase
```
#### Omite la verificación después de restaurar:
```shell
sudo asr restore --source {{nombre_de_imagen}}.dmg --target {{ruta/al/volumen}} --noverify
```
#### Clona volúmenes sin el uso de una imagen de disco intermedia:
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
> Más información: <https://brew.sh>.

#### Busca fórmulas y paquetes disponibles:
```shell
brew search {{text}}
```
#### Instala la última versión estable de una fórmula (usa `--devel` para versiones de desarrollo):
```shell
brew install {{formula}}
```
#### Muestra todas las fórmulas instaladas:
```shell
brew list
```
#### Muestra fórmulas instaladas que no dependen de otras:
```shell
brew leaves
```
#### Actualiza una fórmula instalada (si no se indica el nombre, se actualizan todas las fórmulas):
```shell
brew upgrade {{formula}}
```
#### Actualiza a la última versión de Homebrew y todas sus fórmulas desde GitHub:
```shell
brew update
```
#### Muestra información acerca de una fórmula (versión, ruta de instalación, dependencias, etc.):
```shell
brew info {{formula}}
```
#### Verifica la instalación local de Homebrew en busca de problemas potenciales:
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
#### Verifica uno o más archivos o directorios determinados:
```shell
rubocop {{path/to/file}} {{path/to/directory}}
```
#### Guarda la salida en un archivo:
```shell
rubocop --out {{path/to/file}}
```
#### Muestra la lista de cops (reglas de análisis):
```shell
rubocop --show-cops
```
#### Excluye una regla:
```shell
rubocop --except {{cop_1}} {{cop_2}}
```
#### Ejecuta sólo determinadas reglas:
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
> Una línea de comando para Spotify.
> Más información: <https://github.com/hnarayanan/shpotify>.

#### Encuentra una canción por su nombre y la reproduce:
```shell
spotify play {{song_name}}
```
#### Encuentra una lista de reproducción por su nombre y la reproduce:
```shell
spotify play list {{playlist_name}}
```
#### Pausa (o reanuda) la reproducción:
```shell
spotify pause
```
#### Pasa a la siguiente canción de una lista de reproducción:
```shell
spotify next
```
#### Cambia el volumen:
```shell
spotify vol {{up|down|value}}
```
#### Muestra el estado de reproducción y los detalles de la canción:
```shell
spotify status
```
{% endraw %}