---
layout: default
title: "linux"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#a2disconf">a2disconf</a>
* <a href="#a2dismod">a2dismod</a>
* <a href="#a2dissite">a2dissite</a>
* <a href="#a2enconf">a2enconf</a>
* <a href="#a2enmod">a2enmod</a>
* <a href="#a2ensite">a2ensite</a>
* <a href="#a2query">a2query</a>
* <a href="#apache2ctl">apache2ctl</a>
* <a href="#apt">apt</a>
* <a href="#apt-add-repository">apt-add-repository</a>
* <a href="#apt-cache">apt-cache</a>
* <a href="#apt-file">apt-file</a>
* <a href="#apt-get">apt-get</a>
* <a href="#apt-mark">apt-mark</a>
* <a href="#flameshot">flameshot</a>
* <a href="#ifdown">ifdown</a>
* <a href="#ifup">ifup</a>
* <a href="#ip">ip</a>
* <a href="#ip-address">ip address</a>
* <a href="#iwctl">iwctl</a>
* <a href="#pacman">pacman</a>
* <a href="#useradd">useradd</a>
* <a href="#userdel">userdel</a>
* <a href="#usermod">usermod</a>
* <a href="#xbacklight">xbacklight</a>
* <a href="#xclip">xclip</a>
* <a href="#yay">yay</a>

{% raw %}
<h2 id="a2disconf">
  <a href="/fr/linux/a2disconf.html">a2disconf</a> <a href="#a2disconf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Désactive un fichier de configuration sur une distribution Debian.
> Plus d'informations : <https://manpages.debian.org/latest/apache2/a2disconf.8.en.html>.

#### Désactive un fichier de configuration :
```shell
sudo a2disconf {{fichier_de_configuration}}
```
#### N'affiche aucun message (mode silencieux) :
```shell
sudo a2disconf --quiet {{fichier_de_configuration}}
```
{% endraw %}{% raw %}
<h2 id="a2dismod">
  <a href="/fr/linux/a2dismod.html">a2dismod</a> <a href="#a2dismod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Désactive un module Apache sur une distribution Debian.
> Plus d'informations : <https://manpages.debian.org/latest/apache2/a2dismod.8.en.html>.

#### Désactive un module :
```shell
sudo a2dismod {{module}}
```
#### N'affiche aucun message (mode silencieux) :
```shell
sudo a2dismod --quiet {{module}}
```
{% endraw %}{% raw %}
<h2 id="a2dissite">
  <a href="/fr/linux/a2dissite.html">a2dissite</a> <a href="#a2dissite"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Désactive un hôte virtuel Apache sur une distribution Debian.
> Plus d'informations : <https://manpages.debian.org/latest/apache2/a2dissite.8.en.html>.

#### Désactive un hôte virtuel :
```shell
sudo a2dissite {{virtual_host}}
```
#### N'affiche aucun message (mode silencieux) :
```shell
sudo a2dissite --quiet {{virtual_host}}
```
{% endraw %}{% raw %}
<h2 id="a2enconf">
  <a href="/fr/linux/a2enconf.html">a2enconf</a> <a href="#a2enconf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Active un fichier de configuration sur une distribution Debian.
> Plus d'information : <https://manpages.debian.org/latest/apache2/a2enconf.8.en.html>.

#### Active un fichier de configuration :
```shell
sudo a2enconf {{fichier_de_configuration}}
```
#### N'affiche aucun message (mode silencieux) :
```shell
sudo a2enconf --quiet {{fichier_de_configuration}}
```
{% endraw %}{% raw %}
<h2 id="a2enmod">
  <a href="/fr/linux/a2enmod.html">a2enmod</a> <a href="#a2enmod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Active un module Apache sur une distribution Debian.
> Plus d'information : <https://manpages.debian.org/latest/apache2/a2enmod.8.en.html>.

#### Active un module :
```shell
sudo a2enmod {{module}}
```
#### N'affiche aucun message (mode silencieux) :
```shell
sudo a2enmod --quiet {{module}}
```
{% endraw %}{% raw %}
<h2 id="a2ensite">
  <a href="/fr/linux/a2ensite.html">a2ensite</a> <a href="#a2ensite"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Active un hôte virtuel Apache sur des systèmes d'exploitation (SE) basés sur Debian.
> Plus d'informations : <https://manpages.debian.org/latest/apache2/a2ensite.8.en.html>.

#### Active un hôte virtuel :
```shell
sudo a2ensite {{hote_virtuel}}
```
#### N'affiche aucun message (mode silencieux) :
```shell
sudo a2ensite --quiet {{hote_virtuel}}
```
{% endraw %}{% raw %}
<h2 id="a2query">
  <a href="/fr/linux/a2query.html">a2query</a> <a href="#a2query"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Retourne la configuration d'exécution d'Apache sur une distribution Debian.
> Plus d'informations : <https://manpages.debian.org/latest/apache2/a2query.1.en.html>.

#### Liste les [m]odules Apache actifs :
```shell
sudo a2query -m
```
#### Vérifie si un module spécifique est installé :
```shell
sudo a2query -m {{nom_module}}
```
#### Liste les hôtes virtuels actifs :
```shell
sudo a2query -s
```
#### Affiche le [M]odule de traitement multiple actif :
```shell
sudo a2query -M
```
#### Affiche la [v]ersion d'Apache :
```shell
sudo a2query -v
```
{% endraw %}{% raw %}
<h2 id="apache2ctl">
  <a href="/fr/linux/apache2ctl.html">apache2ctl</a> <a href="#apache2ctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> L'outil d'Interface en Lignes de Commandes (ILC) pour administrer le serveur web HTTP Apache.
> Cette commande est disponible sur une distribution Debian. Pour les distributions basées Red Hat, voir `httpd`.
> Plus d'informations : <https://manpages.debian.org/latest/apache2/apache2ctl.8.en.html>.

#### Démarre le démon Apache. Envoie un message s'il est déjà actif :
```shell
sudo apache2ctl start
```
#### Arrête le démon Apache :
```shell
sudo apache2ctl stop
```
#### Re-démarre le démon Apache :
```shell
sudo apache2ctl restart
```
#### Teste la syntaxe du fichier de configuration :
```shell
sudo apache2ctl -t
```
#### Liste les modules chargés :
```shell
sudo apache2ctl -M
```
{% endraw %}{% raw %}
<h2 id="apt-add-repository">
  <a href="/fr/linux/apt-add-repository.html">apt-add-repository</a> <a href="#apt-add-repository"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gère la définition des dépôts apt.
> Plus d'informations : <https://manpages.debian.org/latest/software-properties-common/apt-add-repository.1.html>.

#### Ajout d'un nouveau dépôt :
```shell
apt-add-repository {{repository_spec}}
```
#### Suppression d'un dépôt :
```shell
apt-add-repository --remove {{repository_spec}}
```
#### Mise à jour du cache des paquets après ajout d'un dépôt :
```shell
apt-add-repository --update {{repository_spec}}
```
#### Activation pour les paquets source :
```shell
apt-add-repository --enable-source {{repository_spec}}
```
{% endraw %}{% raw %}
<h2 id="apt-cache">
  <a href="/fr/linux/apt-cache.html">apt-cache</a> <a href="#apt-cache"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Outil de recherche de paquets Debian et Ubuntu.
> Plus d'informations : <https://manpages.debian.org/latest/apt/apt-cache.8.html>.

#### Recherche un paquet dans vos sources actuelles :
```shell
apt-cache search {{query}}
```
#### Affiche des informations sur un paquet :
```shell
apt-cache show {{package}}
```
#### Indique si un paquet est installé et à jour :
```shell
apt-cache policy {{package}}
```
#### Affiche les dépendances d'un paquet :
```shell
apt-cache depends {{package}}
```
#### Affiche les paquets qui dépendent d'un paquet particulier :
```shell
apt-cache rdepends {{package}}
```
{% endraw %}{% raw %}
<h2 id="apt-file">
  <a href="/fr/linux/apt-file.html">apt-file</a> <a href="#apt-file"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Recherche de fichiers dans les paquets apt, y compris ceux qui ne sont pas encore installés.
> Plus d'informations : <https://manpages.debian.org/latest/apt-file/apt-file.1.html>.

#### Mise à jour la base de données des métadonnées :
```shell
sudo apt update
```
#### Recherche des paquets qui contiennent le fichier ou le chemin d'accès spécifié :
```shell
apt-file search {{part/of/filename}}
```
#### Énumère le contenu d'un paquet spécifique :
```shell
apt-file list {{package_name}}
```
{% endraw %}{% raw %}
<h2 id="apt-get">
  <a href="/fr/linux/apt-get.html">apt-get</a> <a href="#apt-get"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilitaire de gestion des paquets Debian et Ubuntu.
> Recherche des paquets en utilisant `apt-cache`.
> Plus d'informations : <https://manpages.debian.org/latest/apt/apt-get.8.html>.

#### Mise à jour de la liste des paquets et des versions disponibles (il est recommandé de l'exécuter avant les autres commandes `apt-get`) :
```shell
apt-get update
```
#### Installation d'un paquet, ou mise à jour avec la dernière version disponible :
```shell
apt-get install {{package}}
```
#### Suppression d'un paquet :
```shell
apt-get remove {{package}}
```
#### Suppression d'un paquet et de ses fichiers de configuration :
```shell
apt-get purge {{package}}
```
#### Mise à jour de tous les paquets installés vers les dernières versions disponibles :
```shell
apt-get upgrade
```
#### Nettoyage du dépôt local - supprime les fichiers de paquets (`.deb`) des téléchargements interrompus qui ne peuvent plus être téléchargés:
```shell
apt-get autoclean
```
#### Suppression de tous les paquets qui ne sont plus nécessaires :
```shell
apt-get autoremove
```
#### Mise à jour des paquets installés (comme la commande `upgrade`), mais avec suppression des paquets obsolètes et installation des paquets supplémentaires pour répondre aux nouvelles dépendances :
```shell
apt-get dist-upgrade
```
{% endraw %}{% raw %}
<h2 id="apt-mark">
  <a href="/fr/linux/apt-mark.html">apt-mark</a> <a href="#apt-mark"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilitaire permettant de modifier l'état des paquets installés.
> Plus d'informations : <https://manpages.debian.org/latest/apt/apt-mark.8.html>.

#### Marquer un paquet comme étant automatiquement installé :
```shell
sudo apt-mark auto {{package_name}}
```
#### Maintenir un paquet à sa version actuelle et empêcher les mises à jour :
```shell
sudo apt-mark hold {{package_name}}
```
#### Permettre une nouvelle mise à jour d'un paquet :
```shell
sudo apt-mark unhold {{package_name}}
```
#### Afficher les paquets installés manuellement :
```shell
apt-mark showmanual
```
#### Afficher les paquets détenus qui ne sont pas mis à jour :
```shell
apt-mark showhold
```
{% endraw %}{% raw %}
<h2 id="apt">
  <a href="/fr/linux/apt.html">apt</a> <a href="#apt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilitaire de gestion des paquets pour les distributions basées sur Debian.
> Remplacement recommandé pour apt-get lorsqu'il est utilisé de manière interactive dans les versions 16.04 et ultérieures d'Ubuntu.
> Plus d'informations : <https://manpages.debian.org/latest/apt/apt.8.html>.

#### Mettre à jour la liste des paquets et des versions disponibles (il est recommandé de l'exécuter avant les autres commandes `apt`) :
```shell
sudo apt update
```
#### Recherche d'un paquet donné :
```shell
apt search {{package}}
```
#### Afficher les informations pour un paquet :
```shell
apt show {{package}}
```
#### Installer un paquet, ou le mettre à jour avec la dernière version disponible :
```shell
sudo apt install {{package}}
```
#### Supprimer un paquet (utiliser `purge` à la place supprime également ses fichiers de configuration) :
```shell
sudo apt remove {{package}}
```
#### Mettre à jour tous les paquets installés vers les dernières versions disponibles :
```shell
sudo apt upgrade
```
#### Lister tous les paquets :
```shell
apt list
```
#### Lister les paquets installés :
```shell
apt list --installed
```
{% endraw %}{% raw %}
<h2 id="flameshot">
  <a href="/fr/linux/flameshot.html">flameshot</a> <a href="#flameshot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Outil de capture d'écran avec une interface graphique.
> Ajoute du texte, des formes, des couleurs et envoie à imgur.
> Plus d'informations : <https://flameshot.js.org>.

#### Lancez Flameshot en mode graphique :
```shell
flameshot launcher
```
#### Prenez une capture d'écran en cliquant et en faisant glisser :
```shell
flameshot gui
```
#### Prenez une capture d'écran en plein écran :
```shell
flameshot full
```
#### Définissez le chemin de sauvegarde :
```shell
flameshot full --path {{path/to/directory}}
```
#### Retardez la capture d'écran de N millisecondes et la sortie dans le presse-papiers :
```shell
flameshot full --delay {{2000}} --clipboard
```
{% endraw %}{% raw %}
<h2 id="ifdown">
  <a href="/fr/linux/ifdown.html">ifdown</a> <a href="#ifdown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Désactive des interfaces réseau.
> Plus d'informations : <https://manned.org/ifdown>.

#### Désactive l'interface eth0 :
```shell
ifdown {{eth0}}
```
#### Désactive toutes les interfaces déjà actives :
```shell
ifdown -a
```
{% endraw %}{% raw %}
<h2 id="ifup">
  <a href="/fr/linux/ifup.html">ifup</a> <a href="#ifup"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Outil utilisé pour activer des interfaces réseau.
> Plus d'informations : <https://manpages.debian.org/latest/ifupdown/ifup.8.html>.

#### Active l'interface eth0 :
```shell
ifup {{eth0}}
```
#### Active l'ensemble des interfaces réseau définies dans le fichier `/etc/network/interfaces` :
```shell
ifup -a
```
{% endraw %}{% raw %}
<h2 id="ip-address">
  <a href="/fr/linux/ip-address.html">ip address</a> <a href="#ip-address"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sous-commande de gestion des adresses IP.
> Plus d'informations : <https://www.man7.org/linux/man-pages/man8/ip-address.8.html>.

#### Liste les interfaces réseau et leurs adresses IP associées :
```shell
ip address
```
#### Filtre pour n'afficher que les interfaces réseau actives :
```shell
ip address show up
```
#### Affiche les informations relatives à une interface réseau spécifique :
```shell
ip address show dev {{eth0}}
```
#### Ajoute une adresse IP à une interface réseau :
```shell
ip address add {{ip_address}} dev {{eth0}}
```
#### Supprimer une adresse réseau d'une interface réseau :
```shell
ip address delete {{ip_address}} dev {{eth0}}
```
#### Supprime l'ensemble des adresses IP sur une portée donnée (scope) depuis une interface réseau :
```shell
ip address flush dev {{eth0}} scope {{global|host|link}}
```
{% endraw %}{% raw %}
<h2 id="ip">
  <a href="/fr/linux/ip.html">ip</a> <a href="#ip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Affiche / manipule l'adressage, le routage, les interfaces et périphériques réseau, les règles de routage et les tunnels.
> Plus d'informations : <https://www.man7.org/linux/man-pages/man8/ip.8.html>.

#### Liste les interfaces avec des infos détaillées :
```shell
ip address
```
#### Liste les interfaces sur la couche réseau de façon synthétique :
```shell
ip -brief address
```
#### Liste les interfaces sur la couche liaison de façon synthétique :
```shell
ip -brief link
```
#### Affiche la table de routage :
```shell
ip route
```
#### Affiche les voisins (table ARP) :
```shell
ip neighbour
```
#### Active/Désactive une interface :
```shell
ip link set {{interface}} up/down
```
#### Ajoute/Supprime une adresse ip à une interface :
```shell
ip addr add/del {{ip}}/{{mask}} dev {{interface}}
```
#### Ajoute une route par défaut :
```shell
ip route add default via {{ip}} dev {{interface}}
```
{% endraw %}{% raw %}
<h2 id="iwctl">
  <a href="/fr/linux/iwctl.html">iwctl</a> <a href="#iwctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Un outil de ligne de commande pour gérer iwd.
> Plus d'informations : <https://iwd.wiki.kernel.org/gettingstarted>.

#### Lancer le mode interactif, dans ce mode vous pouvez entrer les commandes directement, avec de l'auto-complétion :
```shell
iwctl
```
#### Avoir l'aide générale :
```shell
iwctl --help
```
#### Afficher vos stations wifi :
```shell
iwctl station list
```
#### Lancer la recherche de réseaux avec une station :
```shell
iwctl station {{station}} scan
```
#### Afficher les réseaux trouvés par une station :
```shell
iwctl station {{station}} get-networks
```
#### Se connecter à un réseau avec une station, si des informations de connexion sont nécessaires elles seront demandées :
```shell
iwctl station {{station}} connect {{nom_du_réseau}}
```
{% endraw %}{% raw %}
<h2 id="pacman">
  <a href="/fr/linux/pacman.html">pacman</a> <a href="#pacman"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Outil de gestion de paquets sur Arch Linux.
> Plus d'informations : <https://man.archlinux.org/man/pacman.8>.

#### Synchronise et mets à jour tous les paquets :
```shell
pacman -Syu
```
#### Installe un nouveau paquet :
```shell
pacman -S {{nom_paquet}}
```
#### Efface un paquet et ses dépendances :
```shell
pacman -Rs {{nom_paquet}}
```
#### Recherche dans la base de données des paquets une expression régulière ou mot clé :
```shell
pacman -Ss "{{terme_recherche}}"
```
#### Liste les paquets installés et leurs versions :
```shell
pacman -Q
```
#### Liste seulement les paquets installés explicitement et leurs versions :
```shell
pacman -Qe
```
#### Trouve à quel paquet un certain fichier appartient :
```shell
pacman -Qo {{fichier}}
```
#### Vide le cache des paquets pour libérer de l'espace :
```shell
pacman -Scc
```
{% endraw %}{% raw %}
<h2 id="useradd">
  <a href="/fr/linux/useradd.html">useradd</a> <a href="#useradd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Crée un nouvel utilisateur.
> Plus d'informations : <https://manned.org/useradd>.

#### Crée un nouvel utilisateur :
```shell
useradd {{nom}}
```
#### Crée un nouvel utilisateur avec un dossier home par défaut :
```shell
useradd --create-home {{nom}}
```
#### Crée un nouvel utilisateur avec le shell spécifié :
```shell
useradd --shell {{/chemin/vers/shell}} {{nom}}
```
#### Crée un nouvel utilisateur qui appartient aux groupes supplémentaires (attention à l'omission des espaces) :
```shell
useradd --groups {{groupe1,groupe2}} {{nom}}
```
#### Crée un nouvel utilisateur sans un dossier home :
```shell
useradd --no-create-home --system {{nom}}
```
{% endraw %}{% raw %}
<h2 id="userdel">
  <a href="/fr/linux/userdel.html">userdel</a> <a href="#userdel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Efface un utilisateur.
> Plus d'informations : <https://manned.org/userdel>.

#### Efface un utilisateur et son dossier home :
```shell
userdel -r {{nom}}
```
{% endraw %}{% raw %}
<h2 id="usermod">
  <a href="/fr/linux/usermod.html">usermod</a> <a href="#usermod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Modifie un compte utilisateur.
> Plus d'informations : <https://manned.org/usermod>.

#### Change le nom d'un utilisateur :
```shell
usermod -l {{nouveau_nom}} {{utilisateur}}
```
#### Ajoute l'utilisateur à des groupes supplémentaires (attention à l'omission d'espaces) :
```shell
usermod -a -G {{groupe1,groupe2}} {{utilisateur}}
```
#### Crée un nouveau dossier home pour un utilisateur et déplace ses fichiers vers celui-ci :
```shell
usermod -m -d {{/chemin/vers/home}} {{utilisateur}}
```
{% endraw %}{% raw %}
<h2 id="xbacklight">
  <a href="/fr/linux/xbacklight.html">xbacklight</a> <a href="#xbacklight"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Outil pour ajuster la luminosité du rétroéclairage en utilisant l'extension RandR.
> Plus d'informations : <https://gitlab.freedesktop.org/xorg/app/xbacklight>.

#### Obtient le niveau de luminosité de l'écran actuel comme un pourcentage :
```shell
xbacklight
```
#### Régle la luminosité de l'écran à 40% :
```shell
xbacklight -set {{40}}
```
#### Augmente la luminosité de l'écran actuel de 25% :
```shell
xbacklight -inc {{25}}
```
#### Diminue la luminosité de l'écran actuel de 75% :
```shell
xbacklight -dec {{75}}
```
#### Augment la luminosité de l'écran à 100%, étendu sur 60 secondes (valeur donnée en ms), en 60 pas :
```shell
xbacklight -set {{100}} -time {{60000}} -steps {{60}}
```
{% endraw %}{% raw %}
<h2 id="xclip">
  <a href="/fr/linux/xclip.html">xclip</a> <a href="#xclip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Outil de manipulation de presse-papiers X11, semblable à `xsel`.
> Gère les sélections primaires et secondaires de X, en plus du presse-papier système (`Ctrl + C`/`Ctrl + V`).

#### Copie la sortie d'une commande vers la zone de sélection primaire de X11 (presse-papiers) :
```shell
echo 123 | xclip
```
#### Copie la sortie d'une commande vers une zone de sélection de X11 donnée :
```shell
echo 123 | xclip -selection {{primary|secondary|clipboard}}
```
#### Copie le contenu d'un fichier vers le presse-papiers système, avec la notation courte :
```shell
echo 123 | xclip -sel clip
```
#### Copie le contenu d'un fichier vers le presse-papiers système :
```shell
xclip -sel clip {{fichier_entrée.txt}}
```
#### Copie le contenu d'une image PNG vers le presse-papiers système (peut être collé dans d'autres programmes correctement) :
```shell
xclip -sel clip -t image/png {{fichier_entrée.png}}
```
#### Colle le contenu de la zone de sélection de X11 à la console :
```shell
xclip -o
```
#### Colle le contenu du presse-papier système à la console :
```shell
xclip -o -sel clip
```
#### Colle le contenu du presse-papier système à un fichier :
```shell
xclip -o -sel clip > {{fichier_sortie.txt}}
```
{% endraw %}{% raw %}
<h2 id="yay">
  <a href="/fr/linux/yay.html">yay</a> <a href="#yay"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Yet Another Yogurt : Un outil pour Arch Linux pour construire et installer des paquets depuis le Arch User Repository.
> À regarder : `pacman`.
> Plus d'informations : <https://github.com/Jguer/yay>.

#### Recherche interactivement et installe des paquets depuis les dépôts et l'AUR :
```shell
yay {{nom_paquet|terme_recherche}}
```
#### Synchronise et met à jour tous les paquets depuis les dépôts et l'AUR :
```shell
yay
```
#### Synchronise et met à jour seulement les paquets de l'AUR :
```shell
yay -Sua
```
#### Installe un nouveau paquet depuis les dépôts et l'AUR :
```shell
yay -S {{nom_paquet}}
```
#### Recherche dans la base de données de paquets un mot clé depuis les dépôts et l'AUR :
```shell
yay -Ss {{mot_clé}}
```
#### Montre des statistiques sur les paquets installés et la santé du système :
```shell
yay -Ps
```
{% endraw %}