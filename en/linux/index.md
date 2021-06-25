---
layout: default
title: "linux"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#medusa">Medusa</a>
* <a href="#a2disconf">a2disconf</a>
* <a href="#a2dismod">a2dismod</a>
* <a href="#a2dissite">a2dissite</a>
* <a href="#a2enconf">a2enconf</a>
* <a href="#a2enmod">a2enmod</a>
* <a href="#a2ensite">a2ensite</a>
* <a href="#a2query">a2query</a>
* <a href="#ac">ac</a>
* <a href="#acpi">acpi</a>
* <a href="#add-apt-repository">add-apt-repository</a>
* <a href="#addpart">addpart</a>
* <a href="#addr2line">addr2line</a>
* <a href="#adduser">adduser</a>
* <a href="#alpine">alpine</a>
* <a href="#amixer">amixer</a>
* <a href="#anbox">anbox</a>
* <a href="#apache2ctl">apache2ctl</a>
* <a href="#apk">apk</a>
* <a href="#aplay">aplay</a>
* <a href="#apport-bug">apport-bug</a>
* <a href="#apt">apt</a>
* <a href="#apt-add-repository">apt-add-repository</a>
* <a href="#apt-cache">apt-cache</a>
* <a href="#apt-file">apt-file</a>
* <a href="#apt-get">apt-get</a>
* <a href="#apt-key">apt-key</a>
* <a href="#apt-mark">apt-mark</a>
* <a href="#aptitude">aptitude</a>
* <a href="#arch-chroot">arch-chroot</a>
* <a href="#archey">archey</a>
* <a href="#archinstall">archinstall</a>
* <a href="#archlinux-java">archlinux-java</a>
* <a href="#arecord">arecord</a>
* <a href="#arithmetic">arithmetic</a>
* <a href="#ark">ark</a>
* <a href="#arp-scan">arp-scan</a>
* <a href="#as">as</a>
* <a href="#ascii">ascii</a>
* <a href="#asciiart">asciiart</a>
* <a href="#aspell">aspell</a>
* <a href="#asterisk">asterisk</a>
* <a href="#at">at</a>
* <a href="#auracle">auracle</a>
* <a href="#aurman">aurman</a>
* <a href="#authconfig">authconfig</a>
* <a href="#autorandr">autorandr</a>
* <a href="#avahi-browse">avahi-browse</a>
* <a href="#balooctl">balooctl</a>
* <a href="#beep">beep</a>
* <a href="#betterlockscreen">betterlockscreen</a>
* <a href="#binwalk">binwalk</a>
* <a href="#bitwise">bitwise</a>
* <a href="#blkdiscard">blkdiscard</a>
* <a href="#blkid">blkid</a>
* <a href="#bluetoothctl">bluetoothctl</a>
* <a href="#bmon">bmon</a>
* <a href="#boltctl">boltctl</a>
* <a href="#bpftrace">bpftrace</a>
* <a href="#bpytop">bpytop</a>
* <a href="#brctl">brctl</a>
* <a href="#btrfs">btrfs</a>
* <a href="#btrfs-device">btrfs device</a>
* <a href="#btrfs-filesystem">btrfs filesystem</a>
* <a href="#btrfs-scrub">btrfs scrub</a>
* <a href="#btrfs-subvolume">btrfs subvolume</a>
* <a href="#cal">cal</a>
* <a href="#calc">calc</a>
* <a href="#calcurse">calcurse</a>
* <a href="#ceph">ceph</a>
* <a href="#certbot">certbot</a>
* <a href="#cewl">cewl</a>
* <a href="#cfdisk">cfdisk</a>
* <a href="#chage">chage</a>
* <a href="#chattr">chattr</a>
* <a href="#chcpu">chcpu</a>
* <a href="#check-support-status">check-support-status</a>
* <a href="#chfn">chfn</a>
* <a href="#chkconfig">chkconfig</a>
* <a href="#chronyc">chronyc</a>
* <a href="#chrt">chrt</a>
* <a href="#clamav">clamav</a>
* <a href="#cmus">cmus</a>
* <a href="#collectd">collectd</a>
* <a href="#colrm">colrm</a>
* <a href="#compgen">compgen</a>
* <a href="#compose">compose</a>
* <a href="#compsize">compsize</a>
* <a href="#conky">conky</a>
* <a href="#coredumpctl">coredumpctl</a>
* <a href="#cp">cp</a>
* <a href="#cpufreq-aperf">cpufreq-aperf</a>
* <a href="#cpufreq-info">cpufreq-info</a>
* <a href="#cpufreq-set">cpufreq-set</a>
* <a href="#cpuid">cpuid</a>
* <a href="#cpulimit">cpulimit</a>
* <a href="#create_ap">create_ap</a>
* <a href="#cryptsetup">cryptsetup</a>
* <a href="#csplit">csplit</a>
* <a href="#ctr">ctr</a>
* <a href="#ctrlaltdel">ctrlaltdel</a>
* <a href="#cuyo">cuyo</a>
* <a href="#daemonize">daemonize</a>
* <a href="#datamash">datamash</a>
* <a href="#dbus-daemon">dbus-daemon</a>
* <a href="#dconf">dconf</a>
* <a href="#dconf-write">dconf write</a>
* <a href="#ddrescue">ddrescue</a>
* <a href="#debchange">debchange</a>
* <a href="#debman">debman</a>
* <a href="#debootstrap">debootstrap</a>
* <a href="#debugfs">debugfs</a>
* <a href="#debuild">debuild</a>
* <a href="#deluser">deluser</a>
* <a href="#dex">dex</a>
* <a href="#dget">dget</a>
* <a href="#diff3">diff3</a>
* <a href="#disown">disown</a>
* <a href="#dkms">dkms</a>
* <a href="#dmenu">dmenu</a>
* <a href="#dmesg">dmesg</a>
* <a href="#dmidecode">dmidecode</a>
* <a href="#dnf">dnf</a>
* <a href="#dnsrecon">dnsrecon</a>
* <a href="#do-release-upgrade">do-release-upgrade</a>
* <a href="#dockerd">dockerd</a>
* <a href="#dolphin">dolphin</a>
* <a href="#dos2unix">dos2unix</a>
* <a href="#dpkg">dpkg</a>
* <a href="#dpkg-deb">dpkg-deb</a>
* <a href="#dpkg-query">dpkg-query</a>
* <a href="#dstat">dstat</a>
* <a href="#dumpe2fs">dumpe2fs</a>
* <a href="#dunstify">dunstify</a>
* <a href="#duperemove">duperemove</a>
* <a href="#e2freefrag">e2freefrag</a>
* <a href="#e2fsck">e2fsck</a>
* <a href="#e2image">e2image</a>
* <a href="#e2label">e2label</a>
* <a href="#e2undo">e2undo</a>
* <a href="#e4defrag">e4defrag</a>
* <a href="#ebuild">ebuild</a>
* <a href="#edit">edit</a>
* <a href="#edquota">edquota</a>
* <a href="#efibootmgr">efibootmgr</a>
* <a href="#eix">eix</a>
* <a href="#eject">eject</a>
* <a href="#emerge">emerge</a>
* <a href="#enum4linux">enum4linux</a>
* <a href="#equery">equery</a>
* <a href="#etckeeper">etckeeper</a>
* <a href="#ethtool">ethtool</a>
* <a href="#eval">eval</a>
* <a href="#exif">exif</a>
* <a href="#expect">expect</a>
* <a href="#export">export</a>
* <a href="#extrace">extrace</a>
* <a href="#extundelete">extundelete</a>
* <a href="#eyed3">eyeD3</a>
* <a href="#f5fpc">f5fpc</a>
* <a href="#fail2ban-client">fail2ban-client</a>
* <a href="#faketime">faketime</a>
* <a href="#fallocate">fallocate</a>
* <a href="#fatlabel">fatlabel</a>
* <a href="#fc">fc</a>
* <a href="#fc-cache">fc-cache</a>
* <a href="#fc-list">fc-list</a>
* <a href="#fc-match">fc-match</a>
* <a href="#fc-pattern">fc-pattern</a>
* <a href="#fcrackzip">fcrackzip</a>
* <a href="#fdisk">fdisk</a>
* <a href="#feedreader">feedreader</a>
* <a href="#feh">feh</a>
* <a href="#file">file</a>
* <a href="#filefrag">filefrag</a>
* <a href="#finch">finch</a>
* <a href="#findfs">findfs</a>
* <a href="#findmnt">findmnt</a>
* <a href="#firejail">firejail</a>
* <a href="#firewall-cmd">firewall-cmd</a>
* <a href="#flameshot">flameshot</a>
* <a href="#flash">flash</a>
* <a href="#flashrom">flashrom</a>
* <a href="#flatpak">flatpak</a>
* <a href="#flatpak-builder">flatpak-builder</a>
* <a href="#foreman">foreman</a>
* <a href="#free">free</a>
* <a href="#fsck">fsck</a>
* <a href="#fstrim">fstrim</a>
* <a href="#fuser">fuser</a>
* <a href="#gcov">gcov</a>
* <a href="#gdebi">gdebi</a>
* <a href="#gedit">gedit</a>
* <a href="#genfstab">genfstab</a>
* <a href="#genid">genid</a>
* <a href="#genie">genie</a>
* <a href="#genkernel">genkernel</a>
* <a href="#getent">getent</a>
* <a href="#getfacl">getfacl</a>
* <a href="#gnome-extensions">gnome-extensions</a>
* <a href="#gnome-terminal">gnome-terminal</a>
* <a href="#google-chrome">google-chrome</a>
* <a href="#gpasswd">gpasswd</a>
* <a href="#groupadd">groupadd</a>
* <a href="#groupdel">groupdel</a>
* <a href="#groupmod">groupmod</a>
* <a href="#grub-install">grub-install</a>
* <a href="#grub-mkconfig">grub-mkconfig</a>
* <a href="#gs">gs</a>
* <a href="#guake">guake</a>
* <a href="#guix-package">guix package</a>
* <a href="#halt">halt</a>
* <a href="#hardinfo">hardinfo</a>
* <a href="#hashcat">hashcat</a>
* <a href="#hdparm">hdparm</a>
* <a href="#hello">hello</a>
* <a href="#hexdump">hexdump</a>
* <a href="#hlint">hlint</a>
* <a href="#homectl">homectl</a>
* <a href="#homeshick">homeshick</a>
* <a href="#hostname">hostname</a>
* <a href="#hostnamectl">hostnamectl</a>
* <a href="#htpdate">htpdate</a>
* <a href="#http-prompt">http-prompt</a>
* <a href="#http_load">http_load</a>
* <a href="#httpie">httpie</a>
* <a href="#hwclock">hwclock</a>
* <a href="#i3">i3</a>
* <a href="#i3lock">i3lock</a>
* <a href="#i7z">i7z</a>
* <a href="#ifdown">ifdown</a>
* <a href="#iftop">iftop</a>
* <a href="#ifup">ifup</a>
* <a href="#imgp">imgp</a>
* <a href="#inotifywait">inotifywait</a>
* <a href="#inxi">inxi</a>
* <a href="#iostat">iostat</a>
* <a href="#ip">ip</a>
* <a href="#ip-address">ip address</a>
* <a href="#ip-link">ip link</a>
* <a href="#ip-route">ip route</a>
* <a href="#ip-neighbour">ip-neighbour</a>
* <a href="#ipcalc">ipcalc</a>
* <a href="#ipcmk">ipcmk</a>
* <a href="#ipcrm">ipcrm</a>
* <a href="#iptables">iptables</a>
* <a href="#isoinfo">isoinfo</a>
* <a href="#isosize">isosize</a>
* <a href="#iw">iw</a>
* <a href="#iwconfig">iwconfig</a>
* <a href="#iwctl">iwctl</a>
* <a href="#jobs">jobs</a>
* <a href="#journalctl">journalctl</a>
* <a href="#jpegtran">jpegtran</a>
* <a href="#kde-inhibit">kde-inhibit</a>
* <a href="#kdocker">kdocker</a>
* <a href="#kexec">kexec</a>
* <a href="#kjv">kjv</a>
* <a href="#konsole">konsole</a>
* <a href="#kpackagetool5">kpackagetool5</a>
* <a href="#kpartx">kpartx</a>
* <a href="#kreadconfig5">kreadconfig5</a>
* <a href="#ksvgtopng5">ksvgtopng5</a>
* <a href="#kwriteconfig5">kwriteconfig5</a>
* <a href="#larasail">larasail</a>
* <a href="#lastb">lastb</a>
* <a href="#lastcomm">lastcomm</a>
* <a href="#lastlog">lastlog</a>
* <a href="#ldconfig">ldconfig</a>
* <a href="#ldd">ldd</a>
* <a href="#legit">legit</a>
* <a href="#lftp">lftp</a>
* <a href="#libreoffice">libreoffice</a>
* <a href="#light">light</a>
* <a href="#line">line</a>
* <a href="#locate">locate</a>
* <a href="#logger">logger</a>
* <a href="#login">login</a>
* <a href="#logsave">logsave</a>
* <a href="#logwatch">logwatch</a>
* <a href="#losetup">losetup</a>
* <a href="#lrunzip">lrunzip</a>
* <a href="#lrzip">lrzip</a>
* <a href="#lrztar">lrztar</a>
* <a href="#lrzuntar">lrzuntar</a>
* <a href="#lsattr">lsattr</a>
* <a href="#lsb_release">lsb_release</a>
* <a href="#lsblk">lsblk</a>
* <a href="#lscpu">lscpu</a>
* <a href="#lshw">lshw</a>
* <a href="#lslocks">lslocks</a>
* <a href="#lslogins">lslogins</a>
* <a href="#lsmod">lsmod</a>
* <a href="#lspci">lspci</a>
* <a href="#lsscsi">lsscsi</a>
* <a href="#lsusb">lsusb</a>
* <a href="#ltrace">ltrace</a>
* <a href="#lvcreate">lvcreate</a>
* <a href="#lvdisplay">lvdisplay</a>
* <a href="#lvextend">lvextend</a>
* <a href="#lvm">lvm</a>
* <a href="#lvreduce">lvreduce</a>
* <a href="#lvremove">lvremove</a>
* <a href="#lvresize">lvresize</a>
* <a href="#lvs">lvs</a>
* <a href="#lxc">lxc</a>
* <a href="#lxterminal">lxterminal</a>
* <a href="#lynis">lynis</a>
* <a href="#mac2unix">mac2unix</a>
* <a href="#macchanger">macchanger</a>
* <a href="#maim">maim</a>
* <a href="#makepkg">makepkg</a>
* <a href="#mandb">mandb</a>
* <a href="#manpath">manpath</a>
* <a href="#mcookie">mcookie</a>
* <a href="#mdadm">mdadm</a>
* <a href="#mdbook">mdbook</a>
* <a href="#microcom">microcom</a>
* <a href="#mimetype">mimetype</a>
* <a href="#mke2fs">mke2fs</a>
* <a href="#mkfs">mkfs</a>
* <a href="#mkfs.btrfs">mkfs.btrfs</a>
* <a href="#mkfs.cramfs">mkfs.cramfs</a>
* <a href="#mkfs.exfat">mkfs.exfat</a>
* <a href="#mkfs.ext4">mkfs.ext4</a>
* <a href="#mkfs.fat">mkfs.fat</a>
* <a href="#mkfs.minix">mkfs.minix</a>
* <a href="#mkfs.ntfs">mkfs.ntfs</a>
* <a href="#mkfs.vfat">mkfs.vfat</a>
* <a href="#mkinitcpio">mkinitcpio</a>
* <a href="#mkisofs">mkisofs</a>
* <a href="#mklost+found">mklost+found</a>
* <a href="#mknod">mknod</a>
* <a href="#mkswap">mkswap</a>
* <a href="#mmcli">mmcli</a>
* <a href="#mocp">mocp</a>
* <a href="#modinfo">modinfo</a>
* <a href="#modprobe">modprobe</a>
* <a href="#module">module</a>
* <a href="#mono">mono</a>
* <a href="#mons">mons</a>
* <a href="#mountpoint">mountpoint</a>
* <a href="#mpstat">mpstat</a>
* <a href="#mssh">mssh</a>
* <a href="#mullvad">mullvad</a>
* <a href="#mycli">mycli</a>
* <a href="#n">n</a>
* <a href="#named">named</a>
* <a href="#namei">namei</a>
* <a href="#nautilus">nautilus</a>
* <a href="#ncat">ncat</a>
* <a href="#ncdu">ncdu</a>
* <a href="#ndctl">ndctl</a>
* <a href="#nemo">nemo</a>
* <a href="#nethogs">nethogs</a>
* <a href="#netselect">netselect</a>
* <a href="#netselect-apt">netselect-apt</a>
* <a href="#netstat">netstat</a>
* <a href="#newgrp">newgrp</a>
* <a href="#nft">nft</a>
* <a href="#nixos-rebuild">nixos-rebuild</a>
* <a href="#nm">nm</a>
* <a href="#nmcli">nmcli</a>
* <a href="#nmcli-connection">nmcli connection</a>
* <a href="#nmcli-device">nmcli device</a>
* <a href="#nmon">nmon</a>
* <a href="#nmtui">nmtui</a>
* <a href="#nologin">nologin</a>
* <a href="#notify-send">notify-send</a>
* <a href="#nsenter">nsenter</a>
* <a href="#nsnake">nsnake</a>
* <a href="#ntfsfix">ntfsfix</a>
* <a href="#ntpq">ntpq</a>
* <a href="#numactl">numactl</a>
* <a href="#numlockx">numlockx</a>
* <a href="#openfortivpn">openfortivpn</a>
* <a href="#openrc">openrc</a>
* <a href="#openvpn3">openvpn3</a>
* <a href="#opkg">opkg</a>
* <a href="#pacaur">pacaur</a>
* <a href="#paccache">paccache</a>
* <a href="#pacman">pacman</a>
* <a href="#pacman---database">pacman --database</a>
* <a href="#pacman---deptest">pacman --deptest</a>
* <a href="#pacman---files">pacman --files</a>
* <a href="#pacman---query">pacman --query</a>
* <a href="#pacman---remove">pacman --remove</a>
* <a href="#pacman---sync">pacman --sync</a>
* <a href="#pacman---upgrade">pacman --upgrade</a>
* <a href="#pacman-mirrors">pacman-mirrors</a>
* <a href="#pacman4console">pacman4console</a>
* <a href="#pacstrap">pacstrap</a>
* <a href="#pamac">pamac</a>
* <a href="#parted">parted</a>
* <a href="#partprobe">partprobe</a>
* <a href="#partx">partx</a>
* <a href="#paru">paru</a>
* <a href="#pasuspender">pasuspender</a>
* <a href="#pdfgrep">pdfgrep</a>
* <a href="#perf">perf</a>
* <a href="#phar">phar</a>
* <a href="#photorec">photorec</a>
* <a href="#phpdismod">phpdismod</a>
* <a href="#phpenmod">phpenmod</a>
* <a href="#phpquery">phpquery</a>
* <a href="#physlock">physlock</a>
* <a href="#pi">pi</a>
* <a href="#pidof">pidof</a>
* <a href="#pidstat">pidstat</a>
* <a href="#pihole">pihole</a>
* <a href="#pivpn">pivpn</a>
* <a href="#pkg-config">pkg-config</a>
* <a href="#pkgadd">pkgadd</a>
* <a href="#pkgfile">pkgfile</a>
* <a href="#pkginfo">pkginfo</a>
* <a href="#pkgmk">pkgmk</a>
* <a href="#pkgrm">pkgrm</a>
* <a href="#playerctl">playerctl</a>
* <a href="#pmount">pmount</a>
* <a href="#ports">ports</a>
* <a href="#postfix">postfix</a>
* <a href="#poweroff">poweroff</a>
* <a href="#powertop">powertop</a>
* <a href="#print">print</a>
* <a href="#progress">progress</a>
* <a href="#protontricks">protontricks</a>
* <a href="#prt-get">prt-get</a>
* <a href="#pstree">pstree</a>
* <a href="#ptx">ptx</a>
* <a href="#pulseaudio">pulseaudio</a>
* <a href="#pvcreate">pvcreate</a>
* <a href="#pvdisplay">pvdisplay</a>
* <a href="#pvs">pvs</a>
* <a href="#pwdx">pwdx</a>
* <a href="#pwgen">pwgen</a>
* <a href="#qjoypad">qjoypad</a>
* <a href="#qsub">qsub</a>
* <a href="#qtchooser">qtchooser</a>
* <a href="#quotacheck">quotacheck</a>
* <a href="#radeontop">radeontop</a>
* <a href="#rankmirrors">rankmirrors</a>
* <a href="#rc-service">rc-service</a>
* <a href="#rc-status">rc-status</a>
* <a href="#rc-update">rc-update</a>
* <a href="#rdesktop">rdesktop</a>
* <a href="#readelf">readelf</a>
* <a href="#reboot">reboot</a>
* <a href="#reflector">reflector</a>
* <a href="#rename">rename</a>
* <a href="#rename">rename</a>
* <a href="#rename">rename</a>
* <a href="#rename">rename</a>
* <a href="#reportbug">reportbug</a>
* <a href="#repquota">repquota</a>
* <a href="#reset">reset</a>
* <a href="#resize2fs">resize2fs</a>
* <a href="#resolveip">resolveip</a>
* <a href="#rfkill">rfkill</a>
* <a href="#rig">rig</a>
* <a href="#rofi">rofi</a>
* <a href="#rolldice">rolldice</a>
* <a href="#rpcclient">rpcclient</a>
* <a href="#rpcinfo">rpcinfo</a>
* <a href="#rpm">rpm</a>
* <a href="#rpmbuild">rpmbuild</a>
* <a href="#rspamc">rspamc</a>
* <a href="#rtcwake">rtcwake</a>
* <a href="#rtorrent">rtorrent</a>
* <a href="#run-mailcap">run-mailcap</a>
* <a href="#runcon">runcon</a>
* <a href="#runuser">runuser</a>
* <a href="#rusnapshot">rusnapshot</a>
* <a href="#sa">sa</a>
* <a href="#sacct">sacct</a>
* <a href="#sacctmgr">sacctmgr</a>
* <a href="#sam">sam</a>
* <a href="#sar">sar</a>
* <a href="#sbatch">sbatch</a>
* <a href="#scancel">scancel</a>
* <a href="#scanimage">scanimage</a>
* <a href="#schroot">schroot</a>
* <a href="#scontrol">scontrol</a>
* <a href="#screenkey">screenkey</a>
* <a href="#script">script</a>
* <a href="#scriptreplay">scriptreplay</a>
* <a href="#scrot">scrot</a>
* <a href="#see">see</a>
* <a href="#semanage">semanage</a>
* <a href="#sensible-browser">sensible-browser</a>
* <a href="#sensible-editor">sensible-editor</a>
* <a href="#sensors">sensors</a>
* <a href="#service">service</a>
* <a href="#setfacl">setfacl</a>
* <a href="#setxkbmap">setxkbmap</a>
* <a href="#sfill">sfill</a>
* <a href="#shutdown">shutdown</a>
* <a href="#sic">sic</a>
* <a href="#silentcast">silentcast</a>
* <a href="#sinfo">sinfo</a>
* <a href="#slapt-get">slapt-get</a>
* <a href="#slapt-src">slapt-src</a>
* <a href="#slop">slop</a>
* <a href="#sm">sm</a>
* <a href="#smbclient">smbclient</a>
* <a href="#smbget">smbget</a>
* <a href="#smbmap">smbmap</a>
* <a href="#smbpasswd">smbpasswd</a>
* <a href="#snake4">snake4</a>
* <a href="#snake4scores">snake4scores</a>
* <a href="#snap">snap</a>
* <a href="#snapper">snapper</a>
* <a href="#snmpwalk">snmpwalk</a>
* <a href="#spectre-meltdown-checker">spectre-meltdown-checker</a>
* <a href="#speedometer">speedometer</a>
* <a href="#spi">spi</a>
* <a href="#squeue">squeue</a>
* <a href="#sreport">sreport</a>
* <a href="#srun">srun</a>
* <a href="#ss">ss</a>
* <a href="#ssh-add">ssh-add</a>
* <a href="#sshuttle">sshuttle</a>
* <a href="#sstat">sstat</a>
* <a href="#steghide">steghide</a>
* <a href="#strace">strace</a>
* <a href="#stress">stress</a>
* <a href="#swapoff">swapoff</a>
* <a href="#swapon">swapon</a>
* <a href="#swupd">swupd</a>
* <a href="#sxiv">sxiv</a>
* <a href="#sysctl">sysctl</a>
* <a href="#systemctl">systemctl</a>
* <a href="#systemd-analyze">systemd-analyze</a>
* <a href="#taskset">taskset</a>
* <a href="#tcpflow">tcpflow</a>
* <a href="#tcpkill">tcpkill</a>
* <a href="#tcptraceroute">tcptraceroute</a>
* <a href="#terminator">terminator</a>
* <a href="#thunar">thunar</a>
* <a href="#tic">tic</a>
* <a href="#timedatectl">timedatectl</a>
* <a href="#timeshift">timeshift</a>
* <a href="#tlp">tlp</a>
* <a href="#tlp-stat">tlp-stat</a>
* <a href="#toilet">toilet</a>
* <a href="#tomb">tomb</a>
* <a href="#top">top</a>
* <a href="#tracepath">tracepath</a>
* <a href="#trap">trap</a>
* <a href="#trash">trash</a>
* <a href="#tree">tree</a>
* <a href="#trizen">trizen</a>
* <a href="#tshark">tshark</a>
* <a href="#tune2fs">tune2fs</a>
* <a href="#tuxi">tuxi</a>
* <a href="#udisksctl">udisksctl</a>
* <a href="#ufw">ufw</a>
* <a href="#ul">ul</a>
* <a href="#unix2dos">unix2dos</a>
* <a href="#unix2mac">unix2mac</a>
* <a href="#unset">unset</a>
* <a href="#unshadow">unshadow</a>
* <a href="#update-alternatives">update-alternatives</a>
* <a href="#update-rc.d">update-rc.d</a>
* <a href="#updatedb">updatedb</a>
* <a href="#upower">upower</a>
* <a href="#uprecords">uprecords</a>
* <a href="#urxvt">urxvt</a>
* <a href="#useradd">useradd</a>
* <a href="#userdel">userdel</a>
* <a href="#usermod">usermod</a>
* <a href="#utmpdump">utmpdump</a>
* <a href="#uuid">uuid</a>
* <a href="#uuidd">uuidd</a>
* <a href="#uuidgen">uuidgen</a>
* <a href="#uvcdynctrl">uvcdynctrl</a>
* <a href="#veracrypt">veracrypt</a>
* <a href="#vgcreate">vgcreate</a>
* <a href="#vgdisplay">vgdisplay</a>
* <a href="#vgs">vgs</a>
* <a href="#viewnior">viewnior</a>
* <a href="#vipw">vipw</a>
* <a href="#virt-manager">virt-manager</a>
* <a href="#vmstat">vmstat</a>
* <a href="#vmware-checkvm">vmware-checkvm</a>
* <a href="#vncserver">vncserver</a>
* <a href="#vncviewer">vncviewer</a>
* <a href="#vnstat">vnstat</a>
* <a href="#vpnc">vpnc</a>
* <a href="#vrms">vrms</a>
* <a href="#w">w</a>
* <a href="#wall">wall</a>
* <a href="#watch">watch</a>
* <a href="#wg">wg</a>
* <a href="#wg-quick">wg-quick</a>
* <a href="#whatis">whatis</a>
* <a href="#whereis">whereis</a>
* <a href="#whiptail">whiptail</a>
* <a href="#wine">wine</a>
* <a href="#winetricks">winetricks</a>
* <a href="#wipefs">wipefs</a>
* <a href="#wmctrl">wmctrl</a>
* <a href="#wodim">wodim</a>
* <a href="#wol">wol</a>
* <a href="#wpa_cli">wpa_cli</a>
* <a href="#wpa_passphrase">wpa_passphrase</a>
* <a href="#wtf">wtf</a>
* <a href="#x0vncserver">x0vncserver</a>
* <a href="#x11vnc">x11vnc</a>
* <a href="#xar">xar</a>
* <a href="#xbacklight">xbacklight</a>
* <a href="#xbps">xbps</a>
* <a href="#xclip">xclip</a>
* <a href="#xclock">xclock</a>
* <a href="#xcursorgen">xcursorgen</a>
* <a href="#xdg-mime">xdg-mime</a>
* <a href="#xdg-open">xdg-open</a>
* <a href="#xdotool">xdotool</a>
* <a href="#xeyes">xeyes</a>
* <a href="#xfce4-screenshooter">xfce4-screenshooter</a>
* <a href="#xfce4-terminal">xfce4-terminal</a>
* <a href="#xinput">xinput</a>
* <a href="#xman">xman</a>
* <a href="#xmount">xmount</a>
* <a href="#xrandr">xrandr</a>
* <a href="#xsel">xsel</a>
* <a href="#xsetwacom">xsetwacom</a>
* <a href="#xterm">xterm</a>
* <a href="#xtrlock">xtrlock</a>
* <a href="#xvfb-run">xvfb-run</a>
* <a href="#yank">yank</a>
* <a href="#yaourt">yaourt</a>
* <a href="#yay">yay</a>
* <a href="#yetris">yetris</a>
* <a href="#yum">yum</a>
* <a href="#zenity">zenity</a>
* <a href="#zgrep">zgrep</a>
* <a href="#zile">zile</a>
* <a href="#zramctl">zramctl</a>
* <a href="#zypper">zypper</a>

{% raw %}
<h2 id="a2disconf">
  <a href="/en/linux/a2disconf.html">a2disconf</a> <a href="#a2disconf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Disable an Apache configuration file on Debian-based OSes.
> More information: <https://manpages.debian.org/latest/apache2/a2disconf.8.en.html>.

#### Disable a configuration file:
```shell
sudo a2disconf {{configuration_file}}
```
#### Don't show informative messages:
```shell
sudo a2disconf --quiet {{configuration_file}}
```
{% endraw %}{% raw %}
<h2 id="a2dismod">
  <a href="/en/linux/a2dismod.html">a2dismod</a> <a href="#a2dismod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Disable an Apache module on Debian-based OSes.
> More information: <https://manpages.debian.org/latest/apache2/a2dismod.8.en.html>.

#### Disable a module:
```shell
sudo a2dismod {{module}}
```
#### Don't show informative messages:
```shell
sudo a2dismod --quiet {{module}}
```
{% endraw %}{% raw %}
<h2 id="a2dissite">
  <a href="/en/linux/a2dissite.html">a2dissite</a> <a href="#a2dissite"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Disable an Apache virtual host on Debian-based OSes.
> More information: <https://manpages.debian.org/latest/apache2/a2dissite.8.en.html>.

#### Disable a virtual host:
```shell
sudo a2dissite {{virtual_host}}
```
#### Don't show informative messages:
```shell
sudo a2dissite --quiet {{virtual_host}}
```
{% endraw %}{% raw %}
<h2 id="a2enconf">
  <a href="/en/linux/a2enconf.html">a2enconf</a> <a href="#a2enconf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Enable an Apache configuration file on Debian-based OSes.
> More information: <https://manpages.debian.org/latest/apache2/a2enconf.8.en.html>.

#### Enable a configuration file:
```shell
sudo a2enconf {{configuration_file}}
```
#### Don't show informative messages:
```shell
sudo a2enconf --quiet {{configuration_file}}
```
{% endraw %}{% raw %}
<h2 id="a2enmod">
  <a href="/en/linux/a2enmod.html">a2enmod</a> <a href="#a2enmod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Enable an Apache module on Debian-based OSes.
> More information: <https://manpages.debian.org/latest/apache2/a2enmod.8.en.html>.

#### Enable a module:
```shell
sudo a2enmod {{module}}
```
#### Don't show informative messages:
```shell
sudo a2enmod --quiet {{module}}
```
{% endraw %}{% raw %}
<h2 id="a2ensite">
  <a href="/en/linux/a2ensite.html">a2ensite</a> <a href="#a2ensite"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Enable an Apache virtual host on Debian-based OSes.
> More information: <https://manpages.debian.org/latest/apache2/a2ensite.8.en.html>.

#### Enable a virtual host:
```shell
sudo a2ensite {{virtual_host}}
```
#### Don't show informative messages:
```shell
sudo a2ensite --quiet {{virtual_host}}
```
{% endraw %}{% raw %}
<h2 id="a2query">
  <a href="/en/linux/a2query.html">a2query</a> <a href="#a2query"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Retrieve runtime configuration from Apache on Debian-based OSes.
> More information: <https://manpages.debian.org/buster/apache2/a2query.1.en.html>.

#### List enabled Apache modules:
```shell
sudo a2query -m
```
#### Check if a specific module is installed:
```shell
sudo a2query -m {{module_name}}
```
#### List enabled virtual hosts:
```shell
sudo a2query -s
```
#### Display the currently enabled Multi Processing Module:
```shell
sudo a2query -M
```
#### Display the Apache version:
```shell
sudo a2query -v
```
{% endraw %}{% raw %}
<h2 id="ac">
  <a href="/en/linux/ac.html">ac</a> <a href="#ac"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print statistics on how long users have been connected.

#### Print how long the current user has been connected in hours:
```shell
ac
```
#### Print how long users have been connected in hours:
```shell
ac --individual-totals
```
#### Print how long a particular user has been connected in hours:
```shell
ac --individual-totals {{username}}
```
#### Print how long a particular user has been connected in hours per day (with total):
```shell
ac --daily-totals --individual-totals {{username}}
```
#### Also display additional details:
```shell
ac --compatibility
```
{% endraw %}{% raw %}
<h2 id="acpi">
  <a href="/en/linux/acpi.html">acpi</a> <a href="#acpi"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Shows battery status or thermal information.
> More information: <https://sourceforge.net/projects/acpiclient/files/acpiclient/>.

#### Show battery information:
```shell
acpi
```
#### Show thermal information:
```shell
acpi -t
```
#### Show cooling device information:
```shell
acpi -c
```
#### Show thermal information in Fahrenheit:
```shell
acpi -tf
```
#### Show all information:
```shell
acpi -V
```
#### Extract information from `/proc` instead of `/sys`:
```shell
acpi -p
```
{% endraw %}{% raw %}
<h2 id="add-apt-repository">
  <a href="/en/linux/add-apt-repository.html">add-apt-repository</a> <a href="#add-apt-repository"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manages apt repository definitions.

#### Add a new apt repository:
```shell
add-apt-repository {{repository_spec}}
```
#### Remove an apt repository:
```shell
add-apt-repository --remove {{repository_spec}}
```
#### Update the package cache after adding a repository:
```shell
add-apt-repository --update {{repository_spec}}
```
#### Enable source packages:
```shell
add-apt-repository --enable-source {{repository_spec}}
```
{% endraw %}{% raw %}
<h2 id="addpart">
  <a href="/en/linux/addpart.html">addpart</a> <a href="#addpart"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tells the Linux kernel about the existence of the specified partition.
> The command is a simple wrapper around the `add partition` ioctl.
> More information: <https://manned.org/addpart>.

#### Tell the kernel about the existence of the specified partition:
```shell
addpart {{device}} {{partition}} {{start}} {{length}}
```
{% endraw %}{% raw %}
<h2 id="addr2line">
  <a href="/en/linux/addr2line.html">addr2line</a> <a href="#addr2line"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Convert addresses of a binary into file names and line numbers.

#### Display the filename and line number of the source code from an instruction address of an executable:
```shell
addr2line --exe={{path/to/executable}} {{address}}
```
#### Display the function name, filename and line number:
```shell
addr2line --exe={{path/to/executable}} --functions {{address}}
```
#### Demangle the function name for C++ code:
```shell
addr2line --exe={{path/to/executable}} --functions --demangle {{address}}
```
{% endraw %}{% raw %}
<h2 id="adduser">
  <a href="/en/linux/adduser.html">adduser</a> <a href="#adduser"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> User addition utility.
> More information: <https://manpages.debian.org/latest/adduser/adduser.html>.

#### Create a new user with a default home directory and prompt the user to set a password:
```shell
adduser {{username}}
```
#### Create a new user without a home directory:
```shell
adduser --no-create-home {{username}}
```
#### Create a new user with a home directory at the specified path:
```shell
adduser --home {{path/to/home}} {{username}}
```
#### Create a new user with the specified shell set as the login shell:
```shell
adduser --shell {{path/to/shell}} {{username}}
```
#### Create a new user belonging to the specified group:
```shell
adduser --ingroup {{group}} {{username}}
```
#### Add an existing user to the specified group:
```shell
adduser {{username}} {{group}}
```
{% endraw %}{% raw %}
<h2 id="alpine">
  <a href="/en/linux/alpine.html">alpine</a> <a href="#alpine"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An email client and Usenet newsgroup program with a pico/nano-inspired interface.
> Supports most modern email services through IMAP.

#### Open alpine normally:
```shell
alpine
```
#### Open alpine directly to the message composition screen to send an email to a given email address:
```shell
alpine {{email@example.net}}
```
#### Quit alpine:
```shell
'q' then 'y'
```
{% endraw %}{% raw %}
<h2 id="amixer">
  <a href="/en/linux/amixer.html">amixer</a> <a href="#amixer"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mixer for ALSA soundcard driver.

#### Turn up the master volume by 10%:
```shell
amixer -D pulse sset Master {{10%+}}
```
#### Turn down the master volume by 10%:
```shell
amixer -D pulse sset Master {{10%-}}
```
{% endraw %}{% raw %}
<h2 id="anbox">
  <a href="/en/linux/anbox.html">anbox</a> <a href="#anbox"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run Android applications on any GNU/Linux operating system.
> More information: <https://manned.org/anbox>.

#### Launch Anbox into the app manager:
```shell
anbox launch --package={{org.anbox.appmgr}} --component={{org.anbox.appmgr.AppViewActivity}}
```
{% endraw %}{% raw %}
<h2 id="apache2ctl">
  <a href="/en/linux/apache2ctl.html">apache2ctl</a> <a href="#apache2ctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The CLI tool to administrate HTTP web server Apache.
> This command comes with Debian based OSes, for RHEL based ones see `httpd`.
> More information: <https://manpages.debian.org/latest/apache2/apache2ctl.8.en.html>.

#### Start the Apache daemon. Throw a message if it is already running:
```shell
sudo apache2ctl start
```
#### Stop the Apache daemon:
```shell
sudo apache2ctl stop
```
#### Restart the Apache daemon:
```shell
sudo apache2ctl restart
```
#### Test syntax of the configuration file:
```shell
sudo apache2ctl -t
```
#### List loaded modules:
```shell
sudo apache2ctl -M
```
{% endraw %}{% raw %}
<h2 id="apk">
  <a href="/en/linux/apk.html">apk</a> <a href="#apk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Alpine Linux package management tool.

#### Update repository indexes from all remote repositories:
```shell
apk update
```
#### Install a new package:
```shell
apk add {{package}}
```
#### Remove a package:
```shell
apk del {{package}}
```
#### Repair package or upgrade it without modifying main dependencies:
```shell
apk fix {{package}}
```
#### Search package via keyword:
```shell
apk search {{keyword}}
```
#### Get info about a specific package:
```shell
apk info {{package}}
```
{% endraw %}{% raw %}
<h2 id="aplay">
  <a href="/en/linux/aplay.html">aplay</a> <a href="#aplay"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line sound player for ALSA soundcard driver.
> More information: <https://manned.org/aplay>.

#### Play a specific file (sampling rate, bit depth, etc. will be automatically determined for the file format):
```shell
aplay {{path/to/file}}
```
#### Play the first 10 seconds of a specific file at 2500Hz:
```shell
aplay --duration={{10}} --rate={{2500}} {{path/to/file}}
```
#### Play the raw file as a 22050Hz, mono, 8-bit, Mu-Law `.au` file:
```shell
aplay --channels={{1}} --file-type {{raw}} --rate={{22050}} --format={{mu_law}} {{path/to/file}}
```
{% endraw %}{% raw %}
<h2 id="apport-bug">
  <a href="/en/linux/apport-bug.html">apport-bug</a> <a href="#apport-bug"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> File a bug report on Ubuntu.
> More information: <https://wiki.ubuntu.com/Apport>.

#### Report a bug about the whole system:
```shell
apport-bug
```
#### Report a bug about a specific package:
```shell
apport-bug {{package}}
```
#### Report a bug about a specific executable:
```shell
apport-bug {{path/to/executable}}
```
#### Report a bug about a specific process:
```shell
apport-bug {{PID}}
```
{% endraw %}{% raw %}
<h2 id="apt-add-repository">
  <a href="/en/linux/apt-add-repository.html">apt-add-repository</a> <a href="#apt-add-repository"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manages apt repository definitions.
> More information: <https://manpages.debian.org/latest/software-properties-common/apt-add-repository.1.html>.

#### Add a new apt repository:
```shell
apt-add-repository {{repository_spec}}
```
#### Remove an apt repository:
```shell
apt-add-repository --remove {{repository_spec}}
```
#### Update the package cache after adding a repository:
```shell
apt-add-repository --update {{repository_spec}}
```
#### Enable source packages:
```shell
apt-add-repository --enable-source {{repository_spec}}
```
{% endraw %}{% raw %}
<h2 id="apt-cache">
  <a href="/en/linux/apt-cache.html">apt-cache</a> <a href="#apt-cache"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Debian and Ubuntu package query tool.
> More information: <https://manpages.debian.org/latest/apt/apt-cache.8.html>.

#### Search for a package in your current sources:
```shell
apt-cache search {{query}}
```
#### Show information about a package:
```shell
apt-cache show {{package}}
```
#### Show whether a package is installed and up to date:
```shell
apt-cache policy {{package}}
```
#### Show dependencies for a package:
```shell
apt-cache depends {{package}}
```
#### Show packages that depend on a particular package:
```shell
apt-cache rdepends {{package}}
```
{% endraw %}{% raw %}
<h2 id="apt-file">
  <a href="/en/linux/apt-file.html">apt-file</a> <a href="#apt-file"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Search for files in apt packages, including ones not yet installed.
> More information: <https://manpages.debian.org/latest/apt-file/apt-file.1.html>.

#### Update the metadata database:
```shell
sudo apt update
```
#### Search for packages that contain the specified file or path:
```shell
apt-file {{search|find}} {{part/of/filename}}
```
#### List the contents of a specific package:
```shell
apt-file {{show|list}} {{package_name}}
```
#### Search for packages that match the regular expression given in `pattern`:
```shell
apt-file {{search|find}} --regexp {{regular_expression}}
```
{% endraw %}{% raw %}
<h2 id="apt-get">
  <a href="/en/linux/apt-get.html">apt-get</a> <a href="#apt-get"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Debian and Ubuntu package management utility.
> Search for packages using `apt-cache`.
> More information: <https://manpages.debian.org/latest/apt/apt-get.8.html>.

#### Update the list of available packages and versions (it's recommended to run this before other `apt-get` commands):
```shell
apt-get update
```
#### Install a package, or update it to the latest available version:
```shell
apt-get install {{package}}
```
#### Remove a package:
```shell
apt-get remove {{package}}
```
#### Remove a package and its configuration files:
```shell
apt-get purge {{package}}
```
#### Upgrade all installed packages to their newest available versions:
```shell
apt-get upgrade
```
#### Clean the local repository - removing package files (`.deb`) from interrupted downloads that can no longer be downloaded:
```shell
apt-get autoclean
```
#### Remove all packages that are no longer needed:
```shell
apt-get autoremove
```
#### Upgrade installed packages (like `upgrade`), but remove obsolete packages and install additional packages to meet new dependencies:
```shell
apt-get dist-upgrade
```
{% endraw %}{% raw %}
<h2 id="apt-key">
  <a href="/en/linux/apt-key.html">apt-key</a> <a href="#apt-key"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Key management utility for the APT Package Manager on Debian and Ubuntu.
> Note: `apt-key` is now deprecated (except for the use of `apt-key del` in maintainer scripts).
> More information: <https://manpages.debian.org/latest/apt/apt-key.8.html>.

#### List trusted keys:
```shell
apt-key list
```
#### Add a key to the trusted keystore:
```shell
apt-key add {{public_key_file.asc}}
```
#### Delete a key from the trusted keystore:
```shell
apt-key del {{key_id}}
```
#### Add a remote key to the trusted keystore:
```shell
wget -qO - {{https://host.tld/filename.key}} | apt-key add -
```
#### Add a key from keyserver with only key id:
```shell
apt-key adv --keyserver {{pgp.mit.edu}} --recv {{KEYID}}
```
{% endraw %}{% raw %}
<h2 id="apt-mark">
  <a href="/en/linux/apt-mark.html">apt-mark</a> <a href="#apt-mark"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility to change the status of installed packages.
> More information: <https://manpages.debian.org/latest/apt/apt-mark.8.html>.

#### Mark a package as automatically installed:
```shell
sudo apt-mark auto {{package_name}}
```
#### Hold a package at its current version and prevent updates to it:
```shell
sudo apt-mark hold {{package_name}}
```
#### Allow a package to be updated again:
```shell
sudo apt-mark unhold {{package_name}}
```
#### Show manually installed packages:
```shell
apt-mark showmanual
```
#### Show held packages that aren't being updated:
```shell
apt-mark showhold
```
{% endraw %}{% raw %}
<h2 id="apt">
  <a href="/en/linux/apt.html">apt</a> <a href="#apt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Package management utility for Debian based distributions.
> Recommended replacement for apt-get when used interactively in Ubuntu versions 16.04 and later.
> More information: <https://manpages.debian.org/latest/apt/apt.8.html>.

#### Update the list of available packages and versions (it's recommended to run this before other `apt` commands):
```shell
sudo apt update
```
#### Search for a given package:
```shell
apt search {{package}}
```
#### Show information for a package:
```shell
apt show {{package}}
```
#### Install a package, or update it to the latest available version:
```shell
sudo apt install {{package}}
```
#### Remove a package (using `purge` instead also removes its configuration files):
```shell
sudo apt remove {{package}}
```
#### Upgrade all installed packages to their newest available versions:
```shell
sudo apt upgrade
```
#### List all packages:
```shell
apt list
```
#### List installed packages:
```shell
apt list --installed
```
{% endraw %}{% raw %}
<h2 id="aptitude">
  <a href="/en/linux/aptitude.html">aptitude</a> <a href="#aptitude"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Debian and Ubuntu package management utility.
> More information: <https://manpages.debian.org/latest/aptitude/aptitude.8.html>.

#### Synchronize list of packages and versions available. This should be run first, before running subsequent aptitude commands:
```shell
aptitude update
```
#### Install a new package and its dependencies:
```shell
aptitude install {{package}}
```
#### Search for a package:
```shell
aptitude search {{package}}
```
#### Search for an installed package (`?installed` is an aptitude search term):
```shell
aptitude search '?installed({{package}})'
```
#### Remove a package and all packages depending on it:
```shell
aptitude remove {{package}}
```
#### Upgrade installed packages to newest available versions:
```shell
aptitude upgrade
```
#### Upgrade installed packages (like `aptitude upgrade`) including removing obsolete packages and installing additional packages to meet new package dependencies:
```shell
aptitude full-upgrade
```
#### Put an installed package on hold to prevent it from being automatically upgraded:
```shell
aptitude hold '?installed({{package}})'
```
{% endraw %}{% raw %}
<h2 id="arch-chroot">
  <a href="/en/linux/arch-chroot.html">arch-chroot</a> <a href="#arch-chroot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Enhanced `chroot` command to help in the Arch Linux installation process.
> More information: <https://man.archlinux.org/man/arch-chroot.8>.

#### Start an interactive shell (`bash`, by default) in a new root directory:
```shell
arch-chroot {{path/to/new/root}}
```
#### Specify the user (other than the current user) to run the shell as:
```shell
arch-chroot -u {{user}} {{path/to/new/root}}
```
#### Run a custom command (instead of the default `bash`) in the new root directory:
```shell
arch-chroot {{path/to/new/root}} {{command}} {{command_arguments}}
```
#### Specify the shell, other than the default `bash` (in this case, the `zsh` package should have been installed in the target system):
```shell
arch-chroot {{path/to/new/root}} {{zsh}}
```
{% endraw %}{% raw %}
<h2 id="archey">
  <a href="/en/linux/archey.html">archey</a> <a href="#archey"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Simple tool for stylishly displaying system information.

#### Show system information:
```shell
archey
```
{% endraw %}{% raw %}
<h2 id="archinstall">
  <a href="/en/linux/archinstall.html">archinstall</a> <a href="#archinstall"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Guided Arch Linux installer with a twist.
> More information: <https://archinstall.readthedocs.io>.

#### Start the interactive installer:
```shell
archinstall
```
#### Start a preset installer:
```shell
archinstall {{minimal|unattended}}
```
{% endraw %}{% raw %}
<h2 id="archlinux-java">
  <a href="/en/linux/archlinux-java.html">archlinux-java</a> <a href="#archlinux-java"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A helper script that provides functionalities for Java environments.
> More information: <https://github.com/michaellass/archlinux-java-run>.

#### List installed Java environments:
```shell
archlinux-java status
```
#### Set the default Java environment:
```shell
archlinux-java set {{java_environment}}
```
#### Unset the default Java environment:
```shell
archlinux-java unset
```
#### Set the default Java environment automatically:
```shell
archlinux-java fix
```
{% endraw %}{% raw %}
<h2 id="arecord">
  <a href="/en/linux/arecord.html">arecord</a> <a href="#arecord"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sound recorder for ALSA soundcard driver.
> More information: <https://manned.org/arecord>.

#### Record a snippet in "CD" quality (finish with Ctrl-C when done):
```shell
arecord -vv --format=cd {{path/to/file.wav}}
```
#### Record a snippet in "CD" quality, with a fixed duration of 10 seconds:
```shell
arecord -vv --format=cd --duration={{10}} {{path/to/file.wav}}
```
#### Record a snippet and save it as mp3 (finish with Ctrl-C when done):
```shell
arecord -vv --format=cd --file-type raw | lame -r - {{path/to/file.mp3}}
```
#### List all sound cards and digital audio devices:
```shell
arecord --list-devices
```
#### Allow interactive interface (e.g. use space-bar or enter to play or pause):
```shell
arecord --interactive
```
{% endraw %}{% raw %}
<h2 id="arithmetic">
  <a href="/en/linux/arithmetic.html">arithmetic</a> <a href="#arithmetic"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Quiz on simple arithmetic problems.
> More information: <https://manpages.debian.org/bsdgames/arithmetic.6.en.html>.

#### Start an arithmetic quiz:
```shell
arithmetic
```
#### Specify one or more arithmetic [o]peration symbols to get problems on them:
```shell
arithmetic -o {{+|-|x|/}}
```
#### Specify a range. Addition and multiplication problems would feature numbers between 0 and range, inclusive. Subtraction and division problems would have required result and number to be operated on, between 0 and range:
```shell
arithmetic -r {{7}}
```
{% endraw %}{% raw %}
<h2 id="ark">
  <a href="/en/linux/ark.html">ark</a> <a href="#ark"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> KDE archiving tool.
> More information: <https://docs.kde.org/stable5/en/kdeutils/ark/>.

#### Extract an archive into the current directory:
```shell
ark --batch {{archive}}
```
#### Change extraction directory:
```shell
ark --batch --destination {{path/to/directory}} {{archive}}
```
#### Create an archive if it does not exist and add files to it:
```shell
ark --add-to {{archive}} {{file1}} {{file2}}
```
{% endraw %}{% raw %}
<h2 id="arp-scan">
  <a href="/en/linux/arp-scan.html">arp-scan</a> <a href="#arp-scan"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Send ARP packets to hosts (specified as IP addresses or hostnames) to scan the local network.

#### Scan the current local network:
```shell
arp-scan --localnet
```
#### Scan an IP network with a custom bitmask:
```shell
arp-scan {{192.168.1.1}}/{{24}}
```
#### Scan an IP network within a custom range:
```shell
arp-scan {{127.0.0.0}}-{{127.0.0.31}}
```
#### Scan an IP network with a custom net mask:
```shell
arp-scan {{10.0.0.0}}:{{255.255.255.0}}
```
{% endraw %}{% raw %}
<h2 id="as">
  <a href="/en/linux/as.html">as</a> <a href="#as"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Portable GNU assembler.
> Primarily intended to assemble output from `gcc` to be used by `ld`.

#### Assemble a file, writing the output to `a.out`:
```shell
as {{file.s}}
```
#### Assemble the output to a given file:
```shell
as {{file.s}} -o {{out.o}}
```
#### Generate output faster by skipping whitespace and comment preprocessing. (Should only be used for trusted compilers):
```shell
as -f {{file.s}}
```
#### Include a given path to the list of directories to search for files specified in `.include` directives:
```shell
as -I {{path/to/directory}} {{file.s}}
```
{% endraw %}{% raw %}
<h2 id="ascii">
  <a href="/en/linux/ascii.html">ascii</a> <a href="#ascii"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show ASCII character aliases.
> More information: <http://www.catb.org/~esr/ascii/>.

#### Show ASCII aliases of a character:
```shell
ascii {{a}}
```
#### Show ASCII aliases in short, script-friendly mode:
```shell
ascii -t {{a}}
```
#### Show ASCII aliases of multiple characters:
```shell
ascii -s {{tldr}}
```
#### Show ASCII table in decimal:
```shell
ascii -d
```
#### Show ASCII table in hexadecimal:
```shell
ascii -x
```
#### Show ASCII table in octal:
```shell
ascii -o
```
#### Show ASCII table in binary:
```shell
ascii -b
```
#### Show options summary and complete ASCII table:
```shell
ascii
```
{% endraw %}{% raw %}
<h2 id="asciiart">
  <a href="/en/linux/asciiart.html">asciiart</a> <a href="#asciiart"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Convert images to ASCII.
> More information: <https://github.com/nodanaonlyzuul/asciiart>.

#### Read an image from a file and print in ASCII:
```shell
asciiart {{path/to/image.jpg}}
```
#### Read an image from a URL and print in ASCII:
```shell
asciiart {{www.example.com/image.jpg}}
```
#### Choose the output width (default is 100):
```shell
asciiart -width {{50}} {{path/to/image.jpg}}
```
#### Colorize the ASCII output:
```shell
asciiart --color {{path/to/image.jpg}}
```
#### Choose the output format (default format is text):
```shell
asciiart --format {{text|html}} {{path/to/image.jpg}}
```
#### Invert the character map:
```shell
asciiart --invert-chars {{path/to/image.jpg}}
```
{% endraw %}{% raw %}
<h2 id="aspell">
  <a href="/en/linux/aspell.html">aspell</a> <a href="#aspell"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interactive spell checker.

#### Spell check a single file:
```shell
aspell check {{path/to/file}}
```
#### List misspelled words from standard input:
```shell
cat {{file}} | aspell list
```
#### Show available dictionary languages:
```shell
aspell dicts
```
#### Run aspell with different language (takes two letter ISO 639 language code):
```shell
aspell --lang={{cs}}
```
#### List misspelled words from standard input and ignore words from personal word list:
```shell
cat {{file}} | aspell --personal={{personal-word-list.pws}} {{list}}
```
{% endraw %}{% raw %}
<h2 id="asterisk">
  <a href="/en/linux/asterisk.html">asterisk</a> <a href="#asterisk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Telephone and exchange (phone) server.
> Used for running the server itself, and managing an already running instance.
> More information: <https://wiki.asterisk.org/wiki/display/AST/Home>.

#### [R]econnect to a running server, and turn on logging 3 levels of [v]erbosity:
```shell
asterisk -r -vvv
```
#### [R]econnect to a running server, run a single command, and return:
```shell
asterisk -r -x "{{command}}"
```
#### Show chan_SIP clients (phones):
```shell
asterisk -r -x "sip show peers"
```
#### Show active calls and channels:
```shell
asterisk -r -x "core show channels"
```
#### Show voicemail mailboxes:
```shell
asterisk -r -x "voicemail show users"
```
#### Terminate a channel:
```shell
asterisk -r -x "hangup request {{channel_ID}}"
```
#### Reload chan_SIP configuration:
```shell
asterisk -r -x "sip reload"
```
{% endraw %}{% raw %}
<h2 id="at">
  <a href="/en/linux/at.html">at</a> <a href="#at"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Executes commands at a specified time.
> More information: <https://man.archlinux.org/man/at.1>.

#### Open an `at` prompt to create a new set of scheduled commands, press `Ctrl + D` to save and exit:
```shell
at {{hh:mm}}
```
#### Execute the commands and email the result using a local mailing program such as sendmail:
```shell
at {{hh:mm}} -m
```
#### Execute a script at the given time:
```shell
at {{hh:mm}} -f {{path/to/file}}
```
#### Display a system notification at 11pm on February 18th:
```shell
echo "notify-send '{{Wake up!}}'" | at {{11pm}} {{Feb 18}}
```
{% endraw %}{% raw %}
<h2 id="auracle">
  <a href="/en/linux/auracle.html">auracle</a> <a href="#auracle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line tool used to interact with Arch Linux's User Repository, commonly referred to as the AUR.
> More information: <https://github.com/falconindy/auracle>.

#### Display AUR packages that match a regular expression:
```shell
auracle search '{{regular_expression}}'
```
#### Display package information for a space-separated list of AUR packages:
```shell
auracle info {{package1}} {{package2}}
```
#### Display the `PKGBUILD` file (build information) for a space-separated list of AUR packages:
```shell
auracle show {{package1}} {{package2}}
```
#### Display updates for installed AUR packages:
```shell
auracle outdated
```
{% endraw %}{% raw %}
<h2 id="aurman">
  <a href="/en/linux/aurman.html">aurman</a> <a href="#aurman"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An Arch Linux utility to build and install packages from the Arch User Repository.
> See also `pacman`.
> More information: <https://github.com/polygamma/aurman>.

#### Synchronize and update all packages:
```shell
aurman --sync --refresh --sysupgrade
```
#### Synchronize and update all packages without show changes of `PKGBUILD` files:
```shell
aurman --sync --refresh --sysupgrade --noedit
```
#### Install a new package:
```shell
aurman --sync {{package_name}}
```
#### Install a new package without show changes of `PKGBUILD` files:
```shell
aurman --sync --noedit {{package_name}}
```
#### Install a new package without prompting:
```shell
aurman --sync --noedit --noconfirm {{package_name}}
```
#### Search the package database for a keyword from the official repositories and AUR:
```shell
aurman --sync --search {{keyword}}
```
#### Remove a package and its dependencies:
```shell
aurman --remove --recursive --nosave {{package_name}}
```
#### Clear the package cache (use two `--clean` flags to clean all packages):
```shell
aurman --sync --clean
```
{% endraw %}{% raw %}
<h2 id="authconfig">
  <a href="/en/linux/authconfig.html">authconfig</a> <a href="#authconfig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A CLI interface for configuring system authentication resources.

#### Display the current configuration (or dry run):
```shell
authconfig --test
```
#### Configure the server to use a different password hashing algorithm:
```shell
authconfig --update --passalgo={{algorithm}}
```
#### Enable LDAP authentication:
```shell
authconfig --update --enableldapauth
```
#### Disable LDAP authentication:
```shell
authconfig --update --disableldapauth
```
#### Enable Network Information Service (NIS):
```shell
authconfig --update --enablenis
```
#### Enable Kerberos:
```shell
authconfig --update --enablekrb5
```
#### Enable Winbind (Active Directory) authentication:
```shell
authconfig --update --enablewinbindauth
```
#### Enable local authorization:
```shell
authconfig --update --enablelocauthorize
```
{% endraw %}{% raw %}
<h2 id="autorandr">
  <a href="/en/linux/autorandr.html">autorandr</a> <a href="#autorandr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Automatically change screen layout.

#### Save the current screen layout:
```shell
autorandr -s {{profile_name}}
```
#### Show the saved profiles:
```shell
autorandr
```
#### Change the profile:
```shell
autorandr -l {{profile_name}}
```
#### Set the default profile:
```shell
autorandr -d {{profile_name}}
```
{% endraw %}{% raw %}
<h2 id="avahi-browse">
  <a href="/en/linux/avahi-browse.html">avahi-browse</a> <a href="#avahi-browse"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Displays services and hosts exposed on the local network via mDNS/DNS-SD.
> Avahi is compatible with Bonjour (Zeroconf) found in Apple devices.
> More information: <https://www.avahi.org/>.

#### List all services available on the local network along with their addresses and ports while ignoring local ones:
```shell
avahi-browse --all --resolve --ignore-local
```
#### List all domains:
```shell
avahi-browse --browse-domains
```
#### Limit the search to a particular domain:
```shell
avahi-browse --all --domain={{domain}}
```
{% endraw %}{% raw %}
<h2 id="balooctl">
  <a href="/en/linux/balooctl.html">balooctl</a> <a href="#balooctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> File indexing and searching framework for KDE Plasma.
> More information: <https://wiki.archlinux.org/index.php/Baloo>.

#### Display help:
```shell
balooctl
```
#### Display the status of the indexer:
```shell
balooctl status
```
#### Enable/Disable the file indexer:
```shell
balooctl {{enable|disable}}
```
#### Clean the index database:
```shell
balooctl purge
```
#### Suspend the file indexer:
```shell
balooctl suspend
```
#### Resume the file indexer:
```shell
balooctl resume
```
#### Display the disk space used by Baloo:
```shell
balooctl indexSize
```
#### Check for any unindexed files and index them:
```shell
balooctl check
```
{% endraw %}{% raw %}
<h2 id="beep">
  <a href="/en/linux/beep.html">beep</a> <a href="#beep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A utility to beep the PC speaker.

#### Play a beep:
```shell
beep
```
#### Play a beep that repeats:
```shell
beep -r {{repetitions}}
```
#### Play a beep at a specified frequency (Hz) and duration (milliseconds):
```shell
beep -f {{frequency}} -l {{duration}}
```
#### Play each new frequency and duration as a distinct beep:
```shell
beep -f {{frequency}} -l {{duration}} -n -f {{frequency}} -l {{duration}}
```
#### Play the C major scale:
```shell
beep -f 262 -n -f 294 -n -f 330 -n -f 349 -n -f 392 -n -f 440 -n -f 494 -n -f 523
```
{% endraw %}{% raw %}
<h2 id="betterlockscreen">
  <a href="/en/linux/betterlockscreen.html">betterlockscreen</a> <a href="#betterlockscreen"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Simple, minimal lock screen.

#### Lock the screen:
```shell
betterlockscreen --lock
```
#### Change the lock screen background:
```shell
betterlockscreen -u {{path/to/image.png}}
```
#### Lock the screen, showing some custom text:
```shell
betterlockscreen -l pixel -t "{{custom lock screen text}}"
```
#### Lock the screen, with a custom monitor off timeout in seconds:
```shell
betterlockscreen --off {{5}} -l
```
{% endraw %}{% raw %}
<h2 id="binwalk">
  <a href="/en/linux/binwalk.html">binwalk</a> <a href="#binwalk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Firmware Analysis Tool.
> More information: <https://github.com/ReFirmLabs/binwalk>.

#### Scan a binary file:
```shell
binwalk {{path/to/binary}}
```
#### Extract files from a binary, specifying the output directory:
```shell
binwalk --extract --directory {{output_directory}} {{path/to/binary}}
```
#### Recursively extract files from a binary limiting the recursion depth to 2:
```shell
binwalk --extract --matryoshka --depth {{2}} {{path/to/binary}}
```
#### Extract files from a binary with the specified file signature:
```shell
binwalk --dd '{{png image:png}}' {{path/to/binary}}
```
#### Analyze the entropy of a binary, saving the plot with the same name as the binary and `.png` extension appended:
```shell
binwalk --entropy --save {{path/to/binary}}
```
#### Combine entropy, signature and opcodes analysis in a single command:
```shell
binwalk --entropy --signature --opcodes {{path/to/binary}}
```
{% endraw %}{% raw %}
<h2 id="bitwise">
  <a href="/en/linux/bitwise.html">bitwise</a> <a href="#bitwise"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Multi base interactive calculator supporting dynamic base conversion and bit manipulation.
> More information: <https://github.com/mellowcandle/bitwise>.

#### Run using interactive mode:
```shell
bitwise
```
#### Convert from decimal:
```shell
bitwise {{12345}}
```
#### Convert from hexadecimal:
```shell
bitwise {{0x563d}}
```
#### Convert a C-style calculation:
```shell
bitwise "{{0x123 + 0x20 - 30 / 50}}"
```
{% endraw %}{% raw %}
<h2 id="blkdiscard">
  <a href="/en/linux/blkdiscard.html">blkdiscard</a> <a href="#blkdiscard"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Discards device sectors on storage devices. Useful for SSDs.

#### Discard all sectors on a device, removing all data:
```shell
blkdiscard /dev/{{device}}
```
#### Securely discard all blocks on a device, removing all data:
```shell
blkdiscard --secure /dev/{{device}}
```
#### Discard the first 100MB of a device:
```shell
blkdiscard --length {{100MB}} /dev/{{device}}
```
{% endraw %}{% raw %}
<h2 id="blkid">
  <a href="/en/linux/blkid.html">blkid</a> <a href="#blkid"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lists all recognized partitions and their Universally Unique Identifier (UUID).

#### List all partitions:
```shell
sudo blkid
```
#### List all partitions in a table, including current mountpoints:
```shell
sudo blkid -o list
```
{% endraw %}{% raw %}
<h2 id="bluetoothctl">
  <a href="/en/linux/bluetoothctl.html">bluetoothctl</a> <a href="#bluetoothctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Handling bluetooth devices from the shell.

#### Enter the bluetoothctl shell:
```shell
bluetoothctl
```
#### List devices:
```shell
bluetoothctl -- devices
```
#### Pair a device:
```shell
bluetoothctl -- pair {{mac_address}}
```
#### Remove a device:
```shell
bluetoothctl -- remove {{mac_address}}
```
#### Connect a paired device:
```shell
bluetoothctl -- connect {{mac_address}}
```
#### Disconnect a paired device:
```shell
bluetoothctl -- disconnect {{mac_address}}
```
{% endraw %}{% raw %}
<h2 id="bmon">
  <a href="/en/linux/bmon.html">bmon</a> <a href="#bmon"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Monitor bandwidth and capture network related statistics.

#### Display the list of all the interfaces:
```shell
bmon -a
```
#### Display data transfer rates in bits per second:
```shell
bmon -b
```
#### Set policy to define which network interface(s) is/are displayed:
```shell
bmon -p {{interface_1,interface_2,interface_3}}
```
#### Set interval (in seconds) in which rate per counter is calculated:
```shell
bmon -R {{2.0}}
```
{% endraw %}{% raw %}
<h2 id="boltctl">
  <a href="/en/linux/boltctl.html">boltctl</a> <a href="#boltctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Control thunderbolt devices.
> More information: <https://manned.org/boltctl>.

#### List connected (and authorized) devices:
```shell
boltctl
```
#### List connected devices, including unauthorized ones:
```shell
boltctl list
```
#### Authorize a device temporarily:
```shell
boltctl authorize {{device_uuid}}
```
#### Authorize and remember a device:
```shell
boltctl enroll {{device_uuid}}
```
#### Revoke a previously authorized device:
```shell
boltctl forget {{device_uuid}}
```
#### Show more information about a device:
```shell
boltctl info {{device_uuid}}
```
{% endraw %}{% raw %}
<h2 id="bpftrace">
  <a href="/en/linux/bpftrace.html">bpftrace</a> <a href="#bpftrace"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> High-level tracing language for Linux eBPF.
> More information: <https://github.com/iovisor/bpftrace>.

#### Display bpftrace version:
```shell
bpftrace -V
```
#### List all available probes:
```shell
sudo bpftrace -l
```
#### Run a one-liner program (e.g syscall count by program):
```shell
sudo bpftrace -e '{{tracepoint:raw_syscalls:sys_enter { @[comm] = count(); }}}'
```
#### Run a program from a file:
```shell
sudo bpftrace {{path/to/file}}
```
#### Trace a program by PID:
```shell
sudo bpftrace -e '{{tracepoint:raw_syscalls:sys_enter /pid == 123/ { @[comm] = count(); }}}'
```
#### Do a dry run and display the output in eBPF format:
```shell
sudo bpftrace -d -e '{{one_line_program}}'
```
{% endraw %}{% raw %}
<h2 id="bpytop">
  <a href="/en/linux/bpytop.html">bpytop</a> <a href="#bpytop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display dynamic real-time information about running processes with graphs. Similar to `gtop` and `htop`.
> More information: <https://github.com/aristocratos/bpytop>.

#### Start bpytop:
```shell
bpytop
```
#### Start in minimal mode without memory and networking boxes:
```shell
bpytop -m
```
#### Show version:
```shell
bpytop -v
```
#### Toggle minimal mode:
```shell
m
```
#### Search for running programs or processes:
```shell
f
```
#### Change settings:
```shell
M
```
{% endraw %}{% raw %}
<h2 id="brctl">
  <a href="/en/linux/brctl.html">brctl</a> <a href="#brctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ethernet bridge administration.

#### Show a list with information about currently existing ethernet bridges:
```shell
sudo brctl show
```
#### Create a new ethernet bridge interface:
```shell
sudo brctl add {{bridge_name}}
```
#### Delete an existing ethernet bridge interface:
```shell
sudo brctl del {{bridge_name}}
```
#### Add an interface to an existing bridge:
```shell
sudo brctl addif {{bridge_name}} {{interface_name}}
```
#### Remove an interface from an existing bridge:
```shell
sudo brctl delif {{bridge_name}} {{interface_name}}
```
{% endraw %}{% raw %}
<h2 id="btrfs-device">
  <a href="/en/linux/btrfs-device.html">btrfs device</a> <a href="#btrfs-device"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage devices in a btrfs filesystem.
> More information: <https://btrfs.wiki.kernel.org/index.php/Manpage/btrfs-device>.

#### Add one or more devices to a btrfs filesystem:
```shell
sudo btrfs device add {{path/to/block_device1}} [{{path/to/block_device2}}] {{path/to/btrfs_filesystem}}
```
#### Remove a device from a btrfs filesystem:
```shell
sudo btrfs device remove {{path/to/device|device_id}} [{{...}}]
```
#### Display error statistics:
```shell
sudo btrfs device stats {{path/to/btrfs_filesystem}}
```
#### Scan all disks and inform the kernel of all detected btrfs filesystems:
```shell
sudo btrfs device scan --all-devices
```
#### Display detailed per-disk allocation statistics:
```shell
sudo btrfs device usage {{path/to/btrfs_filesystem}}
```
{% endraw %}{% raw %}
<h2 id="btrfs-filesystem">
  <a href="/en/linux/btrfs-filesystem.html">btrfs filesystem</a> <a href="#btrfs-filesystem"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage btrfs filesystems.
> More information: <https://btrfs.wiki.kernel.org/index.php/Manpage/btrfs-filesystem>.

#### Show filesystem usage (optionally run as root to show detailed information):
```shell
btrfs filesystem usage {{path/to/btrfs_mount}}
```
#### Show usage by individual devices:
```shell
sudo btrfs filesystem show {{path/to/btrfs_mount}}
```
#### Defragment a single file on a btrfs filesystem (avoid while a deduplication agent is running):
```shell
sudo btrfs filesystem defragment -v {{path/to/file}}
```
#### Defragment a directory recursively (does not cross subvolume boundaries):
```shell
sudo btrfs filesystem defragment -v -r {{path/to/directory}}
```
#### Force syncing unwritten data blocks to disk(s):
```shell
sudo btrfs filesystem sync {{path/to/btrfs_mount}}
```
#### Summarize disk usage for the files in a directory recursively:
```shell
sudo btrfs filesystem du --summarize {{path/to/directory}}
```
{% endraw %}{% raw %}
<h2 id="btrfs-scrub">
  <a href="/en/linux/btrfs-scrub.html">btrfs scrub</a> <a href="#btrfs-scrub"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Scrub btrfs filesystems to verify data integrity.
> It is recommended to run a scrub once a month.
> More information: <https://btrfs.wiki.kernel.org/index.php/Manpage/btrfs-scrub>.

#### Start a scrub:
```shell
sudo btrfs scrub start {{path/to/btrfs_mount}}
```
#### Show the status of an ongoing or last completed scrub:
```shell
sudo btrfs scrub status {{path/to/btrfs_mount}}
```
#### Cancel an ongoing scrub:
```shell
sudo btrfs scrub cancel {{path/to/btrfs_mount}}
```
#### Resume a previously cancelled scrub:
```shell
sudo btrfs scrub resume {{path/to/btrfs_mount}}
```
#### Start a scrub, but wait until the scrub finishes before exiting:
```shell
sudo btrfs scrub start -B {{path/to/btrfs_mount}}
```
#### Start a scrub in quiet mode (does not print errors or statistics):
```shell
sudo btrfs scrub start -q {{path/to/btrfs_mount}}
```
{% endraw %}{% raw %}
<h2 id="btrfs-subvolume">
  <a href="/en/linux/btrfs-subvolume.html">btrfs subvolume</a> <a href="#btrfs-subvolume"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage btrfs subvolumes and snapshots.
> More information: <https://btrfs.wiki.kernel.org/index.php/Manpage/btrfs-subvolume>.

#### Create a new empty subvolume:
```shell
sudo btrfs subvolume create {{path/to/new_subvolume}}
```
#### List all subvolumes and snapshots in the specified filesystem:
```shell
sudo btrfs subvolume list {{path/to/btrfs_filesystem}}
```
#### Delete a subvolume:
```shell
sudo btrfs subvolume delete {{path/to/subvolume}}
```
#### Create a read-only snapshot of an existing subvolume:
```shell
sudo btrfs subvolume snapshot -r {{path/to/source_subvolume}} {{path/to/target}}
```
#### Create a read-write snapshot of an existing subvolume:
```shell
sudo btrfs subvolume snapshot {{path/to/source_subvolume}} {{path/to/target}}
```
#### Show detailed information about a subvolume:
```shell
sudo btrfs subvolume show {{path/to/subvolume}}
```
{% endraw %}{% raw %}
<h2 id="btrfs">
  <a href="/en/linux/btrfs.html">btrfs</a> <a href="#btrfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A filesystem based on the copy-on-write (COW) principle for Linux.

#### Create subvolume:
```shell
sudo btrfs subvolume create {{path/to/subvolume}}
```
#### List subvolumes:
```shell
sudo btrfs subvolume list {{path/to/mount_point}}
```
#### Show space usage information:
```shell
sudo btrfs filesystem df {{path/to/mount_point}}
```
#### Enable quota:
```shell
sudo btrfs quota enable {{path/to/subvolume}}
```
#### Show quota:
```shell
sudo btrfs qgroup show {{path/to/subvolume}}
```
{% endraw %}{% raw %}
<h2 id="cal">
  <a href="/en/linux/cal.html">cal</a> <a href="#cal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Prints calendar information, with the current day highlighted.

#### Display a calendar for the current month:
```shell
cal
```
#### Display previous, current and next month:
```shell
cal -3
```
#### Use monday as the first day of the week:
```shell
cal --monday
```
#### Display a calendar for a specific year (4 digits):
```shell
cal {{year}}
```
#### Display a calendar for a specific month and year:
```shell
cal {{month}} {{year}}
```
{% endraw %}{% raw %}
<h2 id="calc">
  <a href="/en/linux/calc.html">calc</a> <a href="#calc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An interactive arbitrary-precision calculator on the terminal.

#### Start calc in interactive mode:
```shell
calc
```
#### Perform a calculation in non-interactive mode:
```shell
calc -p '{{85 * (36 / 4)}}'
```
{% endraw %}{% raw %}
<h2 id="calcurse">
  <a href="/en/linux/calcurse.html">calcurse</a> <a href="#calcurse"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A text-based calendar and scheduling application for the command-line.
> More information: <https://calcurse.org>.

#### Start calcurse on interactive mode:
```shell
calcurse
```
#### Print the appointments and events for the current day and exit:
```shell
calcurse --appointment
```
#### Remove all local calcurse items and import remote objects:
```shell
calcurse-caldav --init=keep-remote
```
#### Remove all remote objects and push local calcurse items:
```shell
calcurse-caldav --init=keep-local
```
#### Copy local objects to the CalDAV server and vice versa:
```shell
calcurse-caldav --init=two-way
```
{% endraw %}{% raw %}
<h2 id="ceph">
  <a href="/en/linux/ceph.html">ceph</a> <a href="#ceph"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A unified storage system.
> More information: <https://ceph.io>.

#### Check cluster health status:
```shell
ceph status
```
#### Check cluster usage stats:
```shell
ceph df
```
#### Get the statistics for the placement groups in a cluster:
```shell
ceph pg dump --format {{plain}}
```
#### Create a storage pool:
```shell
ceph osd pool create {{pool_name}} {{page_number}}
```
#### Delete a storage pool:
```shell
ceph osd pool delete {{pool_name}}
```
#### Rename a storage pool:
```shell
ceph osd pool rename {{current_name}} {{new_name}}
```
#### Self-repair pool storage:
```shell
ceph pg repair {{pool_name}}
```
{% endraw %}{% raw %}
<h2 id="certbot">
  <a href="/en/linux/certbot.html">certbot</a> <a href="#certbot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Let's Encrypt Agent for automatically obtaining and renewing TLS certificates.
> Successor to `letsencrypt`.
> More information: <https://certbot.eff.org/docs/using.html>.

#### Obtain a new certificate via webroot authorization, but do not install it automatically:
```shell
sudo certbot certonly --webroot --webroot-path {{path/to/webroot}} --domain {{subdomain.example.com}}
```
#### Obtain a new certificate via nginx authorization, installing the new certificate automatically:
```shell
sudo certbot --nginx --domain {{subdomain.example.com}}
```
#### Obtain a new certificate via apache authorization, installing the new certificate automatically:
```shell
sudo certbot --apache --domain {{subdomain.example.com}}
```
#### Renew all Let's Encrypt certificates that expire in 30 days or less (don't forget to restart any servers that use them afterwards):
```shell
sudo certbot renew
```
#### Simulate the obtaining of a new certificate, but don't actually save any new certificates to disk:
```shell
sudo certbot --webroot --webroot-path {{path/to/webroot}} --domain {{subdomain.example.com}} --dry-run
```
#### Obtain an untrusted test certificate instead:
```shell
sudo certbot --webroot --webroot-path {{path/to/webroot}} --domain {{subdomain.example.com}} --test-cert
```
{% endraw %}{% raw %}
<h2 id="cewl">
  <a href="/en/linux/cewl.html">cewl</a> <a href="#cewl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> URL spidering tool for making a cracking wordlist from web content.
> More information: <https://digi.ninja/projects/cewl.php>.

#### Create a wordlist file from the given URL up to 2 links depth:
```shell
cewl --depth {{2}} --write {{path/to/wordlist.txt}} {{url}}
```
#### Output an alphanumeric wordlist from the given URL with words of minimum 5 characters:
```shell
cewl --with-numbers --min_word_length {{5}} {{url}}
```
#### Output a wordlist from the given URL in debug mode including email addresses:
```shell
cewl --debug --email {{url}}
```
#### Output a wordlist from the given URL using HTTP Basic or Digest authentication:
```shell
cewl --auth_type {{basic|digest}} --auth_user {{username}} --auth_pass {{password}} {{url}}
```
#### Output a wordlist from the given URL through a proxy:
```shell
cewl --proxy_host {{host}} --proxy_port {{port}} {{url}}
```
{% endraw %}{% raw %}
<h2 id="cfdisk">
  <a href="/en/linux/cfdisk.html">cfdisk</a> <a href="#cfdisk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A program for managing partition tables and partitions on a hard disk using a curses UI.
> More information: <https://manned.org/cfdisk>.

#### Start the partition manipulator with a specific device:
```shell
cfdisk {{/dev/sdX}}
```
#### Create a new partition table for a specific device and manage it:
```shell
cfdisk --zero {{/dev/sdX}}
```
{% endraw %}{% raw %}
<h2 id="chage">
  <a href="/en/linux/chage.html">chage</a> <a href="#chage"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Change user account and password expiry information.

#### List password information for the user:
```shell
chage -l {{username}}
```
#### Enable password expiration in 10 days:
```shell
sudo chage -M {{10}} {{username}}
```
#### Disable password expiration:
```shell
sudo chage -M -1 {{username}}
```
#### Set account expiration date:
```shell
sudo chage -E {{YYYY-MM-DD}}
```
#### Force user to change password on next log in:
```shell
sudo chage -d 0
```
{% endraw %}{% raw %}
<h2 id="chattr">
  <a href="/en/linux/chattr.html">chattr</a> <a href="#chattr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Change attributes of files or directories.

#### Make a file or directory immutable to changes and deletion, even by superuser:
```shell
chattr +i {{path/to/file_or_directory}}
```
#### Make a file or directory mutable:
```shell
chattr -i {{path/to/file_or_directory}}
```
#### Recursively make an entire directory and contents immutable:
```shell
chattr -R +i {{path/to/directory}}
```
{% endraw %}{% raw %}
<h2 id="chcpu">
  <a href="/en/linux/chcpu.html">chcpu</a> <a href="#chcpu"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Enable/disable a system's CPUs.

#### Disable CPUs via a list of CPU ID numbers:
```shell
chcpu -d {{1,3}}
```
#### Enable a set of CPUs via a range of CPU ID numbers:
```shell
chcpu -e {{1-10}}
```
{% endraw %}{% raw %}
<h2 id="check-support-status">
  <a href="/en/linux/check-support-status.html">check-support-status</a> <a href="#check-support-status"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Identify installed Debian packages for which support has had to be limited or prematurely ended.
> More information: <https://manpages.debian.org/buster/debian-security-support/check-support-status.1.en.html>.

#### Display packages whose support is limited, has already ended or will end earlier than the distribution's end of life:
```shell
check-support-status
```
#### Display only packages whose support has ended:
```shell
check-support-status --type {{ended}}
```
#### Skip printing a headline:
```shell
check-support-status --no-heading
```
{% endraw %}{% raw %}
<h2 id="chfn">
  <a href="/en/linux/chfn.html">chfn</a> <a href="#chfn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Update `finger` info for a user.

#### Update a user's "Name" field in the output of `finger`:
```shell
chfn -f {{new_display_name}} {{username}}
```
#### Update a user's "Office Room Number" field for the output of `finger`:
```shell
chfn -o {{new_office_room_number}} {{username}}
```
#### Update a user's "Office Phone Number" field for the output of `finger`:
```shell
chfn -p {{new_office_telephone_number}} {{username}}
```
#### Update a user's "Home Phone Number" field for the output of `finger`:
```shell
chfn -h {{new_home_telephone_number}} {{username}}
```
{% endraw %}{% raw %}
<h2 id="chkconfig">
  <a href="/en/linux/chkconfig.html">chkconfig</a> <a href="#chkconfig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage the runlevel of services on CentOS 6.

#### List services with runlevel:
```shell
chkconfig --list
```
#### Show a service's runlevel:
```shell
chkconfig --list {{ntpd}}
```
#### Enable service at boot:
```shell
chkconfig {{sshd}} on
```
#### Enable service at boot for runlevels 2, 3, 4, and 5:
```shell
chkconfig --level {{2345}} {{sshd}} on
```
#### Disable service at boot:
```shell
chkconfig {{ntpd}} off
```
#### Disable service at boot for runlevel 3:
```shell
chkconfig --level {{3}} {{ntpd}} off
```
{% endraw %}{% raw %}
<h2 id="chronyc">
  <a href="/en/linux/chronyc.html">chronyc</a> <a href="#chronyc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Query the Chrony NTP daemon.
> More information: <https://chrony.tuxfamily.org/doc/4.0/chronyc.html>.

#### Start chronyc in interactive mode:
```shell
chronyc
```
#### Display tracking stats for the Chrony daemon:
```shell
chronyc tracking
```
#### Print the time sources that Chrony is currently using:
```shell
chronyc sources
```
#### Display stats for sources currently used by chrony daemon as a time source:
```shell
chronyc sourcestats
```
#### Step the system clock immediately, bypassing any slewing:
```shell
chronyc makestep
```
#### Display verbose information about each NTP source:
```shell
chronyc ntpdata
```
{% endraw %}{% raw %}
<h2 id="chrt">
  <a href="/en/linux/chrt.html">chrt</a> <a href="#chrt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manipulate the real-time attributes of a process.
> More information: <https://man7.org/linux/man-pages/man1/chrt.1.html>.

#### Display attributes of a process:
```shell
chrt --pid {{PID}}
```
#### Display attributes of all threads of a process:
```shell
chrt --all-tasks --pid {{PID}}
```
#### Display the min/max priority values that can be used with `chrt`:
```shell
chrt --max
```
#### Set the scheduling policy for a process:
```shell
chrt --pid {{PID}} --{{deadline|idle|batch|rr|fifo|other}}
```
{% endraw %}{% raw %}
<h2 id="clamav">
  <a href="/en/linux/clamav.html">clamav</a> <a href="#clamav"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Open-source anti-virus program.
> Designed especially for e-mail scanning on mail gateways, but can be used in other contexts.
> More information: <https://www.clamav.net>.

#### Update virus definitions:
```shell
freshclam
```
#### Scan a file for viruses:
```shell
clamscan {{path/to/file}}
```
#### Scan directories recursively and print out infected files:
```shell
clamscan --recursive --infected {{path/to/directory}}
```
#### Scan directories recursively and move them into quarantine:
```shell
clamscan --recursive --move={{directory}}
```
{% endraw %}{% raw %}
<h2 id="cmus">
  <a href="/en/linux/cmus.html">cmus</a> <a href="#cmus"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line Music Player.
> Use arrow keys to navigate, `<enter/return>` to select, and numbers 1-8 switch between different views.

#### Open cmus into the specified directory (this will become your new working directory):
```shell
cmus {{path/to/directory}}
```
#### Add file/directory to library:
```shell
:add {{path/to/file_or_directory}}
```
#### Pause/unpause current song:
```shell
c
```
#### Toggle shuffle mode on/off:
```shell
s
```
#### Quit cmus:
```shell
q
```
{% endraw %}{% raw %}
<h2 id="collectd">
  <a href="/en/linux/collectd.html">collectd</a> <a href="#collectd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> System statistics collection daemon.
> More information: <https://collectd.org/>.

#### Show usage help, including the program version:
```shell
collectd -h
```
#### Test the configuration file and then exit:
```shell
collectd -t
```
#### Test plugin data collection functionality and then exit:
```shell
collectd -T
```
#### Start collectd:
```shell
collectd
```
#### Specify a custom configuration file location:
```shell
collectd -C {{path/to/file}}
```
#### Specify a custom PID file location:
```shell
collectd -P {{path/to/file}}
```
#### Don't fork into the background:
```shell
collectd -f
```
{% endraw %}{% raw %}
<h2 id="colrm">
  <a href="/en/linux/colrm.html">colrm</a> <a href="#colrm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remove columns from stdin.

#### Remove first column of stdin:
```shell
colrm {{1 1}}
```
#### Remove from 3rd column till the end of each line:
```shell
colrm {{3}}
```
#### Remove from the 3rd column till the 5th column of each line:
```shell
colrm {{3 5}}
```
{% endraw %}{% raw %}
<h2 id="compgen">
  <a href="/en/linux/compgen.html">compgen</a> <a href="#compgen"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A built-in command for auto-completion in bash, which is called on pressing TAB key twice.

#### List all commands that you could run:
```shell
compgen -c
```
#### List all aliases:
```shell
compgen -a
```
#### List all functions that you could run:
```shell
compgen -A function
```
#### Show shell reserved key words:
```shell
compgen -k
```
#### See all available commands/aliases starting with 'ls':
```shell
compgen -ac {{ls}}
```
{% endraw %}{% raw %}
<h2 id="compose">
  <a href="/en/linux/compose.html">compose</a> <a href="#compose"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An alias to a `run-mailcap`'s action compose.
> Originally `run-mailcap` is used to mime-type/file.

#### Compose action can be used to compose any existing file or new on default mailcap edit tool:
```shell
compose {{filename}}
```
#### With `run-mailcap`:
```shell
run-mailcap --action=compose {{filename}}
```
{% endraw %}{% raw %}
<h2 id="compsize">
  <a href="/en/linux/compsize.html">compsize</a> <a href="#compsize"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Calculate the compression ratio of a set of files on a btrfs filesystem.
> See also `btrfs filesystem` for recompressing a file by defragmenting it.
> More information: <https://github.com/kilobyte/compsize>.

#### Calculate the current compression ratio for a file or directory:
```shell
sudo compsize {{path/to/file_or_directory}}
```
#### Don't traverse filesystem boundaries:
```shell
sudo compsize --one-file-system {{path/to/file_or_directory}}
```
#### Show raw byte counts instead of human-readable sizes:
```shell
sudo compsize --bytes {{path/to/file_or_directory}}
```
{% endraw %}{% raw %}
<h2 id="conky">
  <a href="/en/linux/conky.html">conky</a> <a href="#conky"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Light-weight system monitor for X.
> More information: <https://github.com/brndnmtthws/conky>.

#### Launch with default, built-in config:
```shell
conky
```
#### Create a new default config:
```shell
conky -C > ~/.conkyrc
```
#### Launch conky with a given config file:
```shell
conky -c {{path/to/config}}
```
#### Start in the background (daemonize):
```shell
conky -d
```
#### Align conky on the desktop:
```shell
conky -a {{{top,bottom,middle}_{left,right,middle}}}
```
#### Pause for 5 seconds at startup before launching:
```shell
conky -p {{5}}
```
{% endraw %}{% raw %}
<h2 id="coredumpctl">
  <a href="/en/linux/coredumpctl.html">coredumpctl</a> <a href="#coredumpctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Retrieve and process saved core dumps and metadata.
> More information: <https://www.freedesktop.org/software/systemd/man/coredumpctl.html>.

#### List all captured core dumps:
```shell
coredumpctl list
```
#### List captured core dumps for a program:
```shell
coredumpctl list {{program}}
```
#### Show information about the core dumps matching a program with `PID`:
```shell
coredumpctl info {{PID}}
```
#### Invoke debugger using the last core dump of a program:
```shell
coredumpctl debug {{program}}
```
#### Extract the last core dump of a program to a file:
```shell
coredumpctl --output={{path/to/file}} dump {{program}}
```
{% endraw %}{% raw %}
<h2 id="cp">
  <a href="/en/linux/cp.html">cp</a> <a href="#cp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Copy files and directories.
> More information: <https://www.gnu.org/software/coreutils/cp>.

#### Copy a file to another location:
```shell
cp {{path/to/source_file.ext}} {{path/to/target_file.ext}}
```
#### Copy a file into another directory, keeping the filename:
```shell
cp {{path/to/source_file.ext}} {{path/to/target_parent_directory}}
```
#### Recursively copy a directory's contents to another location (if the destination exists, the directory is copied inside it):
```shell
cp -r {{path/to/source_directory}} {{path/to/target_directory}}
```
#### Copy a directory recursively, in verbose mode (shows files as they are copied):
```shell
cp -vr {{path/to/source_directory}} {{path/to/target_directory}}
```
#### Copy text files to another location, in interactive mode (prompts user before overwriting):
```shell
cp -i {{*.txt}} {{path/to/target_directory}}
```
#### Follow symbolic links before copying:
```shell
cp -L {{link}} {{path/to/target_directory}}
```
#### Use the full path of source files, creating any missing intermediate directories when copying:
```shell
cp --parents {{source/path/to/file}} {{path/to/target_file}}
```
{% endraw %}{% raw %}
<h2 id="cpufreq-aperf">
  <a href="/en/linux/cpufreq-aperf.html">cpufreq-aperf</a> <a href="#cpufreq-aperf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Calculate the average CPU frequency over a time period.
> Requires root privileges.

#### Start calculating, defaulting to all CPU cores and 1 second refresh interval:
```shell
sudo cpufreq-aperf
```
#### Start calculating for CPU 1 only:
```shell
sudo cpufreq-aperf -c {{1}}
```
#### Start calculating with a 3 seconds refresh interval for all CPU cores:
```shell
sudo cpufreq-aperf -i {{3}}
```
#### Calculate only once:
```shell
sudo cpufreq-aperf -o
```
{% endraw %}{% raw %}
<h2 id="cpufreq-info">
  <a href="/en/linux/cpufreq-info.html">cpufreq-info</a> <a href="#cpufreq-info"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool to show CPU frequency information.

#### Show CPU frequency information for all CPUs:
```shell
cpufreq-info
```
#### Show CPU frequency information for the specified CPU:
```shell
cpufreq-info -c {{cpu_number}}
```
#### Show the allowed minimum and maximum CPU frequency:
```shell
cpufreq-info -l
```
#### Show the current minimum and maximum CPU frequency and policy in table format:
```shell
cpufreq-info -o
```
#### Show available CPU frequency policies:
```shell
cpufreq-info -g
```
#### Show current CPU work frequency in a human-readable format, according to the cpufreq kernel module:
```shell
cpufreq-info -f -m
```
#### Show current CPU work frequency in a human-readable format, by reading it from hardware (only available to root):
```shell
sudo cpufreq-info -w -m
```
{% endraw %}{% raw %}
<h2 id="cpufreq-set">
  <a href="/en/linux/cpufreq-set.html">cpufreq-set</a> <a href="#cpufreq-set"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool to modify CPU frequency settings.
> The frequency value should range between the output of command `cpufreq-info -l`.

#### Set the CPU frequency policy of CPU 1 to "userspace":
```shell
sudo cpufreq-set -c {{1}} -g {{userspace}}
```
#### Set the current minimum CPU frequency of CPU 1:
```shell
sudo cpufreq-set -c {{1}} --min {{min_frequency}}
```
#### Set the current maximum CPU frequency of CPU 1:
```shell
sudo cpufreq-set -c {{1}} --max {{max_frequency}}
```
#### Set the current work frequency of CPU 1:
```shell
sudo cpufreq-set -c {{1}} -f {{work_frequency}}
```
{% endraw %}{% raw %}
<h2 id="cpuid">
  <a href="/en/linux/cpuid.html">cpuid</a> <a href="#cpuid"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display detailed information about all CPUs.

#### Display information for all CPUs:
```shell
cpuid
```
#### Display information only for the current CPU:
```shell
cpuid -1
```
#### Display raw hex information with no decoding:
```shell
cpuid -r
```
{% endraw %}{% raw %}
<h2 id="cpulimit">
  <a href="/en/linux/cpulimit.html">cpulimit</a> <a href="#cpulimit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool to throttle the CPU usage of other processes.
> More information: <http://cpulimit.sourceforge.net/>.

#### Limit an existing process with PID 1234 to only use 25% of the CPU:
```shell
cpulimit --pid {{1234}} --limit {{25%}}
```
#### Limit an existing program by its executable name:
```shell
cpulimit --exe {{program}} --limit {{25}}
```
#### Launch a given program and limit it to only use 50% of the CPU:
```shell
cpulimit --limit {{50}} -- {{program arg1 arg2 ...}}
```
#### Launch a program, limit its CPU usage to 50% and run cpulimit in the background:
```shell
cpulimit --limit {{50}} --background -- {{program}}
```
#### Kill its process if the program's CPU usage goes over 50%:
```shell
cpulimit --limit 50 --kill -- {{program}}
```
#### Throttle both it and its child processes so that none go about 25% CPU:
```shell
cpulimit --limit {{25}} --monitor-forks -- {{program}}
```
{% endraw %}{% raw %}
<h2 id="create_ap">
  <a href="/en/linux/create_ap.html">create_ap</a> <a href="#create_ap"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create an AP (Access Point) at any channel.

#### Create an open network with no passphrase:
```shell
create_ap {{wlan0}} {{eth0}} {{access_point_ssid}}
```
#### Use a WPA + WPA2 passphrase:
```shell
create_ap {{wlan0}} {{eth0}} {{access_point_ssid}} {{passphrase}}
```
#### Create an access point without Internet sharing:
```shell
create_ap -n {{wlan0}} {{acces_point_ssid}} {{passphrase}}
```
#### Create a bridged network with Internet sharing:
```shell
create_ap -m bridge {{wlan0}} {{eth0}} {{access_point_ssid}} {{passphrase}}
```
#### Create a bridged network with Internet sharing and a pre-configured bridge interface:
```shell
create_ap -m bridge {{wlan0}} {{br0}} {{access_point_ssid}} {{passphrase}}
```
#### Create an access port for Internet sharing from the same WiFi interface:
```shell
create_ap {{wlan0}} {{wlan0}} {{access_point_ssid}} {{passphrase}}
```
#### Choose a different WiFi adapter driver:
```shell
create_ap --driver {{wifi_adapter}} {{wlan0}} {{eth0}} {{access_point_ssid}} {{passphrase}}
```
{% endraw %}{% raw %}
<h2 id="cryptsetup">
  <a href="/en/linux/cryptsetup.html">cryptsetup</a> <a href="#cryptsetup"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage plain dm-crypt and LUKS (Linux Unified Key Setup) encrypted volumes.

#### Initialize a LUKS volume (overwrites all data on the partition):
```shell
cryptsetup luksFormat {{/dev/sda1}}
```
#### Open a LUKS volume and create a decrypted mapping at `/dev/mapper/{{target}}`:
```shell
cryptsetup luksOpen {{/dev/sda1}} {{target}}
```
#### Remove an existing mapping:
```shell
cryptsetup luksClose {{target}}
```
#### Change the LUKS volume's passphrase:
```shell
cryptsetup luksChangeKey {{/dev/sda1}}
```
{% endraw %}{% raw %}
<h2 id="csplit">
  <a href="/en/linux/csplit.html">csplit</a> <a href="#csplit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Split a file into pieces.
> This generates files named "xx00", "xx01", and so on.
> More information: <https://www.gnu.org/software/coreutils/csplit>.

#### Split a file at lines 5 and 23:
```shell
csplit {{file}} {{5}} {{23}}
```
#### Split a file every 5 lines (this will fail if the total number of lines is not divisible by 5):
```shell
csplit {{file}} {{5}} {*}
```
#### Split a file every 5 lines, ignoring exact-division error:
```shell
csplit -k {{file}} {{5}} {*}
```
#### Split a file at line 5 and use a custom prefix for the output files:
```shell
csplit {{file}} {{5}} -f {{prefix}}
```
#### Split a file at a line matching a regular expression:
```shell
csplit {{file}} /{{regular_expression}}/
```
{% endraw %}{% raw %}
<h2 id="ctr">
  <a href="/en/linux/ctr.html">ctr</a> <a href="#ctr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage `containerd` containers and images.
> More information: <https://containerd.io>.

#### List all containers (running and stopped):
```shell
ctr containers list
```
#### List all images:
```shell
ctr images list
```
#### Pull an image:
```shell
ctr images pull {{image}}
```
#### Tag an image:
```shell
ctr images tag {{souce_image}}:{{source_tag}} {{target_image}}:{{target_tag}}
```
{% endraw %}{% raw %}
<h2 id="ctrlaltdel">
  <a href="/en/linux/ctrlaltdel.html">ctrlaltdel</a> <a href="#ctrlaltdel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility to control what happens when CTRL+ALT+DEL is pressed.

#### Get current setting:
```shell
ctrlaltdel
```
#### Set CTRL+ALT+DEL to reboot immediately, without any preparation:
```shell
sudo ctrlaltdel hard
```
#### Set CTRL+ALT+DEL to reboot "normally", giving processes a chance to exit first (send SIGINT to PID1):
```shell
sudo ctrlaltdel soft
```
{% endraw %}{% raw %}
<h2 id="cuyo">
  <a href="/en/linux/cuyo.html">cuyo</a> <a href="#cuyo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tetris like game.
> More information: <https://www.karimmi.de/cuyo/>.

#### Start a new game:
```shell
cuyo
```
#### Navigate the piece horizontally:
```shell
{{A|D}} OR {{Left|Right}} arrow key
```
#### Turn the piece:
```shell
{{W|Up arrow key}} 
```
#### Hard drop the piece:
```shell
{{S|Down arrow key}}
```
{% endraw %}{% raw %}
<h2 id="daemonize">
  <a href="/en/linux/daemonize.html">daemonize</a> <a href="#daemonize"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run a command (that does not daemonize itself) as a Unix daemon.
> More information: <http://software.clapper.org/daemonize/>.

#### Run a command as a daemon:
```shell
daemonize {{command}} {{command_arguments}}
```
#### Write the pid to the specified file:
```shell
daemonize -p {{path/to/pidfile}} {{command}} {{command_arguments}}
```
#### Use a lock file to ensure that only one instance runs at a time:
```shell
daemonize -l {{path/to/lockfile}} {{command}} {{command_arguments}}
```
#### Use the specified user account:
```shell
sudo daemonize -u {{user}} {{command}} {{command_arguments}}
```
{% endraw %}{% raw %}
<h2 id="datamash">
  <a href="/en/linux/datamash.html">datamash</a> <a href="#datamash"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool to perform basic numeric, textual and statistical operations on input textual data files.

#### Get max, min, mean and median of a single column of numbers:
```shell
seq 3 | datamash max 1 min 1 mean 1 median 1
```
#### Get the mean of a single column of float numbers (floats must use "," and not "."):
```shell
echo -e '1.0\n2.5\n3.1\n4.3\n5.6\n5.7' | tr '.' ',' | datamash mean 1
```
#### Get the mean of a single column of numbers with a given decimal precision:
```shell
echo -e '1\n2\n3\n4\n5\n5' | datamash -R {{number_of_decimals_wanted}} mean 1
```
#### Get the mean of a single column of numbers ignoring "Na" and "NaN" (literal) strings:
```shell
echo -e '1\n2\nNa\n3\nNaN' | datamash --narm mean 1
```
{% endraw %}{% raw %}
<h2 id="dbus-daemon">
  <a href="/en/linux/dbus-daemon.html">dbus-daemon</a> <a href="#dbus-daemon"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The D-Bus message daemon, allowing multiple programs to exchange messages.

#### Run the daemon with a configuration file:
```shell
dbus-daemon --config-file {{path/to/file}}
```
#### Run the daemon with the standard per-login-session message bus configuration:
```shell
dbus-daemon --session
```
#### Run the daemon with the standard systemwide message bus configuration:
```shell
dbus-daemon --system
```
#### Set the address to listen on and override the configuration value for it:
```shell
dbus-daemon --address {{address}}
```
#### Output the process id to stdout:
```shell
dbus-daemon --print-pid
```
#### Force the message bus to write to the system log for messages:
```shell
dbus-daemon --syslog
```
{% endraw %}{% raw %}
<h2 id="dconf-write">
  <a href="/en/linux/dconf-write.html">dconf write</a> <a href="#dconf-write"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Write a value to a dconf database path.
> More information: <https://developer.gnome.org/dconf>.

#### Write a string to a dconf path (note the nested quotes):
```shell
dconf write {{/example/dconf/path}} "'{{Example Value}}'"
```
#### Write a boolean to a dconf path:
```shell
dconf write {{/example/dconf/path}} {{true|false}}
```
#### Write an integer to a dconf path:
```shell
dconf write {{/example/dconf/path}} {{16}}
```
#### Write an array to a dconf path:
```shell
dconf write {{/example/dconf/path}} "[{{'My First Value', 'My Second Value'}}]"
```
#### Write an empty array to a dconf path:
```shell
dconf write {{/example/dconf/path}} "@as []"
```
{% endraw %}{% raw %}
<h2 id="dconf">
  <a href="/en/linux/dconf.html">dconf</a> <a href="#dconf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Simple tool for manipulating dconf databases.
> See also `dconf write`.
> More information: <https://developer.gnome.org/dconf>.

#### Print the value of a dconf path:
```shell
dconf read {{/example/dconf/path}}
```
#### List contents of a dconf path:
```shell
dconf list {{/example/dconf/path}}
```
#### Watch for dconf database changes in a path and subpaths:
```shell
dconf watch {{/example/dconf/path}}
```
{% endraw %}{% raw %}
<h2 id="ddrescue">
  <a href="/en/linux/ddrescue.html">ddrescue</a> <a href="#ddrescue"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Data recovery tool that reads data from damaged block devices.
> More information: <https://www.gnu.org/software/ddrescue/>.

#### Take an image of a device, creating a log file:
```shell
sudo ddrescue {{/dev/sdb}} {{path/to/image.dd}} {{path/to/log.txt}}
```
#### Clone Disk A to Disk B, creating a log file:
```shell
sudo ddrescue --force --no-scrape {{/dev/sdX}} {{/dev/sdY}} {{path/to/log.txt}}
```
{% endraw %}{% raw %}
<h2 id="debchange">
  <a href="/en/linux/debchange.html">debchange</a> <a href="#debchange"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool for maintenance of the debian/changelog file in a Debian source package.
> More information: <https://manpages.debian.org/debchange>.

#### Add a new version for a non-maintainer upload to the changelog:
```shell
debchange --nmu
```
#### Add a changelog entry to the current version:
```shell
debchange --append
```
#### Add a changelog entry to close the bug with specified ID:
```shell
debchange --closes {{bug_id}}
```
{% endraw %}{% raw %}
<h2 id="debman">
  <a href="/en/linux/debman.html">debman</a> <a href="#debman"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Read man pages from uninstalled packages.

#### Read a man page for a command that is provided by a specified package name:
```shell
debman -p {{package_name}} {{command_name}}
```
#### Specify a package version to download:
```shell
debman -p {{package_name}}={{version}} {{command_name}}
```
#### Read a man page in a `.deb` file:
```shell
debman -f {{path/to/filename.deb}} {{command_name}}
```
{% endraw %}{% raw %}
<h2 id="debootstrap">
  <a href="/en/linux/debootstrap.html">debootstrap</a> <a href="#debootstrap"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create a basic Debian system.
> More information: <https://wiki.debian.org/Debootstrap>.

#### Create a Debian stable release system inside the `debian-root` directory:
```shell
sudo debootstrap stable {{path/to/debian-root/}} http://deb.debian.org/debian
```
#### Create an Ubuntu 20.04 system inside the `focal-root` directory with a local mirror:
```shell
sudo debootstrap focal {{path/to/focal-root/}} {{file:///path/to/mirror/}}
```
#### Switch to a bootstrapped system:
```shell
sudo chroot {{path/to/root}}
```
#### List available releases:
```shell
ls /usr/share/debootstrap/scripts/
```
{% endraw %}{% raw %}
<h2 id="debugfs">
  <a href="/en/linux/debugfs.html">debugfs</a> <a href="#debugfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An interactive ext2/ext3/ext4 filesystem debugger.

#### Open the filesystem in read only mode:
```shell
debugfs {{/dev/sdXN}}
```
#### Open the filesystem in read write mode:
```shell
debugfs -w {{/dev/sdXN}}
```
#### Read commands from a specified file, execute them and then exit:
```shell
debugfs -f {{path/to/cmd_file}} {{/dev/sdXN}}
```
#### View the filesystem stats in debugfs console:
```shell
stats
```
#### Close the filesystem:
```shell
close -a
```
#### List all available commands:
```shell
lr
```
{% endraw %}{% raw %}
<h2 id="debuild">
  <a href="/en/linux/debuild.html">debuild</a> <a href="#debuild"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool to build a Debian package from source.
> More information: <https://manpages.debian.org/debuild>.

#### Build the package in the current directory:
```shell
debuild
```
#### Build a binary package only:
```shell
debuild -b
```
#### Do not run lintian after building the package:
```shell
debuild --no-lintian
```
{% endraw %}{% raw %}
<h2 id="deluser">
  <a href="/en/linux/deluser.html">deluser</a> <a href="#deluser"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Delete a user from the system.
> Note: all commands must be executed as root.
> More information: <https://manpages.debian.org/latest/adduser/deluser.html>.

#### Remove a user:
```shell
deluser {{username}}
```
#### Remove a user and their home directory:
```shell
deluser --remove-home {{username}}
```
#### Remove a user and their home, but backup their files into a `.tar.gz` file in the specified directory:
```shell
deluser --backup-to {{path/to/backup_directory}} --remove-home {{username}}
```
#### Remove a user, and all files owned by them:
```shell
deluser --remove-all-files {{username}}
```
{% endraw %}{% raw %}
<h2 id="dex">
  <a href="/en/linux/dex.html">dex</a> <a href="#dex"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> DesktopEntry Execution is a program to generate and execute DesktopEntry files of the Application type.
> More information: <https://github.com/jceb/dex>.

#### Execute all programs in the autostart folders:
```shell
dex --autostart
```
#### Execute all programs in the specified folders:
```shell
dex --autostart --search-paths {{path/to/directory1}}:{{path/to/directory2}}:{{path/to/directory3}}:
```
#### Preview the programs would be executed in a GNOME specific autostart:
```shell
dex --autostart --environment {{GNOME}}
```
#### Preview the programs would be executed in a regular autostart:
```shell
dex --autostart --dry-run
```
#### Preview the value of the DesktopEntry property `Name`:
```shell
dex --property {{Name}} {{path/to/file.desktop}}
```
#### Create a DesktopEntry for a program in the current directory:
```shell
dex --create {{path/to/file.desktop}}
```
#### Execute a single program (with `Terminal=true` in the desktop file) in the given terminal:
```shell
dex --term {{terminal}} {{path/to/file.desktop}}
```
{% endraw %}{% raw %}
<h2 id="dget">
  <a href="/en/linux/dget.html">dget</a> <a href="#dget"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Download Debian packages.
> More information: <https://manpages.debian.org/dget>.

#### Download a binary package:
```shell
dget {{package_name}}
```
#### Download and extract a package source from its `.dsc` file:
```shell
dget {{http://deb.debian.org/debian/pool/main/h/haskell-tldr/haskell-tldr_0.4.0-2.dsc}}
```
#### Download a package source tarball from its `.dsc` file but don't extract it:
```shell
dget -d {{http://deb.debian.org/debian/pool/main/h/haskell-tldr/haskell-tldr_0.4.0-2.dsc}}
```
{% endraw %}{% raw %}
<h2 id="diff3">
  <a href="/en/linux/diff3.html">diff3</a> <a href="#diff3"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compare three files line by line.

#### Compare files:
```shell
diff3 {{file1}} {{file2}} {{file3}}
```
#### Show all changes, outlining conflicts:
```shell
diff3 --show-all {{file1}} {{file2}} {{file3}}
```
{% endraw %}{% raw %}
<h2 id="disown">
  <a href="/en/linux/disown.html">disown</a> <a href="#disown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Allow sub-processes to live beyond the shell that they are attached to.
> See also the `jobs` command.

#### Disown the current job:
```shell
disown
```
#### Disown a specific job:
```shell
disown %{{job_number}}
```
#### Disown all jobs:
```shell
disown -a
```
#### Keep job (do not disown it), but mark it so that no future SIGHUP is received on shell exit:
```shell
disown -h %{{job_number}}
```
{% endraw %}{% raw %}
<h2 id="dkms">
  <a href="/en/linux/dkms.html">dkms</a> <a href="#dkms"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A framework that allows for dynamic building of kernel modules.
> More information: <https://github.com/dell/dkms>.

#### List currently installed modules:
```shell
dkms status
```
#### Rebuild all modules for the currently running kernel:
```shell
dkms autoinstall
```
#### Install version 1.2.1 of the acpi_call module for the currently running kernel:
```shell
dkms install -m {{acpi_call}} -v {{1.2.1}}
```
#### Remove version 1.2.1 of the acpi_call module from all kernels:
```shell
dkms remove -m {{acpi_call}} -v {{1.2.1}} --all
```
{% endraw %}{% raw %}
<h2 id="dmenu">
  <a href="/en/linux/dmenu.html">dmenu</a> <a href="#dmenu"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Dynamic menu.
> Creates a menu from a text input with each item on a new line.

#### Display a menu of the output of the `ls` command:
```shell
{{ls}} | dmenu
```
#### Display a menu with custom items separated by a new line (`\n`):
```shell
echo -e "{{red}}\n{{green}}\n{{blue}}" | dmenu
```
#### Let the user choose between multiple items and save the selected one to a file:
```shell
echo -e "{{red}}\n{{green}}\n{{blue}}" | dmenu > {{color.txt}}
```
#### Launch dmenu on a specific monitor:
```shell
ls | dmenu -m {{1}}
```
#### Display dmenu at the bottom of the screen:
```shell
ls | dmenu -b
```
{% endraw %}{% raw %}
<h2 id="dmesg">
  <a href="/en/linux/dmesg.html">dmesg</a> <a href="#dmesg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Write the kernel messages to standard output.

#### Show kernel messages:
```shell
dmesg
```
#### Show kernel error messages:
```shell
dmesg --level err
```
#### Show kernel messages and keep reading new ones, similar to `tail -f` (available in kernels 3.5.0 and newer):
```shell
dmesg -w
```
#### Show how much physical memory is available on this system:
```shell
dmesg | grep -i memory
```
#### Show kernel messages 1 page at a time:
```shell
dmesg | less
```
#### Show kernel messages with a timestamp (available in kernels 3.5.0 and newer):
```shell
dmesg -T
```
#### Show kernel messages in human-readable form (available in kernels 3.5.0 and newer):
```shell
dmesg -H
```
#### Colorize output (available in kernels 3.5.0 and newer):
```shell
dmesg -L
```
{% endraw %}{% raw %}
<h2 id="dmidecode">
  <a href="/en/linux/dmidecode.html">dmidecode</a> <a href="#dmidecode"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display the DMI (alternatively known as SMBIOS) table contents in a human-readable format.
> Requires root privileges.

#### Show all DMI table contents:
```shell
sudo dmidecode
```
#### Show the BIOS version:
```shell
sudo dmidecode -s bios-version
```
#### Show the system's serial number:
```shell
sudo dmidecode -s system-serial-number
```
#### Show BIOS information:
```shell
sudo dmidecode -t bios
```
#### Show CPU information:
```shell
sudo dmidecode -t processor
```
#### Show memory information:
```shell
sudo dmidecode -t memory
```
{% endraw %}{% raw %}
<h2 id="dnf">
  <a href="/en/linux/dnf.html">dnf</a> <a href="#dnf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Package management utility for RHEL, Fedora, and CentOS (replaces yum).
> More information: <https://dnf.readthedocs.io/>.

#### Upgrade installed packages to the newest available versions:
```shell
sudo dnf upgrade
```
#### Search packages via keywords:
```shell
dnf search {{keywords}}
```
#### Display details about a package:
```shell
dnf info {{package}}
```
#### Install a new package:
```shell
sudo dnf install {{package}}
```
#### Install a new package and assume yes to all questions:
```shell
sudo dnf -y install {{package}}
```
#### Remove a package:
```shell
sudo dnf remove {{package}}
```
#### List installed packages:
```shell
dnf list --installed
```
#### Find which packages provide a given file:
```shell
dnf provides {{file}}
```
{% endraw %}{% raw %}
<h2 id="dnsrecon">
  <a href="/en/linux/dnsrecon.html">dnsrecon</a> <a href="#dnsrecon"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> DNS enumeration tool.
> More information: <https://github.com/darkoperator/dnsrecon>.

#### Scan a domain and save the results to a SQLite database:
```shell
dnsrecon --domain {{example.com}} --db {{path/to/database.sqlite}}
```
#### Scan a domain, specifying the nameserver and performing a zone transfer:
```shell
dnsrecon --domain {{example.com}} --name_server {{nameserver.example.com}} --type axfr
```
#### Scan a domain, using a brute-force attack and a dictionary of subdomains and hostnames:
```shell
dnsrecon --domain {{example.com}} --dictionary {{path/to/dictionary.txt}} --type brt
```
#### Scan a domain, performing a reverse lookup of IP ranges from the SPF record and saving the results to a JSON file:
```shell
dnsrecon --domain {{example.com}} -s --json
```
#### Scan a domain, performing a Google enumeration and saving the results to a CSV file:
```shell
dnsrecon --domain {{example.com}} -g --csv
```
#### Scan a domain, performing DNS cache snooping:
```shell
dnsrecon --domain {{example.com}} --type snoop --name_server {{nameserver.example.com}} --dictionary {{path/to/dictionary.txt}}
```
#### Scan a domain, performing zone walking:
```shell
dnsrecon --domain {{example.com}} --type zonewalk
```
{% endraw %}{% raw %}
<h2 id="do-release-upgrade">
  <a href="/en/linux/do-release-upgrade.html">do-release-upgrade</a> <a href="#do-release-upgrade"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Ubuntu release upgrader.

#### Upgrade to the latest release:
```shell
sudo do-release-upgrade
```
#### Upgrade to the latest development release:
```shell
sudo do-release-upgrade --devel-release
```
#### Upgrade to the latest proposed release:
```shell
sudo do-release-upgrade --proposed
```
{% endraw %}{% raw %}
<h2 id="dockerd">
  <a href="/en/linux/dockerd.html">dockerd</a> <a href="#dockerd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A persistent process to start and manage docker containers.
> More information: <https://docs.docker.com/engine/reference/commandline/dockerd/>.

#### Run docker daemon:
```shell
dockerd
```
#### Run docker daemon and config it to listen to specific sockets(unix,tcp):
```shell
dockerd --host unix://{{path/to/tmp.sock}} --host tcp://{{ip}}
```
#### Run with specific daemon PID file:
```shell
dockerd --pidfile {{path/to/pid_file}}
```
#### Run in debug mode:
```shell
dockerd --debug
```
#### Run and set a specific log level:
```shell
dockerd --log-level={{debug|info|warn|error|fatal}}
```
{% endraw %}{% raw %}
<h2 id="dolphin">
  <a href="/en/linux/dolphin.html">dolphin</a> <a href="#dolphin"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> KDE file manager.
> More information: <https://apps.kde.org/dolphin/>.

#### Launch Dolphin:
```shell
dolphin
```
#### Launch Dolphin and display a specific directory:
```shell
dolphin {{path/to/directory}}
```
#### Launch Dolphin with a specific file or directory selected:
```shell
dolphin --select {{path/to/file_or_directory}}
```
#### Launch Dolphin in a separated window:
```shell
dolphin --new-window
```
#### Launch Dolphin in split view:
```shell
dolphin --split
```
#### Start the Dolphin daemon (only required to use the DBus interface):
```shell
dolphin --daemon
```
#### Display help:
```shell
dolphin --help
```
{% endraw %}{% raw %}
<h2 id="dos2unix">
  <a href="/en/linux/dos2unix.html">dos2unix</a> <a href="#dos2unix"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Change DOS-style line endings to Unix-style.
> Replaces CRLF with CR.

#### Change the line endings of a file:
```shell
dos2unix {{filename}}
```
#### Create a copy with Unix-style line endings:
```shell
dos2unix -n {{filename}} {{new_filename}}
```
{% endraw %}{% raw %}
<h2 id="dpkg-deb">
  <a href="/en/linux/dpkg-deb.html">dpkg-deb</a> <a href="#dpkg-deb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pack, unpack and provide information about Debian archives.
> More information: <https://manpages.debian.org/buster/dpkg/dpkg-deb.1.en.html>.

#### Display information about a package:
```shell
dpkg-deb --info {{path/to/file.deb}}
```
#### Display the package's name and version on one line:
```shell
dpkg-deb --show {{path/to/file.deb}}
```
#### List the package's contents:
```shell
dpkg-deb --contents {{path/to/file.deb}}
```
#### Extract package's contents into a directory:
```shell
dpkg-deb --extract {{path/to/file.deb}} {{path/to/directory}}
```
#### Create a package from a specified directory:
```shell
dpkg-deb --build {{path/to/directory}}
```
{% endraw %}{% raw %}
<h2 id="dpkg-query">
  <a href="/en/linux/dpkg-query.html">dpkg-query</a> <a href="#dpkg-query"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool that shows information about installed packages.

#### List all installed packages:
```shell
dpkg-query -l
```
#### List installed packages matching a pattern:
```shell
dpkg-query -l '{{pattern}}'
```
#### List all files installed by a package:
```shell
dpkg-query -L {{package_name}}
```
#### Show information about a package:
```shell
dpkg-query -s {{package_name}}
```
{% endraw %}{% raw %}
<h2 id="dpkg">
  <a href="/en/linux/dpkg.html">dpkg</a> <a href="#dpkg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Debian package manager.
> More information: <https://manpages.debian.org/buster/dpkg/dpkg.1.en.html>.

#### Install a package:
```shell
dpkg -i {{path/to/file.deb}}
```
#### Remove a package:
```shell
dpkg -r {{package_name}}
```
#### List installed packages:
```shell
dpkg -l {{pattern}}
```
#### List a package's contents:
```shell
dpkg -L {{package_name}}
```
#### List contents of a local package file:
```shell
dpkg -c {{path/to/file.deb}}
```
#### Find out which package owns a file:
```shell
dpkg -S {{filename}}
```
{% endraw %}{% raw %}
<h2 id="dstat">
  <a href="/en/linux/dstat.html">dstat</a> <a href="#dstat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Versatile tool for generating system resource statistics.
> More information: <http://dag.wieers.com/home-made/dstat>.

#### Display CPU, disk, net, paging and system statistics:
```shell
dstat
```
#### Display statistics every 5 seconds and 4 updates only:
```shell
dstat {{5}} {{4}}
```
#### Display CPU and memory statistics only:
```shell
dstat --cpu --mem
```
#### List all available dstat plugins:
```shell
dstat --list
```
#### Display the process using the most memory and most CPU:
```shell
dstat --top-mem --top-cpu
```
#### Display battery percentage and remaining battery time:
```shell
dstat --battery --battery-remain
```
{% endraw %}{% raw %}
<h2 id="dumpe2fs">
  <a href="/en/linux/dumpe2fs.html">dumpe2fs</a> <a href="#dumpe2fs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print the super block and blocks group information for ext2/ext3/ext4 filesystems.
> Unmount the partition before running this command using `umount {{device}}`.
> More information: <https://manned.org/dumpe2fs>.

#### Display ext2, ext3 and ext4 filesystem information:
```shell
dumpe2fs {{/dev/sdXN}}
```
#### Display the blocks which are reserved as bad in the filesystem:
```shell
dumpe2fs -b {{/dev/sdXN}}
```
#### Force display filesystem information even with non-recognisable feature flags:
```shell
dumpe2fs -f {{/dev/sdXN}}
```
#### Only display the superblock information and not any of the block group descriptor detail information:
```shell
dumpe2fs -h {{/dev/sdXN}}
```
#### Print the detailed group information block numbers in hexadecimal format:
```shell
dumpe2fs -x {{/dev/sdXN}}
```
{% endraw %}{% raw %}
<h2 id="dunstify">
  <a href="/en/linux/dunstify.html">dunstify</a> <a href="#dunstify"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A notification tool that is an extension of notify-send, but has more features based around dunst.
> Works with all options that work for notify-send.

#### Show a notification with a given title and message:
```shell
dunstify "{{Title}}" "{{Message}}"
```
#### Show a notification with specified urgency:
```shell
dunstify "{{Title}}" "{{Message}}" -u {{low|normal|critical}}
```
#### Specify a message ID (overwrites any previous messages with the same ID):
```shell
dunstify "{{Title}}" "{{Message}}" -r {{123}}
```
#### To see other possible options:
```shell
notify-send --help
```
{% endraw %}{% raw %}
<h2 id="duperemove">
  <a href="/en/linux/duperemove.html">duperemove</a> <a href="#duperemove"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Finds duplicate filesystem extents and optionally schedule them for deduplication.
> An extent is small part of a file inside the filesystem.
> On some filesystems one extent can be referenced multiple times, when parts of the content of the files are identical.
> More information: <https://markfasheh.github.io/duperemove/>.

#### Search for duplicate extents in a directory and show them:
```shell
duperemove -r {{path/to/directory}}
```
#### Deduplicate duplicate extents on a Btrfs or XFS (experimental) filesystem:
```shell
duperemove -r -d {{path/to/directory}}
```
#### Use a hash file to store extent hashes (less memory usage and can be reused on subsequent runs):
```shell
duperemove -r -d --hashfile={{path/to/hashfile}} {{path/to/directory}}
```
#### Limit I/O threads (for hashing and dedupe stage) and CPU threads (for duplicate extent finding stage):
```shell
duperemove -r -d --hashfile={{path/to/hashfile}} --io-threads={{N}} --cpu-threads={{N}} {{path/to/directory}}
```
{% endraw %}{% raw %}
<h2 id="e2freefrag">
  <a href="/en/linux/e2freefrag.html">e2freefrag</a> <a href="#e2freefrag"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print the free space fragmentation information for ext2/ext3/ext4 filesystems.
> More information: <https://manned.org/e2freefrag>.

#### Check how many free blocks are present as contiguous and aligned free space:
```shell
e2freefrag {{/dev/sdXN}}
```
#### Specify chunk size in kilobytes to print how many free chunks are available:
```shell
e2freefrag -c {{chunk_size_in_kb}} {{/dev/sdXN}}
```
{% endraw %}{% raw %}
<h2 id="e2fsck">
  <a href="/en/linux/e2fsck.html">e2fsck</a> <a href="#e2fsck"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Check a Linux ext2/ext3/ext4 filesystem. The filesystem should be unmounted at the time the command is run.

#### Check filesystem, reporting any damaged blocks:
```shell
e2fsck {{/dev/sdXN}}
```
#### Check filesystem and automatically repair any damaged blocks:
```shell
e2fsck -p {{/dev/sdXN}}
```
#### Check filesystem in read only mode:
```shell
e2fsck -c {{/dev/sdXN}}
```
{% endraw %}{% raw %}
<h2 id="e2image">
  <a href="/en/linux/e2image.html">e2image</a> <a href="#e2image"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Save critical ext2/ext3/ext4 filesystem metadata to a file.
> More information: <https://manned.org/e2image>.

#### Write metadata located on device to a specific file:
```shell
e2image {{/dev/sdXN}} {{path/to/image_file}}
```
#### Print metadata located on device to stdout:
```shell
e2image {{/dev/sdXN}} -
```
#### Restore the filesystem metadata back to the device:
```shell
e2image -I {{/dev/sdXN}} {{path/to/image_file}}
```
#### Create a large raw sparse file with metadata at proper offsets:
```shell
e2image -r {{/dev/sdXN}} {{path/to/image_file}}
```
#### Create a QCOW2 image file instead of a normal or raw image file:
```shell
e2image -Q {{/dev/sdXN}} {{path/to/image_file}}
```
{% endraw %}{% raw %}
<h2 id="e2label">
  <a href="/en/linux/e2label.html">e2label</a> <a href="#e2label"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Change the label on an ext2/ext3/ext4 filesystem.

#### Change the volume label on a specific ext partition:
```shell
e2label {{/dev/sda1}} "{{label_name}}"
```
{% endraw %}{% raw %}
<h2 id="e2undo">
  <a href="/en/linux/e2undo.html">e2undo</a> <a href="#e2undo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Replay undo logs for an ext2/ext3/ext4 filesystem.
> This can be used to undo a failed operation by an e2fsprogs program.
> More information: <https://man7.org/linux/man-pages/man8/e2undo.8.html>.

#### Display information about a specific undo file:
```shell
e2undo -h {{path/to/undo_file}} {{/dev/sdXN}}
```
#### Perform a dry-run and display the candidate blocks for replaying:
```shell
e2undo -nv {{path/to/undo_file}} {{/dev/sdXN}}
```
#### Perform an undo operation:
```shell
e2undo {{path/to/undo_file}} {{/dev/sdXN}}
```
#### Perform an undo operation and display verbose information:
```shell
e2undo -v {{path/to/undo_file}} {{/dev/sdXN}}
```
#### Write the old contents of the block to an undo file before overwriting a file system block:
```shell
e2undo -z {{path/to/file.e2undo}} {{path/to/undo_file}} {{/dev/sdXN}}
```
{% endraw %}{% raw %}
<h2 id="e4defrag">
  <a href="/en/linux/e4defrag.html">e4defrag</a> <a href="#e4defrag"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Defragment an ext4 filesystem.

#### Defragment the filesystem:
```shell
e4defrag {{/dev/sdXN}}
```
#### See how fragmented a filesystem is:
```shell
e4defrag -c {{/dev/sdXN}}
```
#### Print errors and the fragmentation count before and after each file:
```shell
e4defrag -v {{/dev/sdXN}}
```
{% endraw %}{% raw %}
<h2 id="ebuild">
  <a href="/en/linux/ebuild.html">ebuild</a> <a href="#ebuild"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A low level interface to the Gentoo Portage system.

#### Create or update the package manifest:
```shell
ebuild {{path/to/file.ebuild}} manifest
```
#### Clean the temporary build directories for the build file:
```shell
ebuild {{path/to/file.ebuild}} clean
```
#### Fetch sources if they do not exist:
```shell
ebuild {{path/to/file.ebuild}} fetch
```
#### Extract the sources to a temporary build directory:
```shell
ebuild {{path/to/file.ebuild}} unpack
```
#### Compile the extracted sources:
```shell
ebuild {{path/to/file.ebuild}} compile
```
#### Install the package to a temporary install directory:
```shell
ebuild {{path/to/file.ebuild}} install
```
#### Install the temporary files to the live filesystem:
```shell
ebuild {{path/to/file.ebuild}} qmerge
```
#### Fetch, unpack, compile, install and qmerge the specified ebuild file:
```shell
ebuild {{path/to/file.ebuild}} merge
```
{% endraw %}{% raw %}
<h2 id="edit">
  <a href="/en/linux/edit.html">edit</a> <a href="#edit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An alias to a `run-mailcap`'s action edit.
> Originally `run-mailcap` is used to process/edit mime-type/file.

#### Edit action can be used to view any file on default mailcap explorer:
```shell
edit {{filename}}
```
#### With `run-mailcap`:
```shell
run-mailcap --action=edit {{filename}}
```
{% endraw %}{% raw %}
<h2 id="edquota">
  <a href="/en/linux/edquota.html">edquota</a> <a href="#edquota"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Edit quotas for a user or group. By default it operates on all filesystems with quotas.
> Quota information is stored permanently in the `quota.user` and `quota.group` files in the root of the filesystem.

#### Edit quota of the current user:
```shell
edquota --user $(whoami)
```
#### Edit quota of a specific user:
```shell
sudo edquota --user {{username}}
```
#### Edit quota for a group:
```shell
sudo edquota --group {{group}}
```
#### Restrict operations to a given filesystem (by default edquota operates on all filesystems with quotas):
```shell
sudo edquota --file-system {{filesystem}}
```
#### Edit the default grace period:
```shell
sudo edquota -t
```
#### Duplicate a quota to other users:
```shell
sudo edquota -p {{reference_user}} {{destination_user1}} {{destination_user2}}
```
{% endraw %}{% raw %}
<h2 id="efibootmgr">
  <a href="/en/linux/efibootmgr.html">efibootmgr</a> <a href="#efibootmgr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manipulate the UEFI Boot Manager.
> More information: <https://manned.org/efibootmgr>.

#### List the current settings / bootnums:
```shell
efibootmgr
```
#### List the filepaths:
```shell
efibootmgr -v
```
#### Add UEFI Shell v2 as a boot option:
```shell
sudo efibootmgr -c -d {{/dev/sda1}} -l {{\EFI\tools\Shell.efi}} -L "{{UEFI Shell}}"
```
#### Change the current boot order:
```shell
sudo efibootmgr -o {{0002,0008,0001,0005}}
```
#### Delete a boot option:
```shell
sudo efibootmgr -b {{0008}} --delete-bootnum
```
{% endraw %}{% raw %}
<h2 id="eix">
  <a href="/en/linux/eix.html">eix</a> <a href="#eix"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utilities for searching local Gentoo packages.
> Update local package cache using `eix-update`.

#### Search for a package:
```shell
eix {{package_name}}
```
#### Search for installed packages:
```shell
eix --installed {{package_name}}
```
#### Search in package descriptions:
```shell
eix --description "{{description}}"
```
#### Search by package license:
```shell
eix --license {{license}}
```
#### Exclude results from search:
```shell
eix --not --license {{license}}
```
{% endraw %}{% raw %}
<h2 id="eject">
  <a href="/en/linux/eject.html">eject</a> <a href="#eject"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Eject cds, floppy disks and tape drives.

#### Display the default device:
```shell
eject -d
```
#### Eject the default device:
```shell
eject
```
#### Eject a specific device (the default order is cd-rom, scsi, floppy and tape):
```shell
eject {{/dev/cdrom}}
```
#### Toggle whether a device's tray is open or closed:
```shell
eject -T {{/dev/cdrom}}
```
#### Eject a cd drive:
```shell
eject -r {{/dev/cdrom}}
```
#### Eject a floppy drive:
```shell
eject -f {{/mnt/floppy}}
```
#### Eject a tape drive:
```shell
eject -q {{/mnt/tape}}
```
{% endraw %}{% raw %}
<h2 id="emerge">
  <a href="/en/linux/emerge.html">emerge</a> <a href="#emerge"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gentoo Linux package manager utility.

#### Synchronize all packages:
```shell
emerge --sync
```
#### Update all packages, including dependencies:
```shell
emerge -uDNav @world
```
#### Resume a failed updated, skipping the failing package:
```shell
emerge --resume --skipfirst
```
#### Install a new package, with confirmation:
```shell
emerge -av {{package_name}}
```
#### Remove a package, with confirmation:
```shell
emerge -Cav {{package_name}}
```
#### Remove orphaned packages (that were installed only as dependencies):
```shell
emerge -avc
```
#### Search the package database for a keyword:
```shell
emerge -S {{keyword}}
```
{% endraw %}{% raw %}
<h2 id="enum4linux">
  <a href="/en/linux/enum4linux.html">enum4linux</a> <a href="#enum4linux"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool for enumerating Windows and Samba information from remote systems.
> It attempts to offer similar functionality to enum.exe formerly available from www.bindview.com.

#### Try to enumerate using all methods:
```shell
enum4linux -a {{remote_host}}
```
#### Enumerate using given login credentials:
```shell
enum4liux -u {{user_name}} -p {{password}} {{remote_host}}
```
#### List usernames from a given host:
```shell
enum4liux -U {{remote_host}}
```
#### List shares:
```shell
enum4liux -S {{remote_host}}
```
#### Get OS information:
```shell
enum4liux -o {{remote_host}}
```
{% endraw %}{% raw %}
<h2 id="equery">
  <a href="/en/linux/equery.html">equery</a> <a href="#equery"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> View information about Portage packages.

#### List all installed packages:
```shell
equery list '*'
```
#### Search for installed packages in the Portage tree and in overlays:
```shell
equery list -po {{package_name}}
```
#### List all packages that depend on a given package:
```shell
equery depends {{package_name}}
```
#### List all packages that a given package depends on:
```shell
equery depgraph {{package_name}}
```
#### List all files installed by a package:
```shell
equery files --tree {{package_name}}
```
{% endraw %}{% raw %}
<h2 id="etckeeper">
  <a href="/en/linux/etckeeper.html">etckeeper</a> <a href="#etckeeper"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Track system configuration files in Git.
> More information: <http://etckeeper.branchable.com/>.

#### Set up a Git repo and perform various setup tasks (run from `/etc`):
```shell
sudo etckeeper init
```
#### Commit all changes in `/etc`:
```shell
sudo etckeeper commit {{message}}
```
#### Run arbitrary Git commands:
```shell
sudo etckeeper vcs {{status}}
```
#### Check if there are uncommitted changes (only returns an exit code):
```shell
sudo etckeeper unclean
```
#### Destroy existing repo and stop tracking changes:
```shell
sudo etckeeper uninit
```
{% endraw %}{% raw %}
<h2 id="ethtool">
  <a href="/en/linux/ethtool.html">ethtool</a> <a href="#ethtool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display and modify Network Interface Controller (NIC) parameters.
> More information: <http://man7.org/linux/man-pages/man8/ethtool.8.html>.

#### Display the current settings for an interface:
```shell
ethtool {{eth0}}
```
#### Display the driver information for an interface:
```shell
ethtool --driver {{eth0}}
```
#### Display the network usage statistics for an interface:
```shell
ethtool --statistics {{eth0}}
```
#### Blink one or more LEDs on an interface for 10 seconds:
```shell
ethtool --identify {{eth0}} {{10}}
```
#### Set the link speed, duplex mode, and parameter auto-negotiation for a given interface:
```shell
ethtool -s {{eth0}} speed {{10|100|1000}} duplex {{half|full}} autoneg {{on|off}}
```
{% endraw %}{% raw %}
<h2 id="eval">
  <a href="/en/linux/eval.html">eval</a> <a href="#eval"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Execute arguments as a single command in the current shell and return its result.

#### Call `echo` with the "foo" argument:
```shell
eval "{{echo foo}}"
```
#### Set a variable in the current shell:
```shell
eval "{{foo=bar}}"
```
{% endraw %}{% raw %}
<h2 id="exif">
  <a href="/en/linux/exif.html">exif</a> <a href="#exif"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show and change EXIF information in JPEG files.
> More information: <https://github.com/libexif/exif/>.

#### Show all recognized EXIF information in an image:
```shell
exif {{path/to/image.jpg}}
```
#### Show a table listing known EXIF tags and whether each one exists in an image:
```shell
exif --list-tags --no-fixup {{image.jpg}}
```
#### Extract the image thumbnail into the file `thumbnail.jpg`:
```shell
exif --extract-thumbnail --output={{thumbnail.jpg}} {{image.jpg}}
```
#### Show the raw contents of the "Model" tag in the given image:
```shell
exif --ifd={{0}} --tag={{Model}} --machine-readable {{image.jpg}}
```
#### Change the value of the "Artist" tag to John Smith and save to `new.jpg`:
```shell
exif --output={{new.jpg}} --ifd={{0}} --tag="{{Artist}}" --set-value="{{John Smith}}" --no-fixup {{image.jpg}}
```
{% endraw %}{% raw %}
<h2 id="expect">
  <a href="/en/linux/expect.html">expect</a> <a href="#expect"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Script executor that interacts with other programs that require user input.
> More information: <https://manned.org/expect>.

#### Execute an expect script from a file:
```shell
expect {{path/to/file}}
```
#### Execute a specified expect script:
```shell
expect -c "{{commands}}"
```
#### Enter an interactive REPL (use `exit` or Ctrl + D to exit):
```shell
expect -i
```
{% endraw %}{% raw %}
<h2 id="export">
  <a href="/en/linux/export.html">export</a> <a href="#export"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command to mark shell variables in the current environment to be exported with any newly forked child processes.

#### Set a new environment variable:
```shell
export {{VARIABLE}}={{value}}
```
#### Remove an environment variable:
```shell
export -n {{VARIABLE}}
```
#### Mark a shell function for export:
```shell
export -f {{FUNCTION_NAME}}
```
#### Append something to the PATH variable:
```shell
export PATH=$PATH:{{path/to/append}}
```
{% endraw %}{% raw %}
<h2 id="extrace">
  <a href="/en/linux/extrace.html">extrace</a> <a href="#extrace"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Trace exec() calls.
> More information: <https://github.com/chneukirchen/extrace>.

#### Trace all program executions occurring on the system:
```shell
sudo extrace
```
#### Run a command and only trace descendants of this command:
```shell
sudo extrace {{command}}
```
#### Print the current working directory of each process:
```shell
sudo extrace -d
```
#### Resolve the full path of each executable:
```shell
sudo extrace -l
```
#### Display the user running each process:
```shell
sudo extrace -u
```
{% endraw %}{% raw %}
<h2 id="extundelete">
  <a href="/en/linux/extundelete.html">extundelete</a> <a href="#extundelete"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Recover deleted files from ext3 or ext4 partitions by parsing the journal.
> See also `date` for Unix time information and `umount` for unmounting partitions.
> More information: <http://extundelete.sourceforge.net>.

#### Restore all deleted files inside partition N on device X:
```shell
sudo extundelete {{/dev/sdXN}} --restore-all
```
#### Restore a file from a path relative to root (Do not start the path with `/`):
```shell
extundelete {{/dev/sdXN}} --restore-file {{path/to/file}}
```
#### Restore a directory from a path relative to root (Do not start the path with `/`):
```shell
extundelete {{/dev/sdXN}} --restore-directory {{path/to/directory}}
```
#### Restore all files deleted after January 1st, 2020 (in Unix time):
```shell
extundelete {{/dev/sdXN}} --restore-all --after {{1577840400}}
```
{% endraw %}{% raw %}
<h2 id="eyed3">
  <a href="/en/linux/eyed3.html">eyeD3</a> <a href="#eyed3"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Read and manipulate metadata of MP3 files.
> More information: <https://eyed3.readthedocs.io/en/latest/>.

#### View information about an MP3 file:
```shell
eyeD3 {{filename.mp3}}
```
#### Set the title of an MP3 file:
```shell
eyeD3 --title "{{A Title}}" {{filename.mp3}}
```
#### Set the album of all the MP3 files in a directory:
```shell
eyeD3 --album "{{Album Name}}" {{*.mp3}}
```
#### Set the front cover art for an MP3 file:
```shell
eyeD3 --add-image {{front_cover.jpeg}}:FRONT_COVER: {{filename.mp3}}
```
{% endraw %}{% raw %}
<h2 id="f5fpc">
  <a href="/en/linux/f5fpc.html">f5fpc</a> <a href="#f5fpc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A proprietry commercial SSL VPN client by BIG-IP Edge.

#### Open a new VPN connection:
```shell
sudo f5fpc --start
```
#### Open a new VPN connection to a specific host:
```shell
sudo f5fpc --start --host {{host.example.com}}
```
#### Specify a username (user will be prompted for a password):
```shell
sudo f5fpc --start --host {{host.example.com}} --username {{user}}
```
#### Show the current VPN status:
```shell
sudo f5fpc --info
```
#### Shutdown the VPN connection:
```shell
sudo f5fpc --stop
```
{% endraw %}{% raw %}
<h2 id="fail2ban-client">
  <a href="/en/linux/fail2ban-client.html">fail2ban-client</a> <a href="#fail2ban-client"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Configure and control fail2ban server.
> More information: <https://github.com/fail2ban/fail2ban>.

#### Retrieve current status of the jail service:
```shell
fail2ban-client status {{jail}}
```
#### Remove the specified IP from the jail service's ban list:
```shell
fail2ban-client set {{jail}} unbanip {{ip}}
```
#### Verify fail2ban server is alive:
```shell
fail2ban-client ping
```
{% endraw %}{% raw %}
<h2 id="faketime">
  <a href="/en/linux/faketime.html">faketime</a> <a href="#faketime"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Fake the system time for a given command.
> More information: <https://manpages.ubuntu.com/manpages/trusty/man1/faketime.1.html>.

#### Fake the time to this evening, before printing the result of `date`:
```shell
faketime '{{today 23:30}}' {{date}}
```
#### Open a new `bash` shell, which uses yesterday as the current date:
```shell
faketime '{{yesterday}}' {{bash}}
```
#### Simulate how any program would act next friday night:
```shell
faketime '{{next Friday 1 am}}' {{path/to/any/program}}
```
{% endraw %}{% raw %}
<h2 id="fallocate">
  <a href="/en/linux/fallocate.html">fallocate</a> <a href="#fallocate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Reserve or deallocate disk space to files.
> The utility allocates space without zeroing.

#### Reserve a file taking up 700MB of disk space:
```shell
fallocate --length {{700M}} {{path/to/file}}
```
#### Shrink an already allocated file by 200MB:
```shell
fallocate --collapse-range --length {{200M}} {{path/to/file}}
```
#### Shrink 20MB of space after 100MB in a file:
```shell
fallocate --collapse-range --offset {{100M}} --length {{20M}} {{path/to/file}}
```
{% endraw %}{% raw %}
<h2 id="fatlabel">
  <a href="/en/linux/fatlabel.html">fatlabel</a> <a href="#fatlabel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sets or gets the label of a FAT32 partition.

#### Get the label of a FAT32 partition:
```shell
fatlabel {{/dev/sda1}}
```
#### Set the label of a FAT32 partition:
```shell
fatlabel {{/dev/sdc3}} "{{new_label}}"
```
{% endraw %}{% raw %}
<h2 id="fc-cache">
  <a href="/en/linux/fc-cache.html">fc-cache</a> <a href="#fc-cache"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Scan font directories in order to build font cache files.

#### Generate font cache files:
```shell
fc-cache
```
#### Force a rebuild of all font cache files, without checking if cache is up-to-date:
```shell
fc-cache -f
```
#### Erase font cache files, then generate new font cache files:
```shell
fc-cache -r
```
{% endraw %}{% raw %}
<h2 id="fc-list">
  <a href="/en/linux/fc-list.html">fc-list</a> <a href="#fc-list"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List available fonts installed on the system.

#### Return a list of installed fonts in your system:
```shell
fc-list
```
#### Return a list of installed fonts with given name:
```shell
fc-list | grep '{{DejaVu Serif}}'
```
#### Return the number of installed fonts in your system:
```shell
fc-list | wc -l
```
{% endraw %}{% raw %}
<h2 id="fc-match">
  <a href="/en/linux/fc-match.html">fc-match</a> <a href="#fc-match"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Match available fonts.

#### Return a sorted list of best matching fonts:
```shell
fc-match -s '{{DejaVu Serif}}'
```
{% endraw %}{% raw %}
<h2 id="fc-pattern">
  <a href="/en/linux/fc-pattern.html">fc-pattern</a> <a href="#fc-pattern"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Shows information about a font matching a pattern.

#### Display default information about a font:
```shell
fc-pattern -d '{{DejaVu Serif}}'
```
{% endraw %}{% raw %}
<h2 id="fc">
  <a href="/en/linux/fc.html">fc</a> <a href="#fc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Open the most recent command and edit it.

#### Open in the default system editor:
```shell
fc
```
#### Specify an editor to open with:
```shell
fc -e {{'emacs'}}
```
#### List recent commands from history:
```shell
fc -l
```
{% endraw %}{% raw %}
<h2 id="fcrackzip">
  <a href="/en/linux/fcrackzip.html">fcrackzip</a> <a href="#fcrackzip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ZIP archive password cracking utility.

#### Brute-force a password with a length of 4 to 8 characters, and contains only alphanumeric characters (order matters):
```shell
fcrackzip --brute-force --length 4-8 --charset aA1 {{archive}}
```
#### Brute-force a password in verbose mode with a length of 3 characters that only contains lowercase characters, `$` and `%`:
```shell
fcrackzip -v --brute-force --length 3 --charset a:$% {{archive}}
```
#### Brute-force a password that contains only lowercase and special characters:
```shell
fcrackzip --brute-force --length 4 --charset a! {{archive}}
```
#### Brute-force a password containing only digits, starting from the password `12345`:
```shell
fcrackzip --brute-force --length 5 --charset 1 --init-password 12345 {{archive}}
```
#### Crack a password using a wordlist:
```shell
fcrackzip --use-unzip --dictionary --init-password {{wordlist}} {{archive}}
```
#### Benchmark cracking performance:
```shell
fcrackzip --benchmark
```
{% endraw %}{% raw %}
<h2 id="fdisk">
  <a href="/en/linux/fdisk.html">fdisk</a> <a href="#fdisk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A program for managing partition tables and partitions on a hard disk.

#### List partitions:
```shell
fdisk -l
```
#### Start the partition manipulator:
```shell
fdisk {{/dev/sdX}}
```
{% endraw %}{% raw %}
<h2 id="feedreader">
  <a href="/en/linux/feedreader.html">feedreader</a> <a href="#feedreader"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A GUI desktop RSS client.
> More information: <https://jangernert.github.io/FeedReader/>.

#### Print the count of unread articles:
```shell
feedreader --unreadCount
```
#### Add a URL for a feed to follow:
```shell
feedreader --addFeed={{feed_url}}
```
#### Grab a specific article using its URL:
```shell
feedreader --grabArticle={{article_url}}
```
#### Download all images from a specific article:
```shell
feedreader --url={{feed_url}} --grabImages={{article_path}}
```
#### Play media from a URL:
```shell
feedreader --playMedia={{article_url}}
```
{% endraw %}{% raw %}
<h2 id="feh">
  <a href="/en/linux/feh.html">feh</a> <a href="#feh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lightweight image viewing utility.

#### View images locally or using a URL:
```shell
feh {{path/to/images}}
```
#### View images recursively:
```shell
feh --recursive {{path/to/images}}
```
#### View images without window borders:
```shell
feh --borderless {{path/to/images}}
```
#### Exit after the last image:
```shell
feh --cycle-once {{path/to/images}}
```
#### Set the slideshow cycle delay:
```shell
feh --slideshow-delay {{seconds}} {{path/to/images}}
```
#### Set your wallpaper (centered, filled, maximized, scaled or tiled):
```shell
feh --bg-{{center|fill|max|scale|tile}} {{path/to/image}}
```
#### Create a montage of all images within a directory. Outputs as a new image:
```shell
feh --montage --thumb-height {{150}} --thumb-width {{150}} --index-info "{{%nn%wx%h}}" --output {{path/to/montage_image.png}}
```
{% endraw %}{% raw %}
<h2 id="rename">
  <a href="/en/linux/file-rename.html">rename</a> <a href="#rename"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rename multiple files.
> NOTE: this page refers to the command from the `file-rename` Debian package.

#### Rename files using a Perl Common Regular Expression (substitute 'foo' with 'bar' wherever found):
```shell
rename {{'s/foo/bar/'}} {{*}}
```
#### Dry-run - display which renames would occur without performing them:
```shell
rename -n {{'s/foo/bar/'}} {{*}}
```
#### Force renaming even if the operation would remove existing destination files:
```shell
rename -f {{'s/foo/bar/'}} {{*}}
```
#### Convert filenames to lower case (use `-f` in case-insensitive filesystems to prevent "already exists" errors):
```shell
rename 'y/A-Z/a-z/' {{*}}
```
#### Replace whitespace with underscores:
```shell
rename 's/\s+/_/g' {{*}}
```
{% endraw %}{% raw %}
<h2 id="file">
  <a href="/en/linux/file.html">file</a> <a href="#file"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Determine file type.

#### Give a description of the type of the specified file. Works fine for files with no file extension:
```shell
file {{filename}}
```
#### Look inside a zipped file and determine the file type(s) inside:
```shell
file -z {{foo.zip}}
```
#### Allow file to work with special or device files:
```shell
file -s {{filename}}
```
#### Don't stop at first file type match; keep going until the end of the file:
```shell
file -k {{filename}}
```
#### Determine the mime encoding type of a file:
```shell
file -i {{filename}}
```
{% endraw %}{% raw %}
<h2 id="filefrag">
  <a href="/en/linux/filefrag.html">filefrag</a> <a href="#filefrag"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Report how badly fragmented a particular file might be.
> More information: <https://manned.org/filefrag>.

#### Display a report for a specific file:
```shell
filefrag {{path/to/file}}
```
#### Display a report for space-separated list of files:
```shell
filefrag {{path/to/file1}} {{path/to/file2}}
```
#### Display a report using a 1024 byte blocksize:
```shell
filefrag -b {{path/to/file}}
```
#### Sync the file before requesting the mapping:
```shell
filefrag -s {{path/to/files}}
```
#### Display mapping of extended attributes:
```shell
filefrag -x {{path/to/files}}
```
#### Display a report with verbose information:
```shell
filefrag -v {{path/to/files}}
```
{% endraw %}{% raw %}
<h2 id="finch">
  <a href="/en/linux/finch.html">finch</a> <a href="#finch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Console-based modular messaging client.
> More information: <https://developer.pidgin.im/wiki/Using%20Finch>.

#### Launch finch:
```shell
finch
```
#### Quit:
```shell
alt + q or ctrl + c
```
#### Show actions menu:
```shell
alt + a
```
#### Jump to n-th window:
```shell
alt + {{number_key}}
```
#### Close current window:
```shell
alt + c
```
#### Start moving a window, use arrow keys to move, press escape when done:
```shell
alt + m
```
#### Start resizing a window, use arrow keys to resize, press escape when done:
```shell
alt + r
```
{% endraw %}{% raw %}
<h2 id="findfs">
  <a href="/en/linux/findfs.html">findfs</a> <a href="#findfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Finds a filesystem by label or UUID.
> More information: <https://mirrors.edge.kernel.org/pub/linux/utils/util-linux>.

#### Search block devices by filesystem label:
```shell
findfs LABEL={{label}}
```
#### Search by filesystem UUID:
```shell
findfs UUID={{uuid}}
```
#### Search by partition label (GPT or MAC partition table):
```shell
findfs PARTLABEL={{partition_label}}
```
#### Search by partition UUID (GPT partition table only):
```shell
findfs PARTUUID={{partition_uuid}}
```
{% endraw %}{% raw %}
<h2 id="findmnt">
  <a href="/en/linux/findmnt.html">findmnt</a> <a href="#findmnt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Find your filesystem.

#### List all mounted filesystems:
```shell
findmnt
```
#### Search for a device:
```shell
findmnt {{/dev/sdb1}}
```
#### Search for a mountpoint:
```shell
findmnt {{/}}
```
#### Find filesystems in specific type:
```shell
findmnt -t {{ext4}}
```
#### Find filesystems with specific label:
```shell
findmnt LABEL={{BigStorage}}
```
{% endraw %}{% raw %}
<h2 id="firejail">
  <a href="/en/linux/firejail.html">firejail</a> <a href="#firejail"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Securely sandboxes processes to containers using built-in Linux capabilities.

#### Integrate firejail with your desktop environment:
```shell
sudo firecfg
```
#### Open a restricted Mozilla Firefox:
```shell
firejail {{firefox}}
```
#### Start a restricted Apache server on a known interface and address:
```shell
firejail --net={{eth0}} --ip={{192.168.1.244}} {{/etc/init.d/apache2}} {{start}}
```
#### List running sandboxes:
```shell
firejail --list
```
#### List network activity from running sandboxes:
```shell
firejail --netstats
```
#### Shutdown a running sandbox:
```shell
firejail --shutdown={{7777}}
```
{% endraw %}{% raw %}
<h2 id="firewall-cmd">
  <a href="/en/linux/firewall-cmd.html">firewall-cmd</a> <a href="#firewall-cmd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The firewalld command-line client.

#### View the available firewall zones:
```shell
firewall-cmd --get-active-zones
```
#### View the rules which are currently applied:
```shell
firewall-cmd --list-all
```
#### Permanently move the interface into the block zone, effectively blocking all communication:
```shell
firewall-cmd --permanent --zone={{block}} --change-interface={{enp1s0}}
```
#### Permanently open the port for a service in the specified zone (like port 443 when in the `public` zone):
```shell
firewall-cmd --permanent --zone={{public}} --add-service={{https}}
```
#### Permanently close the port for a service in the specified zone (like port 80 when in the `public` zone):
```shell
firewall-cmd --permanent --zone={{public}} --remove-service={{http}}
```
#### Permanently open two arbitrary ports in the specified zone:
```shell
firewall-cmd --permanent --zone={{public}} --add-port={{25565/tcp}} --add-port={{19132/udp}}
```
#### Reload firewalld to force rule changes to take effect:
```shell
firewall-cmd --reload
```
{% endraw %}{% raw %}
<h2 id="flameshot">
  <a href="/en/linux/flameshot.html">flameshot</a> <a href="#flameshot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Screenshot utility with a gui interface.
> Supports basic image editing, such as text, shapes, colors, and imgur.
> More information: <https://flameshot.js.org>.

#### Launch flameshot in gui mode:
```shell
flameshot launcher
```
#### Take a screenshot by clicking and dragging:
```shell
flameshot gui
```
#### Take a full screen screenshot:
```shell
flameshot full
```
#### Set the save path to write screenshots to:
```shell
flameshot full --path {{path/to/directory}}
```
#### Delay the screenshot for N milliseconds and output to clipboard:
```shell
flameshot full --delay {{2000}} --clipboard
```
{% endraw %}{% raw %}
<h2 id="flash">
  <a href="/en/linux/flash.html">flash</a> <a href="#flash"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Flash cards in the terminal.
> More information: <https://github.com/tallguyjenks/fla.sh>.

#### Open a menu of available flashcard decks for selection:
```shell
flash
```
#### Display the program version:
```shell
flash -v
```
#### Display information about the flashcard system:
```shell
flash -i
```
#### Display a list of available commands:
```shell
flash -h
```
#### Change the previewer from default `bat` to `cat`:
```shell
flash -p {{cat}}
```
{% endraw %}{% raw %}
<h2 id="flashrom">
  <a href="/en/linux/flashrom.html">flashrom</a> <a href="#flashrom"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Read, write, verify and erase flash chips.
> More information: <https://manned.org/flashrom>.

#### Probe the chip, ensuring the wiring is correct:
```shell
flashrom --programmer {{programmer}}
```
#### Read flash and save it to a file:
```shell
flashrom -p {{programmer}} --read {{path/to/file}}
```
#### Write a file to the flash:
```shell
flashrom -p {{programmer}} --write {{path/to/file}}
```
#### Verify the flash against a file:
```shell
flashrom -p {{programmer}} --verify {{path/to/file}}
```
#### Probe the chip using RaspberryPi:
```shell
flashrom -p {{linux_spi:dev=/dev/spidev0.0}}
```
{% endraw %}{% raw %}
<h2 id="flatpak-builder">
  <a href="/en/linux/flatpak-builder.html">flatpak-builder</a> <a href="#flatpak-builder"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Help build application dependencies.
> More information: <https://docs.flatpak.org/en/latest/flatpak-builder-command-reference.html>.

#### Build a Flatpak and export it to a new repository:
```shell
flatpak-builder {{path/to/build_directory}} {{path/to/manifest}}
```
#### Build a Flatpak and export it to the specified repository:
```shell
flatpak-builder --repo={{repository_name}} {{path/to/build_directory}} {{path/to/manifest}}
```
#### Build a Flatpak and install it locally:
```shell
flatpak-builder --install {{path/to/build_directory}} {{path/to/manifest}}
```
#### Build and sign a Flatpak and export it to the specified repository:
```shell
flatpak-builder --gpg-sign={{key_id}} --repo={{repository_name}} {{path/to/manifest}}
```
#### Run a shell inside of an application sandbox without installing it:
```shell
flatpak-builder --run {{path/to/build_directory}} {{path/to/manifest}} {{sh}}
```
{% endraw %}{% raw %}
<h2 id="flatpak">
  <a href="/en/linux/flatpak.html">flatpak</a> <a href="#flatpak"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Build, install and run flatpak applications and runtimes.

#### Run an installed application:
```shell
flatpak run {{name}}
```
#### Install an application from a remote source:
```shell
flatpak install {{remote}} {{name}}
```
#### List all installed applications and runtimes:
```shell
flatpak list
```
#### Update all installed applications and runtimes:
```shell
flatpak update
```
#### Add a remote source:
```shell
flatpak remote-add --if-not-exists {{remote_name}} {{remote_url}}
```
#### List all configured remote sources:
```shell
flatpak remote-list
```
#### Remove an installed application:
```shell
flatpak remove {{name}}
```
#### Show information about an installed application:
```shell
flatpak info {{name}}
```
{% endraw %}{% raw %}
<h2 id="foreman">
  <a href="/en/linux/foreman.html">foreman</a> <a href="#foreman"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage Procfile-based applications.

#### Start an application with the Procfile in the current directory:
```shell
foreman start
```
#### Start an application with a specified Procfile:
```shell
foreman start -f {{Procfile}}
```
#### Start a specific application:
```shell
foreman start {{process}}
```
#### Validate Procfile format:
```shell
foreman check
```
#### Run one-off commands with the process's environment:
```shell
foreman run {{command}}
```
#### Start all processes except the one named "worker":
```shell
foreman start -m all=1,{{worker}}=0
```
{% endraw %}{% raw %}
<h2 id="free">
  <a href="/en/linux/free.html">free</a> <a href="#free"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display amount of free and used memory in the system.

#### Display system memory:
```shell
free
```
#### Display memory in Bytes/KB/MB/GB:
```shell
free -{{b|k|m|g}}
```
#### Display memory in human readable units:
```shell
free -h
```
#### Refresh the output every 2 seconds:
```shell
free -s {{2}}
```
{% endraw %}{% raw %}
<h2 id="fsck">
  <a href="/en/linux/fsck.html">fsck</a> <a href="#fsck"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Check the integrity of a filesystem or repair it. The filesystem should be unmounted at the time the command is run.

#### Check filesystem `/dev/sdX`, reporting any damaged blocks:
```shell
fsck {{/dev/sdX}}
```
#### Check filesystem `/dev/sdX`, reporting any damaged blocks and interactively letting the user choose to repair each one:
```shell
fsck -r {{/dev/sdX}}
```
#### Check filesystem `/dev/sdX`, reporting any damaged blocks and automatically repairing them:
```shell
fsck -a {{/dev/sdX}}
```
{% endraw %}{% raw %}
<h2 id="fstrim">
  <a href="/en/linux/fstrim.html">fstrim</a> <a href="#fstrim"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Discard unused blocks on a mounted filesystem.
> Only supported by flash memory devices such as SSDs and microSD cards.

#### Trim unused blocks on all mounted partitions that support it:
```shell
sudo fstrim --all
```
#### Trim unused blocks on a specified partition:
```shell
sudo fstrim {{/}}
```
#### Display statistics after trimming:
```shell
sudo fstrim --verbose {{/}}
```
{% endraw %}{% raw %}
<h2 id="fuser">
  <a href="/en/linux/fuser.html">fuser</a> <a href="#fuser"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display process IDs currently using files or sockets.

#### Find which processes are accessing a file or directory:
```shell
fuser {{path/to/file_or_directory}}
```
#### Show more fields (`USER`, `PID`, `ACCESS` and `COMMAND`):
```shell
fuser --verbose {{path/to/file_or_directory}}
```
#### Identify processes using a TCP socket:
```shell
fuser --namespace tcp {{port}}
```
#### Kill all processes accessing a file or directory (sends the `SIGKILL` signal):
```shell
fuser --kill {{path/to/file_or_directory}}
```
#### Find which processes are accessing the filesystem containing a specific file or directory:
```shell
fuser --mount {{path/to/file_or_directory}}
```
{% endraw %}{% raw %}
<h2 id="gcov">
  <a href="/en/linux/gcov.html">gcov</a> <a href="#gcov"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Code coverage analysis and profiling tool that discovers untested parts of a program.
> Also displays a copy of source code annotated with execution frequencies of code segments.
> More information: <https://gcc.gnu.org/onlinedocs/gcc/Invoking-Gcov.html>.

#### Generate a coverage report named `file.cpp.gcov`:
```shell
gcov {{path/to/file.cpp}}
```
#### Write individual execution counts for every basic block:
```shell
gcov --all-blocks {{path/to/file.cpp}}
```
#### Write branch frequencies to the output file and print summary information to stdout as a percentage:
```shell
gcov --branch-probabilities {{path/to/file.cpp}}
```
#### Write branch frequencies as the number of branches taken, rather than the percentage:
```shell
gcov --branch-counts {{path/to/file.cpp}}
```
#### Do not create a `gcov` output file:
```shell
gcov --no-output {{path/to/file.cpp}}
```
#### Write file level as well as function level summaries:
```shell
gcov --function-summaries {{path/to/file.cpp}}
```
{% endraw %}{% raw %}
<h2 id="gdebi">
  <a href="/en/linux/gdebi.html">gdebi</a> <a href="#gdebi"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Simple tool to install `.deb` files.
> More information: <https://www.commandlinux.com/man-page/man1/gdebi.1.html>.

#### Install local `.deb` packages resolving and installing its dependencies:
```shell
gdebi {{path/to/package.deb}}
```
#### Display the program version:
```shell
gdebi --version
```
#### Do not show progress information:
```shell
gdebi {{path/to/package.deb}} --quiet
```
#### Set an APT configuration option:
```shell
gdebi {{path/to/package.deb}} --option={{APT_OPTS}}
```
#### Use alternative root dir:
```shell
gdebi {{path/to/package.deb}} --root={{path/to/root_dir}}
```
{% endraw %}{% raw %}
<h2 id="gedit">
  <a href="/en/linux/gedit.html">gedit</a> <a href="#gedit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Text editor of the GNOME Desktop project.

#### Open a text file:
```shell
gedit {{path/to/file}}
```
#### Open multiple text files:
```shell
gedit {{file1 file2 ...}}
```
#### Open a text file with a specific encoding:
```shell
gedit --encoding={{UTF-8}} {{path/to/file}}
```
#### Display a list of supported encodings:
```shell
gedit --list-encodings
```
{% endraw %}{% raw %}
<h2 id="genfstab">
  <a href="/en/linux/genfstab.html">genfstab</a> <a href="#genfstab"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux install script to generate output suitable for addition to an fstab file.
> More information: <https://man.archlinux.org/man/extra/arch-install-scripts/genfstab.8>.

#### Display an fstab compatible output based on a volume label:
```shell
genfstab -L {{path/to/mount_point}}
```
#### Display an fstab compatible output based on a volume UUID:
```shell
genfstab -U {{path/to/mount_point}}
```
#### A usual way to generate an fstab file, requires root permissions:
```shell
genfstab -U {{/mnt}} >> {{/mnt/etc/fstab}}
```
#### Append a volume into an fstab file to mount it automatically:
```shell
genfstab -U {{path/to/mount_point}} | sudo tee -a /etc/fstab
```
{% endraw %}{% raw %}
<h2 id="genid">
  <a href="/en/linux/genid.html">genid</a> <a href="#genid"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate IDs, such as snowflakes, UUIDs, and a new GAID.
> More information: <https://github.com/bleonard252/genid>.

#### Generate a UUIDv4:
```shell
genid uuid
```
#### Generate a UUIDv5 using a namespace UUID and a specific name:
```shell
genid uuidv5 {{{ce598faa-8dd0-49ee-8525-9e24fff71dca}}} {{name}}
```
#### Generate a Discord Snowflake, without a trailing newline (useful in shell scripts):
```shell
genid --script snowflake
```
#### Generate a Generic Anonymous ID with a specific "real ID":
```shell
genid gaid {{real_id}}
```
#### Generate a Snowflake with the epoch set to a specific date:
```shell
genid snowflake --epoch={{unix_epoch_time}}
```
{% endraw %}{% raw %}
<h2 id="genie">
  <a href="/en/linux/genie.html">genie</a> <a href="#genie"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Set up and use a "bottle" namespace to run systemd under WSL (Windows Subsystem for Linux).
> To run these from Windows rather than an already-running distribution, precede them with `wsl`.
> More information: <https://github.com/arkane-systems/genie>.

#### Initialize the bottle (run once, at start):
```shell
genie -i
```
#### Run a login shell inside the bottle:
```shell
genie -s
```
#### Run a specified command inside the bottle:
```shell
genie -c {{command}}
```
{% endraw %}{% raw %}
<h2 id="genkernel">
  <a href="/en/linux/genkernel.html">genkernel</a> <a href="#genkernel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gentoo Linux utility to compile and install kernels.

#### Automatically compile and install a generic kernel:
```shell
sudo genkernel all
```
#### Build and install the bzImage|initramfs|kernel|ramdisk only:
```shell
sudo genkernel {{bzImage|initramfs|kernel|ramdisk}}
```
#### Apply changes to the kernel configuration before compiling and installing:
```shell
sudo genkernel --menuconfig all
```
#### Generate a kernel with a custom name:
```shell
sudo genkernel --kernname={{custom_name}} all
```
#### Use a kernel source outside of the default directory `/usr/src/linux`:
```shell
sudo genkernel --kerneldir={{path/to/directory}} all
```
{% endraw %}{% raw %}
<h2 id="getent">
  <a href="/en/linux/getent.html">getent</a> <a href="#getent"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Get entries from Name Service Switch libraries.

#### Get list of all groups:
```shell
getent group
```
#### See the members of a group:
```shell
getent group {{group_name}}
```
#### Get list of all services:
```shell
getent services
```
#### Find a username by UID:
```shell
getent passwd 1000
```
#### Perform a reverse DNS lookup:
```shell
getent hosts {{host}}
```
{% endraw %}{% raw %}
<h2 id="getfacl">
  <a href="/en/linux/getfacl.html">getfacl</a> <a href="#getfacl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Get file access control lists.

#### Display the file access control list:
```shell
getfacl {{path/to/file_or_directory}}
```
#### Display the file access control list with numeric user and group IDs:
```shell
getfacl -n {{path/to/file_or_directory}}
```
#### Display the file access control list with tabular output format:
```shell
getfacl -t {{path/to/file_or_directory}}
```
{% endraw %}{% raw %}
<h2 id="gnome-extensions">
  <a href="/en/linux/gnome-extensions.html">gnome-extensions</a> <a href="#gnome-extensions"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage gnome extensions from the terminal.
> More information: <https://wiki.gnome.org/Projects/GnomeShell/Extensions>.

#### Display the version:
```shell
gnome-extensions version
```
#### List all the installed extensions:
```shell
gnome-extensions list
```
#### Display information about a specific extension:
```shell
gnome-extensions info "{{extension_id}}"
```
#### Display help for a subcommand (like `list`):
```shell
gnome-extensions help {{subcommand}}
```
#### Enable a specific extension:
```shell
gnome-extensions enable "{{extension_id}}"
```
#### Disable a specific extension:
```shell
gnome-extension disable "{{extension_id}}"
```
#### Uninstall a specific extension:
```shell
gnome-extension uninstall "{{extension_id}}"
```
{% endraw %}{% raw %}
<h2 id="gnome-terminal">
  <a href="/en/linux/gnome-terminal.html">gnome-terminal</a> <a href="#gnome-terminal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The GNOME Terminal emulator.

#### Open a new GNOME terminal window:
```shell
gnome-terminal
```
#### Run a specific command in a new terminal window:
```shell
gnome-terminal -- {{command}}
```
#### Open a new tab in the last opened window instead:
```shell
gnome-terminal --tab
```
#### Set the title of the new tab:
```shell
gnome-terminal --tab --title "{{title}}"
```
{% endraw %}{% raw %}
<h2 id="google-chrome">
  <a href="/en/linux/google-chrome.html">google-chrome</a> <a href="#google-chrome"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The web browser from Google.
> More information: <https://chrome.google.com>.

#### Run with a custom profile directory:
```shell
google-chrome --user-data-dir={{path/to/directory}}
```
#### Run without CORS validation, useful to test an API:
```shell
google-chrome --user-data-dir={{path/to/directory}} --disable-web-security
```
{% endraw %}{% raw %}
<h2 id="gpasswd">
  <a href="/en/linux/gpasswd.html">gpasswd</a> <a href="#gpasswd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Administer `/etc/group` and `/etc/gshadow`.

#### Define group administrators:
```shell
sudo gpasswd -A {{user1,user2}} {{group}}
```
#### Set the list of group members:
```shell
sudo gpasswd -M {{user1,user2}} {{group}}
```
#### Create a password for the named group:
```shell
gpasswd {{group}}
```
#### Add a user to the named group:
```shell
gpasswd -a {{user}} {{group}}
```
#### Remove a user from the named group:
```shell
gpasswd -d {{user}} {{group}}
```
{% endraw %}{% raw %}
<h2 id="groupadd">
  <a href="/en/linux/groupadd.html">groupadd</a> <a href="#groupadd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Add user groups to the system.
> More information: <https://manned.org/groupadd>.

#### Create a new Linux group:
```shell
groupadd {{group_name}}
```
#### Create new group with a specific groupid:
```shell
groupadd {{group_name}} -g {{group_id}}
```
{% endraw %}{% raw %}
<h2 id="groupdel">
  <a href="/en/linux/groupdel.html">groupdel</a> <a href="#groupdel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Delete existing user groups from the system.
> More information: <https://manned.org/groupdel>.

#### Delete an existing group:
```shell
groupdel {{group_name}}
```
{% endraw %}{% raw %}
<h2 id="groupmod">
  <a href="/en/linux/groupmod.html">groupmod</a> <a href="#groupmod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Modify existing user groups in the system.
> More information: <https://manned.org/groupmod>.

#### Change the group name:
```shell
groupmod -n {{new_group_name}} {{old_group_name}}
```
#### Change the group id:
```shell
groupmod -g {{new_group_id}} {{old_group_name}}
```
{% endraw %}{% raw %}
<h2 id="grub-install">
  <a href="/en/linux/grub-install.html">grub-install</a> <a href="#grub-install"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Install GRUB to a device.
> More information: <https://www.gnu.org/software/grub/manual/grub/html_node/Installing-GRUB-using-grub_002dinstall.html>.

#### Install GRUB on a BIOS system:
```shell
grub-install --target={{i386-pc}} {{path/to/device}}
```
#### Install GRUB on an UEFI system:
```shell
grub-install --target={{x86_64-efi}} --efi-directory={{path/to/efi_directory}} --bootloader-id={{GRUB}}
```
#### Install GRUB pre-loading specific modules:
```shell
grub-install --target={{x86_64-efi}} --efi-directory={{path/to/efi_directory}} --modules="{{part_gpt part_msdos}}"
```
{% endraw %}{% raw %}
<h2 id="grub-mkconfig">
  <a href="/en/linux/grub-mkconfig.html">grub-mkconfig</a> <a href="#grub-mkconfig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate a GRUB configuration file.
> More information: <https://www.gnu.org/software/grub/manual/grub/html_node/Invoking-grub_002dmkconfig.html>.

#### Do a dry run and print the configuration to stdout:
```shell
sudo grub-mkconfig
```
#### Generate the configuration file:
```shell
sudo grub-mkconfig --output={{/boot/grub/grub.cfg}}
```
#### Print the help page:
```shell
grub-mkconfig --help
```
{% endraw %}{% raw %}
<h2 id="gs">
  <a href="/en/linux/gs.html">gs</a> <a href="#gs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> GhostScript is a PDF and PostScript interpreter.

#### To view a file:
```shell
gs -dQUIET -dBATCH {{file.pdf}}
```
#### Reduce PDF file size to 150 dpi images for reading on a e-book device:
```shell
gs -dNOPAUSE -dQUIET -dBATCH -sDEVICE=pdfwrite -dPDFSETTINGS=/ebook -sOutputFile={{output.pdf}} {{input.pdf}}
```
#### Convert PDF file (pages 1 through 3) to an image with 150 dpi resolution:
```shell
gs -dQUIET -dBATCH -dNOPAUSE -sDEVICE=jpeg -r150 -dFirstPage={{1}} -dLastPage={{3}} -sOutputFile={{output_%d.jpg}} {{input.pdf}}
```
#### Extract pages from a PDF file:
```shell
gs -dQUIET -dBATCH -dNOPAUSE -sDEVICE=pdfwrite -sOutputFile={{output.pdf}} {{input.pdf}}
```
#### Merge PDF files:
```shell
gs -dQUIET -dBATCH -dNOPAUSE -sDEVICE=pdfwrite -sOutputFile={{output.pdf}} {{input1.pdf}} {{input2.pdf}}
```
#### Convert from PostScript file to PDF file:
```shell
gs -dQUIET -dBATCH -dNOPAUSE -sDEVICE=pdfwrite -sOutputFile={{output.pdf}} {{input.ps}}
```
{% endraw %}{% raw %}
<h2 id="guake">
  <a href="/en/linux/guake.html">guake</a> <a href="#guake"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A drop-down terminal for GNOME.

#### Toggle Guake visibility:
```shell
F12
```
#### Toggle fullscreen mode:
```shell
F11
```
#### Open a new tab:
```shell
Ctrl+Shift+T
```
#### Close the terminal:
```shell
Super+X
```
#### Go to the previous tab:
```shell
Ctrl+PageUp
```
#### Search the selected text in the browser:
```shell
Shift+Ctrl+L
```
{% endraw %}{% raw %}
<h2 id="guix-package">
  <a href="/en/linux/guix-package.html">guix package</a> <a href="#guix-package"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Install, upgrade and remove Guix packages, or rollback to previous configurations.

#### Install a new package:
```shell
guix package -i {{package_name}}
```
#### Remove a package:
```shell
guix package -r {{package_name}}
```
#### Search the package database for a regular expression:
```shell
guix package -s "{{search_pattern}}"
```
#### List installed packages:
```shell
guix package -I
```
#### List generations:
```shell
guix package -l
```
#### Roll back to the previous generation:
```shell
guix package --roll-back
```
{% endraw %}{% raw %}
<h2 id="halt">
  <a href="/en/linux/halt.html">halt</a> <a href="#halt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Halt the system.
> More information: <https://www.man7.org/linux/man-pages/man8/halt.8.html>.

#### Halt the system:
```shell
halt
```
#### Power off the system (same as `poweroff`):
```shell
halt --poweroff
```
#### Reboot the system (same as `reboot`):
```shell
halt --reboot
```
#### Halt immediately without contacting the system manager:
```shell
halt --force --force
```
#### Write the wtmp shutdown entry without halting the system:
```shell
halt --wtmp-only
```
{% endraw %}{% raw %}
<h2 id="hardinfo">
  <a href="/en/linux/hardinfo.html">hardinfo</a> <a href="#hardinfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show hardware information in GUI window.

#### Start hardinfo:
```shell
hardinfo
```
#### Print report to standard output:
```shell
hardinfo -r
```
#### Save report to HTML file:
```shell
hardinfo -r -f html > hardinfo.html
```
{% endraw %}{% raw %}
<h2 id="hashcat">
  <a href="/en/linux/hashcat.html">hashcat</a> <a href="#hashcat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Fast and advanced password recovery tool.
> More information: <https://manned.org/hashcat>.

#### Perform a brute-force attack (mode 3) with the default hashcat mask:
```shell
hashcat --hash-type {{hash_type_id}} --attack-mode {{3}} {{hash_value}}
```
#### Perform a brute-force attack (mode 3) with a known pattern of 4 digits:
```shell
hashcat --hash-type {{hash_type_id}} --attack-mode {{3}} {{hash_value}} "{{?d?d?d?d}}"
```
#### Perform a brute-force attack (mode 3) using at most 8 of all printable ASCII characters:
```shell
hashcat --hash-type {{hash_type_id}} --attack-mode {{3}} --increment {{hash_value}} "{{?a?a?a?a?a?a?a?a}}"
```
#### Perform a dictionary attack (mode 0) using the RockYou wordlist of a Kali Linux box:
```shell
hashcat --hash-type {{hash_type_id}} --attack-mode {{0}} {{hash_value}} {{/usr/share/wordlists/rockyou.txt}}
```
#### Perform a rule based dictionary attack (mode 0) using the RockYou wordlist mutated with common password variations:
```shell
hashcat --hash-type {{hash_type_id}} --attack-mode {{0}} --rules-file {{/usr/share/hashcat/rules/best64.rule}} {{hash_value}} {{/usr/share/wordlists/rockyou.txt}}
```
#### Perform a combination attack (mode 1) using the concatenation of words from two different custom dictionaries:
```shell
hashcat --hash-type {{hash_type_id}} --attack-mode {{1}} {{hash_value}} {{/path/to/dictionary1.txt}} {{/path/to/dictionary2.txt}}
```
#### Show result of an already cracked hash:
```shell
hashcat --show {{hash_value}}
```
{% endraw %}{% raw %}
<h2 id="hdparm">
  <a href="/en/linux/hdparm.html">hdparm</a> <a href="#hdparm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Get and set SATA and IDE hard drive parameters.

#### Request the identification info of a given device:
```shell
sudo hdparm -I /dev/{{device}}
```
#### Get the Advanced Power Management level:
```shell
sudo hdparm -B /dev/{{device}}
```
#### Set the Advanced Power Management value (values 1-127 permit spin-down, and values 128-254 do not):
```shell
sudo hdparm -B {{1}} /dev/{{device}}
```
#### Display the device's current power mode status:
```shell
sudo hdparm -C /dev/{{device}}
```
#### Force a drive to immediately enter standby mode (usually causes a drive to spin down):
```shell
sudo hdparm -y /dev/{{device}}
```
#### Put the drive into idle (low-power) mode, also setting its standby timeout:
```shell
sudo hdparm -S {{standby_timeout}} {{device}}
```
{% endraw %}{% raw %}
<h2 id="hello">
  <a href="/en/linux/hello.html">hello</a> <a href="#hello"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print "Hello, world!", "hello, world" or a customizable text.
> More information: <https://www.gnu.org/software/hello/>.

#### Print "Hello, world!":
```shell
hello
```
#### Print "hello, world", the traditional type:
```shell
hello --traditional
```
#### Print a text message:
```shell
hello --greeting="{{greeting_text}}"
```
{% endraw %}{% raw %}
<h2 id="hexdump">
  <a href="/en/linux/hexdump.html">hexdump</a> <a href="#hexdump"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An ASCII, decimal, hexadecimal, octal dump.

#### Print the hexadecimal representation of a file:
```shell
hexdump {{file}}
```
#### Display the input offset in hexadecimal and its ASCII representation in two columns:
```shell
hexdump -C {{file}}
```
#### Display the hexadecimal representation of a file, but interpret only n bytes of the input:
```shell
hexdump -C -n{{number_of_bytes}} {{file}}
```
{% endraw %}{% raw %}
<h2 id="hlint">
  <a href="/en/linux/hlint.html">hlint</a> <a href="#hlint"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool for suggesting improvements to Haskell code.
> More information: <http://hackage.haskell.org/package/hlint>.

#### Display suggestions for a given file:
```shell
hlint {{path/to/file}} options
```
#### Check all Haskell files and generate a report:
```shell
hlint {{path/to/directory}} --report
```
#### Automatically apply most suggestions:
```shell
hlint {{path/to/file}} --refactor
```
#### Display additional options:
```shell
hlint {{path/to/file}} --refactor-options
```
#### Generate a settings file ignoring all outstanding hints:
```shell
hlint {{path/to/file}} --default > {{.hlint.yaml}}
```
{% endraw %}{% raw %}
<h2 id="homectl">
  <a href="/en/linux/homectl.html">homectl</a> <a href="#homectl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create, remove, change or inspect home directories using the systemd-homed service.
> More information: <https://man.archlinux.org/man/homectl.1>.

#### List user accounts and their associated home directories:
```shell
homectl list
```
#### Create a user account and their associated home directory:
```shell
sudo homectl create {{username}}
```
#### Remove a specific user and the associated home directory:
```shell
sudo homectl remove {{username}}
```
#### Change the password for a specific user:
```shell
sudo homectl passwd {{username}}
```
#### Run a shell or a command with access to a specific home directory:
```shell
sudo homectl with {{username}} -- {{command}} {{command_arguments}}
```
#### Lock or unlock a specific home directory:
```shell
sudo homectl {{lock|unlock}} {{username}}
```
#### Change the disk space assigned to a specific home directory to 100 GiB:
```shell
sudo homectl resize {{username}} {{100G}}
```
#### Display help:
```shell
homectl --help
```
{% endraw %}{% raw %}
<h2 id="homeshick">
  <a href="/en/linux/homeshick.html">homeshick</a> <a href="#homeshick"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Synchronize Git dotfiles.
> More information: <https://github.com/andsens/homeshick/wiki>.

#### Create a new castle:
```shell
homeshick generate {{castle_name}}
```
#### Add a file to your castle:
```shell
homeshick track {{castle_name}} {{path/to/file}}
```
#### Go to a castle:
```shell
homeshick cd {{castle_name}}
```
#### Clone a castle:
```shell
homeshick clone {{github_username}}/{{repository_name}}
```
#### Symlink all files from a castle:
```shell
homeshick link {{castle_name}}
```
{% endraw %}{% raw %}
<h2 id="hostname">
  <a href="/en/linux/hostname.html">hostname</a> <a href="#hostname"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show or set the system's host name.

#### Show current host name:
```shell
hostname
```
#### Show the network address of the host name:
```shell
hostname -i
```
#### Show all network addresses of the host:
```shell
hostname -I
```
#### Show the FQDN (Fully Qualified Domain Name):
```shell
hostname --fqdn
```
#### Set current host name:
```shell
hostname {{new_hostname}}
```
{% endraw %}{% raw %}
<h2 id="hostnamectl">
  <a href="/en/linux/hostnamectl.html">hostnamectl</a> <a href="#hostnamectl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Get or set the hostname of the computer.

#### Get the hostname of the computer:
```shell
hostnamectl
```
#### Set the hostname of the computer:
```shell
sudo hostnamectl set-hostname "{{hostname}}"
```
#### Set a pretty hostname for the computer:
```shell
sudo hostnamectl set-hostname --static "{{hostname.example.com}}" && sudo hostnamectl set-hostname --pretty "{{hostname}}"
```
#### Reset hostname to its default value:
```shell
sudo hostnamectl set-hostname --pretty ""
```
{% endraw %}{% raw %}
<h2 id="htpdate">
  <a href="/en/linux/htpdate.html">htpdate</a> <a href="#htpdate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Synchronize local date and time via HTTP headers from web servers.
> More information: <http://www.vervest.org/htp/>.

#### Synchronize date and time:
```shell
sudo htpdate {{host}}
```
#### Perform simulation of synchronization, without any action:
```shell
htpdate -q {{host}}
```
#### Compensate the systematisch clock drift:
```shell
sudo htpdate -x {{host}}
```
#### Set time immediate after the synchronization:
```shell
sudo htpdate -s {{host}}
```
{% endraw %}{% raw %}
<h2 id="http-prompt">
  <a href="/en/linux/http-prompt.html">http-prompt</a> <a href="#http-prompt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An interactive command-line HTTP client featuring autocomplete and syntax highlighting.

#### Launch a session targeting the default URL of http://localhost:8000 or the previous session:
```shell
http-prompt
```
#### Launch a session with a given URL:
```shell
http-prompt {{http://example.com}}
```
#### Launch a session with some initial options:
```shell
http-prompt {{localhost:8000/api}} --auth {{username:password}}
```
{% endraw %}{% raw %}
<h2 id="http_load">
  <a href="/en/linux/http_load.html">http_load</a> <a href="#http_load"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A HTTP benchmarking tool.
> Runs multiple HTTP fetches in parallel to test the throughput of a web server.
> More information: <http://www.acme.com/software/http_load/>.

#### Emulate 20 requests based on a given URL list file per second for 60 seconds:
```shell
http_load -rate {{20}} -seconds {{60}} {{path/to/urls.txt}}
```
#### Emulate 5 concurrent requests based on a given URL list file for 60 seconds:
```shell
http_load -parallel {{5}} -seconds {{60}} {{path/to/urls.txt}}
```
#### Emulate 1000 requests at 20 requests per second, based on a given URL list file:
```shell
http_load -rate {{20}} -fetches {{1000}} {{path/to/urls.txt}}
```
#### Emulate 1000 requests at 5 concurrent requests at a time, based on a given URL list file:
```shell
http_load -parallel {{5}} -fetches {{1000}} {{path/to/urls.txt}}
```
{% endraw %}{% raw %}
<h2 id="httpie">
  <a href="/en/linux/httpie.html">httpie</a> <a href="#httpie"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A user friendly command-line HTTP tool.

#### Send a GET request (default method with no request data):
```shell
http {{https://example.com}}
```
#### Send a POST request (default method with request data):
```shell
http {{https://example.com}} {{hello=World}}
```
#### Send a POST request with redirected input:
```shell
http {{https://example.com}} < {{file.json}}
```
#### Send a PUT request with a given json body:
```shell
http PUT {{https://example.com/todos/7}} {{hello=world}}
```
#### Send a DELETE request with a given request header:
```shell
http DELETE {{https://example.com/todos/7}} {{API-Key:foo}}
```
#### Show the whole HTTP exchange (both request and response):
```shell
http -v {{https://example.com}}
```
#### Download a file:
```shell
http --download {{https://example.com}}
```
{% endraw %}{% raw %}
<h2 id="hwclock">
  <a href="/en/linux/hwclock.html">hwclock</a> <a href="#hwclock"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Used for reading or changing the hardware clock. Usually requires root.

#### Display the current time as reported by the hardware clock:
```shell
hwclock
```
#### Write the current software clock time to the hardware clock (sometimes used during system setup):
```shell
hwclock --systohc
```
#### Write the current hardware clock time to the software clock:
```shell
hwclock --hctosys
```
{% endraw %}{% raw %}
<h2 id="i3">
  <a href="/en/linux/i3.html">i3</a> <a href="#i3"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A dynamic tiling window manager.
> More information: <https://i3wm.org/docs/userguide.html>.

#### Start i3 (Note that a pre-existing window manager must not be open when this command is run.):
```shell
i3
```
#### Open a new terminal window:
```shell
Super + Return
```
#### Create a new workspace:
```shell
Super + Shift + {{number}}
```
#### Switch to workspace {{number}}:
```shell
Super + {{number}}
```
#### Open new window horizontally:
```shell
Super + h
```
#### Open new window vertically:
```shell
Super + v
```
#### Open application (type out application name after executing command):
```shell
Super + D
```
{% endraw %}{% raw %}
<h2 id="i3lock">
  <a href="/en/linux/i3lock.html">i3lock</a> <a href="#i3lock"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Simple screen locker built for the i3 window manager.
> More information: <https://i3wm.org/i3lock>.

#### Lock screen with a simple color background (rrggbb format):
```shell
i3lock -c {{0000ff}}
```
#### Lock screen to a PNG background:
```shell
i3lock -i {{path/to/picture.png}}
```
#### Disable the unlock indicator (removes feedback on keypress):
```shell
i3lock -u
```
#### Display mouse pointer instead of hiding it ('default' for default pointer, 'win' for a MS Windows pointer):
```shell
i3lock -p {{default|win}}
```
#### Lock screen to a PNG background displayed in multiple monitors, with enabled mouse pointer:
```shell
i3lock -i {{path/to/picture.png}} -p {{default|win}} -t
```
{% endraw %}{% raw %}
<h2 id="i7z">
  <a href="/en/linux/i7z.html">i7z</a> <a href="#i7z"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An Intel CPU (only i3, i5 and i7) realtime reporting tool.

#### Start i7z (needs to be run in super user mode):
```shell
sudo i7z
```
{% endraw %}{% raw %}
<h2 id="ifdown">
  <a href="/en/linux/ifdown.html">ifdown</a> <a href="#ifdown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Disable network interfaces.
> More information: <https://manned.org/ifdown>.

#### Disable interface eth0:
```shell
ifdown {{eth0}}
```
#### Disable all interfaces which are enabled:
```shell
ifdown -a
```
{% endraw %}{% raw %}
<h2 id="iftop">
  <a href="/en/linux/iftop.html">iftop</a> <a href="#iftop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show bandwidth usage on an interface by host.
> More information: <https://manned.org/iftop>.

#### Show the bandwidth usage:
```shell
sudo iftop
```
#### Show the bandwidth usage of a given interface:
```shell
sudo iftop -i {{interface}}
```
#### Show the bandwidth usage with port information:
```shell
sudo iftop -P
```
#### Do not show bar graphs of traffic:
```shell
sudo iftop -b
```
#### Do not look up hostnames:
```shell
sudo iftop -n
```
#### Get help about interactive commands:
```shell
?
```
{% endraw %}{% raw %}
<h2 id="ifup">
  <a href="/en/linux/ifup.html">ifup</a> <a href="#ifup"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool used to enable network interfaces.
> More information: <https://manpages.debian.org/latest/ifupdown/ifup.8.html>.

#### Enable interface eth0:
```shell
ifup {{eth0}}
```
#### Enable all the interfaces defined with "auto" in `/etc/network/interfaces`:
```shell
ifup -a
```
{% endraw %}{% raw %}
<h2 id="imgp">
  <a href="/en/linux/imgp.html">imgp</a> <a href="#imgp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line image resizer and rotator for JPEG and PNG images.

#### Convert single images and/or whole directories containing valid image formats:
```shell
imgp -x {{1366x1000}} {{path/to/directory}} {{path/to/file}}
```
#### Scale an image by 75% and overwrite the source image to a target resolution:
```shell
imgp -x {{75}} -w {{path/to/file}}
```
#### Rotate an image clockwise by 90 degrees:
```shell
imgp -o {{90}} {{path/to/file}}
```
{% endraw %}{% raw %}
<h2 id="inotifywait">
  <a href="/en/linux/inotifywait.html">inotifywait</a> <a href="#inotifywait"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Waits for changes to one or more files.

#### Run a command when a file changes:
```shell
while inotifywait {{path/to/file}}; do {{command}}; done
```
#### Be quiet about watching for changes:
```shell
while inotifywait --quiet {{path/to/file}}; do {{command}}; done
```
#### Watch a directory recursively for changes:
```shell
while inotifywait --recursive {{path/to/directory}}; do {{command}}; done
```
#### Exclude files matching a regular expression:
```shell
while inotifywait --recursive {{path/to/directory}} --exlude '{{regular_expression}}'; do {{command}}; done
```
#### Wait at most 30 seconds:
```shell
while inotifywait --timeout {{30}} {{path/to/file}}; do {{command}}; done
```
#### Only watch for file modification events:
```shell
while inotifywait --event {{modify}} {{path/to/file}}; do {{command}}; done
```
{% endraw %}{% raw %}
<h2 id="inxi">
  <a href="/en/linux/inxi.html">inxi</a> <a href="#inxi"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print a summary of system information and resources for debugging purposes.

#### Print a short summary of CPU, memory, hard drive and kernel information:
```shell
inxi
```
#### Print a full description of CPU, memory, disk, network and process information:
```shell
inxi -Fz
```
#### Print information about the distribution's repository:
```shell
inxi -r
```
{% endraw %}{% raw %}
<h2 id="iostat">
  <a href="/en/linux/iostat.html">iostat</a> <a href="#iostat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Report statistics for devices and partitions.

#### Display a report of CPU and disk statistics since system startup:
```shell
iostat
```
#### Display a report of CPU and disk statistics with units converted to megabytes:
```shell
iostat -m
```
#### Display CPU statistics:
```shell
iostat -c
```
#### Display disk statistics with disk names (including LVM):
```shell
iostat -N
```
#### Display extended disk statistics with disk names for device "sda":
```shell
iostat -xN {{sda}}
```
#### Display incremental reports of CPU and disk statistics every 2 seconds:
```shell
iostat {{2}}
```
{% endraw %}{% raw %}
<h2 id="ip-address">
  <a href="/en/linux/ip-address.html">ip address</a> <a href="#ip-address"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> IP Address management subcommand.

#### List network interfaces and their associated IP addresses:
```shell
ip address
```
#### Filter to show only active network interfaces:
```shell
ip address show up
```
#### Display information about a specific network interface:
```shell
ip address show dev {{eth0}}
```
#### Add an IP address to a network interface:
```shell
ip address add {{ip_address}} dev {{eth0}}
```
#### Remove an IP address from a network interface:
```shell
ip address delete {{ip_address}} dev {{eth0}}
```
#### Delete all IP addresses in a given scope from a network interface:
```shell
ip address flush dev {{eth0}} scope {{global|host|link}}
```
{% endraw %}{% raw %}
<h2 id="ip-link">
  <a href="/en/linux/ip-link.html">ip link</a> <a href="#ip-link"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage network interfaces.
> More information: <https://man7.org/linux/man-pages/man8/ip-link.8.html>.

#### Show information about all network interfaces:
```shell
ip link
```
#### Show information about a specific network interface:
```shell
ip link show {{ethN}}
```
#### Bring a network interface up or down:
```shell
ip link set {{ethN}} {{up|down}}
```
#### Give a meaningful name to a network interface:
```shell
ip link set {{ethN}} alias "{{LAN Interface}}"
```
#### Change the MAC address of a network interface:
```shell
ip link set {{ethN}} address {{ff:ff:ff:ff:ff:ff}}
```
#### Change the MTU size for a network interface to use jumbo frames:
```shell
ip link set {{ethN}} mtu {{9000}}
```
{% endraw %}{% raw %}
<h2 id="ip-neighbour">
  <a href="/en/linux/ip-neighbour.html">ip-neighbour</a> <a href="#ip-neighbour"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Neighbour/ARP tables management IP subcommand.
> More information: <https://manned.org/ip-neighbour.8>.

#### Display the neighbour/ARP table entries:
```shell
ip neighbour
```
#### Remove entries in the neighbour table on device `eth0`:
```shell
sudo ip neighbour flush dev {{eth0}}
```
#### Perform a neighbour lookup and return a neighbour entry:
```shell
ip neighbour get {{lookup_ip}} dev {{eth0}}
```
#### Add or delete an ARP entry for the neighbour IP address to `eth0`:
```shell
sudo ip neighbour {{add|del}} {{ip_address}} lladdr {{mac_address}} dev {{eth0}} nud reachable
```
#### Change or replace an ARP entry for the neighbour IP address to `eth0`:
```shell
sudo ip neighbour {{change|replace}} {{ip_address}} lladdr {{new_mac_address}} dev {{eth0}}
```
{% endraw %}{% raw %}
<h2 id="ip-route">
  <a href="/en/linux/ip-route.html">ip route</a> <a href="#ip-route"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> IP Routing table management subcommand.
> More information: <https://manned.org/ip-route>.

#### Display the routing table:
```shell
ip route {{show|list}}
```
#### Add a default route using gateway forwarding:
```shell
sudo ip route add default via {{gateway_ip}}
```
#### Add a default route using `eth0`:
```shell
sudo ip route add default dev {{eth0}}
```
#### Add a static route:
```shell
sudo ip route add {{destination_ip}} via {{gateway_ip}} dev {{eth0}}
```
#### Delete a static route:
```shell
sudo ip route del {{destination_ip}} dev {{eth0}}
```
#### Change or replace a static route:
```shell
sudo ip route {{change|replace}} {{destination_ip}} via {{gateway_ip}} dev {{eth0}}
```
#### Show which route will be used by the kernel to reach an IP address:
```shell
ip route get {{destination_ip}}
```
{% endraw %}{% raw %}
<h2 id="ip">
  <a href="/en/linux/ip.html">ip</a> <a href="#ip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show / manipulate routing, devices, policy routing and tunnels.
> More information: <https://www.man7.org/linux/man-pages/man8/ip.8.html>.

#### List interfaces with detailed info:
```shell
ip address
```
#### List interfaces with brief network layer info:
```shell
ip -brief address
```
#### List interfaces with brief link layer info:
```shell
ip -brief link
```
#### Display the routing table:
```shell
ip route
```
#### Show neighbors (ARP table):
```shell
ip neighbour
```
#### Make an interface up/down:
```shell
ip link set {{interface}} up/down
```
#### Add/Delete an ip address to an interface:
```shell
ip addr add/del {{ip}}/{{mask}} dev {{interface}}
```
#### Add a default route:
```shell
ip route add default via {{ip}} dev {{interface}}
```
{% endraw %}{% raw %}
<h2 id="ipcalc">
  <a href="/en/linux/ipcalc.html">ipcalc</a> <a href="#ipcalc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Perform simple operations and calculations on IP addresses and networks.

#### Show information about an address or network with a given subnet mask:
```shell
ipcalc {{1.2.3.4}} {{255.255.255.0}}
```
#### Show information about an address or network in CIDR notation:
```shell
ipcalc {{1.2.3.4}}/{{24}}
```
#### Show the broadcast address of an address or network:
```shell
ipcalc -b {{1.2.3.4}}/{{30}}
```
#### Show the network address of provided IP address and netmask:
```shell
ipcalc -n {{1.2.3.4}}/{{24}}
```
#### Display geographic information about a given IP address:
```shell
ipcalc -g {{1.2.3.4}}
```
{% endraw %}{% raw %}
<h2 id="ipcmk">
  <a href="/en/linux/ipcmk.html">ipcmk</a> <a href="#ipcmk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create IPC (Inter-process Communication) resources.

#### Create a shared memory segment:
```shell
ipcmk --shmem {{segment_size_in_bytes}}
```
#### Create a semaphore:
```shell
ipcmk --semaphore {{element_size}}
```
#### Create a message queue:
```shell
ipcmk --queue
```
#### Create a shared memory segment with specific permissions (default is 0644):
```shell
ipcmk --shmem {{segment_size_in_bytes}} {{octal_permissons}}
```
{% endraw %}{% raw %}
<h2 id="ipcrm">
  <a href="/en/linux/ipcrm.html">ipcrm</a> <a href="#ipcrm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Delete IPC (Inter-process Communication) resources.

#### Delete a shared memory segment by ID:
```shell
ipcrm --shmem-id {{shmem_id}}
```
#### Delete a shared memory segment by key:
```shell
ipcrm --shmem-key {{shmem_key}}
```
#### Delete an IPC queue by ID:
```shell
ipcrm --queue-id {{ipc_queue_id}}
```
#### Delete an IPC queue by key:
```shell
ipcrm --queue-key {{ipc_queue_key}}
```
#### Delete a semaphore by ID:
```shell
ipcrm --semaphore-id {{semaphore_id}}
```
#### Delete a semaphore by key:
```shell
ipcrm --semaphore-key {{semaphore_key}}
```
#### Delete all IPC resources:
```shell
ipcrm --all
```
{% endraw %}{% raw %}
<h2 id="iptables">
  <a href="/en/linux/iptables.html">iptables</a> <a href="#iptables"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Program that allows configuration of tables, chains and rules provided by the Linux kernel firewall.
> More information: <https://www.netfilter.org/projects/iptables/>.

#### View chains, rules, and packet/byte counters for the filter table:
```shell
sudo iptables -vnL
```
#### Set chain policy rule:
```shell
sudo iptables -P {{chain}} {{rule}}
```
#### Append rule to chain policy for IP:
```shell
sudo iptables -A {{chain}} -s {{ip}} -j {{rule}}
```
#### Append rule to chain policy for IP considering protocol and port:
```shell
sudo iptables -A {{chain}} -s {{ip}} -p {{protocol}} --dport {{port}} -j {{rule}}
```
#### Delete chain rule:
```shell
sudo iptables -D {{chain}} {{rule_line_number}}
```
#### Save iptables configuration of a given table to a file:
```shell
sudo iptables-save -t {{tablename}} > {{path/to/iptables_file}}
```
#### Restore iptables configuration from a file:
```shell
sudo iptables-restore < {{path/to/iptables_file}}
```
{% endraw %}{% raw %}
<h2 id="isoinfo">
  <a href="/en/linux/isoinfo.html">isoinfo</a> <a href="#isoinfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility programs for dumping and verifying ISO disk images.

#### List all the files included in an ISO image:
```shell
isoinfo -f -i {{path/to/image.iso}}
```
#### E[x]tract a specific file from an ISO image and send it out stdout:
```shell
isoinfo -i {{path/to/image.iso}} -x {{/PATH/TO/FILE/INSIDE/ISO.EXT}}
```
#### Show header information for an ISO disk image:
```shell
isoinfo -d -i {{path/to/image.iso}}
```
{% endraw %}{% raw %}
<h2 id="isosize">
  <a href="/en/linux/isosize.html">isosize</a> <a href="#isosize"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display the size of an ISO file.
> More information: <https://manned.org/isosize>.

#### Display the size of an ISO file:
```shell
isosize {{path/to/file.iso}}
```
#### Display the block count and block size of an ISO file:
```shell
isosize --sectors {{path/to/file.iso}}
```
#### Display the size of an ISO file divided by a given number (only usable when --sectors is not given):
```shell
isosize --divisor={{number}} {{path/to/file.iso}}
```
{% endraw %}{% raw %}
<h2 id="iw">
  <a href="/en/linux/iw.html">iw</a> <a href="#iw"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show and manipulate wireless devices.

#### Scan for available wireless networks:
```shell
iw dev {{wlp}} scan
```
#### Join an open wireless network:
```shell
iw dev {{wlp}} connect {{SSID}}
```
#### Close the current connection:
```shell
iw dev {{wlp}} disconnect
```
#### Show information about the current connection:
```shell
iw dev {{wlp}} link
```
{% endraw %}{% raw %}
<h2 id="iwconfig">
  <a href="/en/linux/iwconfig.html">iwconfig</a> <a href="#iwconfig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Configure and show the parameters of a wireless network interface.
> More information: <https://manned.org/iwconfig>.

#### Show the parameters and statistics of all the interfaces:
```shell
iwconfig
```
#### Show the parameters and statistics of the specified interface:
```shell
iwconfig {{interface}}
```
#### Set the ESSID (network name) of the specified interface (e.g., eth0 or wlp2s0):
```shell
iwconfig {{interface}} {{new_network_name}}
```
#### Set the operating mode of the specified interface:
```shell
iwconfig {{interface}} mode {{ad hoc|Managed|Master|Repeater|Secondary|Monitor|Auto}}
```
{% endraw %}{% raw %}
<h2 id="iwctl">
  <a href="/en/linux/iwctl.html">iwctl</a> <a href="#iwctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line tool for controlling the iwd network supplicant.
> More information: <https://iwd.wiki.kernel.org/gettingstarted>.

#### Start the interactive mode, in this mode you can enter the commands directly, with autocompletion:
```shell
iwctl
```
#### Call general help:
```shell
iwctl --help
```
#### Display your wifi stations:
```shell
iwctl station list
```
#### Start looking for networks with a station:
```shell
iwctl station {{station}} scan
```
#### Display the networks found by a station:
```shell
iwctl station {{station}} get-networks
```
#### Connect to a network with a station, if credentials are needed they will be asked:
```shell
iwctl station {{station}} connect {{network_name}}
```
{% endraw %}{% raw %}
<h2 id="jobs">
  <a href="/en/linux/jobs.html">jobs</a> <a href="#jobs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> BASH builtin for viewing information about processes spawned by the current shell.

#### View jobs spawned by the current shell:
```shell
jobs
```
#### List jobs and their process ids:
```shell
jobs -l
```
#### Display information about jobs with changed status:
```shell
jobs -n
```
#### Display process id of process group leader:
```shell
jobs -p
```
#### Display running processes:
```shell
jobs -r
```
#### Display stopped processes:
```shell
jobs -s
```
{% endraw %}{% raw %}
<h2 id="journalctl">
  <a href="/en/linux/journalctl.html">journalctl</a> <a href="#journalctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Query the systemd journal.

#### Show all messages from this [b]oot:
```shell
journalctl -b
```
#### Show all messages from last [b]oot:
```shell
journalctl -b -1
```
#### Show all messages with priority level 3 (errors) from this [b]oot:
```shell
journalctl -b --priority={{3}}
```
#### [f]ollow new messages (like `tail -f` for traditional syslog):
```shell
journalctl -f
```
#### Show all messages by a specific [u]nit:
```shell
journalctl -u {{unit}}
```
#### Filter messages within a time range (either timestamp or placeholders like "yesterday"):
```shell
journalctl --since {{now|today|yesterday|tomorrow}} --until {{YYYY-MM-DD HH:MM:SS}}
```
#### Show all messages by a specific process:
```shell
journalctl _PID={{pid}}
```
#### Show all messages by a specific executable:
```shell
journalctl {{path/to/executable}}
```
{% endraw %}{% raw %}
<h2 id="jpegtran">
  <a href="/en/linux/jpegtran.html">jpegtran</a> <a href="#jpegtran"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Perform lossless transformation of JPEG files.
> More information: <https://manned.org/jpegtran>.

#### Mirror an image horizontally or vertically:
```shell
jpegtran -flip {{horizontal|vertical}} {{path/to/image.jpg}} > {{path/to/output.jpg}}
```
#### Rotate an image 90, 180 or 270 degrees clockwise:
```shell
jpegtran -rotate {{90|180|270}} {{path/to/image.jpg}} > {{path/to/output.jpg}}
```
#### Transpose the image across the upper left to lower right axis:
```shell
jpegtran -transpose {{path/to/image.jpg}} > {{path/to/output.jpg}}
```
#### Transverse the image across the upper right to lower left axis:
```shell
jpegtran -transverse {{path/to/image.jpg}} > {{path/to/output.jpg}}
```
#### Convert the image to grayscale:
```shell
jpegtran -grayscale {{path/to/image.jpg}} > {{path/to/output.jpg}}
```
#### Crop the image to a rectangular region of width `W` and height `H` from the upper left corner, saving the output to a specific file:
```shell
jpegtran -crop {{W}}x{{H}} -outfile {{path/to/output.jpg}} {{path/to/image.jpg}}
```
#### Crop the image to a rectangular region of width `W` and height `H`, starting at point `X` and `Y` from the upper left corner:
```shell
jpegtran -crop {{W}}x{{H}}+{{X}}+{{Y}} {{path/to/image.jpg}} > {{path/to/output.jpg}}
```
{% endraw %}{% raw %}
<h2 id="kde-inhibit">
  <a href="/en/linux/kde-inhibit.html">kde-inhibit</a> <a href="#kde-inhibit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Inhibit various desktop functions while a command runs.

#### Inhibit power management:
```shell
kde-inhibit --power {{command}} {{command_arguments}}
```
#### Inhibit screen saver:
```shell
kde-inhibit --screenSaver {{command}} {{command_arguments}}
```
#### Launch vlc, and inhibit colour correction (night mode) while it's running:
```shell
kde-inhibit --colorCorrect {{vlc}}
```
{% endraw %}{% raw %}
<h2 id="kdocker">
  <a href="/en/linux/kdocker.html">kdocker</a> <a href="#kdocker"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Easily dock applications to the system tray.
> More information: <https://github.com/user-none/KDocker>.

#### Display a cursor to send a window to the system tray when pressing the left mouse button (press any other mouse button to cancel):
```shell
kdocker
```
#### Open an application and send it to the system tray:
```shell
kdocker {{application}}
```
#### Send focused window to the system tray:
```shell
kdocker -f
```
#### Display a cursor to send a window to the system tray with a custom icon when pressing the left mouse button:
```shell
kdocker -i {{/path/to/icon}}
```
#### Open an application, send it to the system tray and if focus is lost, minimize it:
```shell
kdocker -l {{application}}
```
#### Print version:
```shell
kdocker --version
```
{% endraw %}{% raw %}
<h2 id="kexec">
  <a href="/en/linux/kexec.html">kexec</a> <a href="#kexec"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Directly reboot into a new kernel.

#### Load a new kernel:
```shell
kexec -l {{path/to/kernel}} --initrd={{path/to/initrd}} --command-line={{arguments}}
```
#### Load a new kernel with current boot parameters:
```shell
kexec -l {{path/to/kernel}} --initrd={{path/to/initrd}} --reuse-cmdline
```
#### Execute a currently loaded kernel:
```shell
kexec -e
```
#### Unload current kexec target kernel:
```shell
kexec -u
```
{% endraw %}{% raw %}
<h2 id="kjv">
  <a href="/en/linux/kjv.html">kjv</a> <a href="#kjv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The word of God available right on your desktop.
> More information: <https://github.com/bontibon/kjv>.

#### Display books:
```shell
kjv -l
```
#### Open a specific book:
```shell
kjv {{Genesis}}
```
#### Open a specific chapter of a book:
```shell
kjv {{Genesis}} {{2}}
```
#### Open a specific verse of a specific chapter of a book:
```shell
kjv {{John}} {{3}}:{{16}}
```
#### Open a specific range of verses of a book's chapter:
```shell
kjv {{Proverbs}} {{3}}:{{1-6}}
```
#### Display a specific range of verses of a book from different chapters:
```shell
kjv {{Matthew}} {{1}}:{{7}}-{{2}}:{{6}}
```
#### Display all verses that match a pattern:
```shell
kjv /{{Plagues}}
```
#### Display all verses that match a pattern in a specific book:
```shell
kjv {{1Jn}}/{{antichrist}}
```
{% endraw %}{% raw %}
<h2 id="konsole">
  <a href="/en/linux/konsole.html">konsole</a> <a href="#konsole"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Konsole: The KDE terminal emulator.
> More information: <https://konsole.kde.org>.

#### Open a new Konsole in a specific directory:
```shell
konsole --workdir {{path/to/directory}}
```
#### Run a specific command and do not close the window after it exits:
```shell
konsole --noclose -e {{command}}
```
#### Open a new tab:
```shell
konsole --new-tab
```
#### Open a Konsole in the background and bring to the front when Ctrl+Shift+F12 (by default) is pressed:
```shell
konsole --background-mode
```
#### Open a Konsole with the emergency FALLBACK profile:
```shell
konsole --fallback-profile
```
{% endraw %}{% raw %}
<h2 id="kpackagetool5">
  <a href="/en/linux/kpackagetool5.html">kpackagetool5</a> <a href="#kpackagetool5"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> KPackage Manager: Install, list, remove Plasma packages.
> More information: <https://techbase.kde.org/Development/Tutorials/Plasma5/QML2/GettingStarted#Kpackagetool5>.

#### List all known package types that can be installed:
```shell
kpackagetool5 --list-types
```
#### Install the package from a directory:
```shell
kpackagetool5 --type {{package_type}} --install {{path/to/directory}}
```
#### Update installed package from a directory:
```shell
kpackagetool5 --type {{package_type}} --upgrade {{path/to/directory}}
```
#### List installed plasmoids (--global for all users):
```shell
kpackagetool5 --type Plasma/Applet --list --global
```
#### Remove a plasmoid by name:
```shell
kpackagetool5 --type Plasma/Applet --remove "{{name}}"
```
{% endraw %}{% raw %}
<h2 id="kpartx">
  <a href="/en/linux/kpartx.html">kpartx</a> <a href="#kpartx"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create device maps from partition tables.

#### Add partition mappings:
```shell
kpartx -a {{whole_disk.img}}
```
#### Delete partition mappings:
```shell
kpartx -d {{whole_disk.img}}
```
#### List partition mappings:
```shell
kpartx -l {{whole_disk.img}}
```
{% endraw %}{% raw %}
<h2 id="kreadconfig5">
  <a href="/en/linux/kreadconfig5.html">kreadconfig5</a> <a href="#kreadconfig5"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Read KConfig entries for KDE Plasma.
> More information: <https://userbase.kde.org/KDE_System_Administration/Configuration_Files>.

#### Read a key from the global configuration:
```shell
kreadconfig5 --group {{group_name}} --key {{key_name}}
```
#### Read a key from a specific configuration file:
```shell
kwriteconfig5 --file {{path/to/file}} --group {{group_name}} --key {{key_name}}
```
#### Check if systemd is used to start the Plasma session:
```shell
kreadconfig5 --file {{startkderc}} --group {{General}} --key {{systemdBoot}}
```
{% endraw %}{% raw %}
<h2 id="ksvgtopng5">
  <a href="/en/linux/ksvgtopng5.html">ksvgtopng5</a> <a href="#ksvgtopng5"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Convert SVG files to PNG format.
> More information: <https://invent.kde.org/plasma/kde-cli-tools/-/blob/master/ksvgtopng/ksvgtopng.cpp>.

#### Convert an SVG file (should be an absolute path) to PNG:
```shell
ksvgtopng5 {{width}} {{height}} {{path/to/file.svg}} {{output_filename.png}}
```
{% endraw %}{% raw %}
<h2 id="kwriteconfig5">
  <a href="/en/linux/kwriteconfig5.html">kwriteconfig5</a> <a href="#kwriteconfig5"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Write KConfig entries for KDE Plasma.
> More information: <https://userbase.kde.org/KDE_System_Administration/Configuration_Files>.

#### Display help:
```shell
kwriteconfig5 --help
```
#### Set a global configuration key:
```shell
kwriteconfig5 --group {{group_name}} --key {{key}} {{value}}
```
#### Set a key in a specific configuration file:
```shell
kwriteconfig5 --file {{path/to/file}} --group {{group_name}} --key {{key}} {{value}}
```
#### Delete a key:
```shell
kwriteconfig5 --group {{group_name}} --key {{key}} --delete
```
#### Use systemd to start the Plasma session when available:
```shell
kwriteconfig5 --file {{startkderc}} --group {{General}} --key {{systemdBoot}} {{true}}
```
#### Hide the title bar when a window is maximized (like Ubuntu):
```shell
kwriteconfig5 --file {{~/.config/kwinrc}} --group {{Windows}} --key {{BorderlessMaximizedWindows}} {{true}}
```
#### Configure KRunner to open with the Meta (Command/Windows) global hotkey:
```shell
kwriteconfig5 --file {{~/.config/kwinrc}} --group {{ModifierOnlyShortcuts}} --key {{Meta}} {{"org.kde.kglobalaccel,/component/krunner_desktop,org.kde.kglobalaccel.Component,invokeShortcut,_launch"}}
```
{% endraw %}{% raw %}
<h2 id="larasail">
  <a href="/en/linux/larasail.html">larasail</a> <a href="#larasail"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A CLI tool for managing Laravel on Digital Ocean servers.
> More information: <https://github.com/thedevdojo/larasail>.

#### Set up the server with Laravel dependencies using the default PHP version:
```shell
larasail setup
```
#### Set up the server with Laravel dependencies using a specific PHP version:
```shell
larasail setup {{php71}}
```
#### Add a new Laravel site:
```shell
larasail host {{domain}} {{path/to/site_directory}}
```
#### Retrieve the Larasail user password:
```shell
larasail pass
```
#### Retrieve the Larasail MySQL password:
```shell
larasail mysqlpass
```
{% endraw %}{% raw %}
<h2 id="lastb">
  <a href="/en/linux/lastb.html">lastb</a> <a href="#lastb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show a listing of last logged in users.

#### Show a list of all last logged in users:
```shell
sudo lastb
```
#### Show a list of all last logged in users since a given time:
```shell
sudo lastb --since {{YYYY-MM-DD}}
```
#### Show a list of all last logged in users until a given time:
```shell
sudo lastb --until {{YYYY-MM-DD}}
```
#### Show a list of all logged in users at a specific time:
```shell
sudo lastb --present {{hh:mm}}
```
#### Show a list of all last logged in users and translate the IP into a hostname:
```shell
sudo lastb --dns
```
{% endraw %}{% raw %}
<h2 id="lastcomm">
  <a href="/en/linux/lastcomm.html">lastcomm</a> <a href="#lastcomm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show last commands executed.
> More information: <https://manpages.debian.org/stable/acct/lastcomm.1.en.html>.

#### Print information about all of the commands in the acct (record file):
```shell
lastcomm
```
#### Display commands executed by a given user:
```shell
lastcomm --user {{user}}
```
#### Display information about a given command executed on the system:
```shell
lastcomm --command {{command}}
```
#### Display information about commands executed on a given terminal:
```shell
lastcomm --tty {{terminal_name}}
```
{% endraw %}{% raw %}
<h2 id="lastlog">
  <a href="/en/linux/lastlog.html">lastlog</a> <a href="#lastlog"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show the most recent login of all users or of a given user.

#### Display the most recent login of all users:
```shell
lastlog
```
#### Display lastlog record of the specified user:
```shell
lastlog -u {{username}}
```
#### Display records before than 7 days:
```shell
lastlog -b {{7}}
```
#### Display records more recent than 3 days:
```shell
lastlog -t {{3}}
```
{% endraw %}{% raw %}
<h2 id="ldconfig">
  <a href="/en/linux/ldconfig.html">ldconfig</a> <a href="#ldconfig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Configure symlinks and cache for shared library dependencies.

#### Update symlinks and rebuild the cache (usually run when a new library is installed):
```shell
sudo ldconfig
```
#### Update the symlinks for a given directory:
```shell
sudo ldconfig -n {{path/to/directory}}
```
#### Print the libraries in the cache and check whether a given library is present:
```shell
ldconfig -p | grep {{library_name}}
```
{% endraw %}{% raw %}
<h2 id="ldd">
  <a href="/en/linux/ldd.html">ldd</a> <a href="#ldd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display shared library dependencies.

#### Display shared library dependencies of a binary:
```shell
ldd {{path/to/binary}}
```
#### Display unused direct dependencies:
```shell
ldd -u {{path/to/binary}}
```
{% endraw %}{% raw %}
<h2 id="legit">
  <a href="/en/linux/legit.html">legit</a> <a href="#legit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Complementary command-line interface for Git.
> More information: <https://frostming.github.io/legit>.

#### Switch to a specified branch, stashing and restoring unstaged changes:
```shell
git switch {{target_branch}}
```
#### Synchronize current branch, automatically merging or rebasing, and stashing and unstashing:
```shell
git sync
```
#### Publish a specified branch to the remote server:
```shell
git publish {{branch_name}}
```
#### Remove a branch from the remote server:
```shell
git unpublish {{branch_name}}
```
#### List all branches and their publication status:
```shell
git branches {{glob_pattern}}
```
#### Remove the last commit from the history:
```shell
git undo {{--hard}}
```
{% endraw %}{% raw %}
<h2 id="lftp">
  <a href="/en/linux/lftp.html">lftp</a> <a href="#lftp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sophisticated file transfer program.
> More information: <https://lftp.yar.ru/lftp-man.html>.

#### Connect to an FTP server:
```shell
lftp {{ftp.example.com}}
```
#### Download multiple files (glob expression):
```shell
mget {{path/to/*.png}}
```
#### Upload multiple files (glob expression):
```shell
mput {{path/to/*.zip}}
```
#### Delete multiple files on the remote server:
```shell
mrm {{path/to/*.txt}}
```
#### Rename a file on the remote server:
```shell
mv {{original_filename}} {{new_filename}}
```
#### Download or update an entire directory:
```shell
mirror {{path/to/remote_dir}} {{path/to/local_output_dir}}
```
#### Upload or update an entire directory:
```shell
mirror -R {{path/to/local_dir}} {{path/to/remote_output_dir}}
```
{% endraw %}{% raw %}
<h2 id="libreoffice">
  <a href="/en/linux/libreoffice.html">libreoffice</a> <a href="#libreoffice"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI for the powerful and free office suite LibreOffice.
> More information: <https://www.libreoffice.org/>.

#### Open a space-separated list of files in read-only mode:
```shell
libreoffice --view {{path/to/file1}} {{path/to/file2}}
```
#### Display the content of specific files:
```shell
libreoffice --cat {{path/to/file1}} {{path/to/file2}}
```
#### Print files to a specific printer:
```shell
libreoffice --pt {{printer_name}} {{path/to/file1}} {{path/to/file2}}
```
#### Convert all `.doc` files in current directory to pdf:
```shell
libreoffice --convert-to {{pdf}} {{*.doc}}
```
{% endraw %}{% raw %}
<h2 id="light">
  <a href="/en/linux/light.html">light</a> <a href="#light"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI to control the backlight of your screen.

#### Get the current backlight value in percent:
```shell
light
```
#### Set the backlight value to 50 percent:
```shell
light -S {{50}}
```
#### Reduce 20 percent from the current backlight value:
```shell
light -U {{20}}
```
#### Add 20 percent to the current backlight value:
```shell
light -A {{20}}
```
{% endraw %}{% raw %}
<h2 id="line">
  <a href="/en/linux/line.html">line</a> <a href="#line"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Read a single line of input.

#### Read input:
```shell
line
```
{% endraw %}{% raw %}
<h2 id="locate">
  <a href="/en/linux/locate.html">locate</a> <a href="#locate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Find filenames quickly.

#### Look for pattern in the database. Note: the database is recomputed periodically (usually weekly or daily):
```shell
locate {{pattern}}
```
#### Look for a file by its exact filename (a pattern containing no globbing characters is interpreted as `*pattern*`):
```shell
locate */{{filename}}
```
#### Recompute the database. You need to do it if you want to find recently added files:
```shell
sudo updatedb
```
{% endraw %}{% raw %}
<h2 id="logger">
  <a href="/en/linux/logger.html">logger</a> <a href="#logger"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Add messages to syslog (/var/log/syslog).

#### Log a message to syslog:
```shell
logger {{message}}
```
#### Take input from stdin and log to syslog:
```shell
echo {{log_entry}} | logger
```
#### Send the output to a remote syslog server running at a given port. Default port is 514:
```shell
echo {{log_entry}} | logger --server {{hostname}} --port {{port}}
```
#### Use a specific tag for every line logged. Default is the name of logged in user:
```shell
echo {{log_entry}} | logger --tag {{tag}}
```
#### Log messages with a given priority. Default is `user.notice`. See `man logger` for all priority options:
```shell
echo {{log_entry}} | logger --priority {{user.warning}}
```
{% endraw %}{% raw %}
<h2 id="login">
  <a href="/en/linux/login.html">login</a> <a href="#login"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Initiates a session for a user.

#### Log in as a user:
```shell
login {{user}}
```
#### Log in as user without authentication if user is preauthenticated:
```shell
login -f {{user}}
```
#### Log in as user and preserve environment:
```shell
login -p {{user}}
```
#### Log in as a user on a remote host:
```shell
login -h {{host}} {{user}}
```
{% endraw %}{% raw %}
<h2 id="logsave">
  <a href="/en/linux/logsave.html">logsave</a> <a href="#logsave"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Save the output of a command in a logfile.
> More information: <https://manned.org/logsave>.

#### Execute command with specified argument(s) and save its output to log file:
```shell
logsave {{path/to/logfile}} {{command}}
```
#### Take input from standard input and save it in a log file:
```shell
logsave {{logfile}} -
```
#### Append the output to a log file, instead of replacing its current contents:
```shell
logsave -a {{logfile}} {{command}}
```
#### Show verbose output:
```shell
logsave -v {{logfile}} {{command}}
```
{% endraw %}{% raw %}
<h2 id="logwatch">
  <a href="/en/linux/logwatch.html">logwatch</a> <a href="#logwatch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Summarizes many different logs for common services (e.g., apache, pam_unix, sshd, etc.) in a single report.

#### Analyze logs for a range of dates at certain level of detail:
```shell
logwatch --range {{yesterday|today|all|help}} --detail {{low|medium|others}}'
```
#### Restrict report to only include information for a selected service:
```shell
logwatch --range {{all}} --service {{apache|pam_unix|etc}}
```
{% endraw %}{% raw %}
<h2 id="losetup">
  <a href="/en/linux/losetup.html">losetup</a> <a href="#losetup"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Set up and control loop devices.

#### List loop devices with detailed info:
```shell
losetup -a
```
#### Attach a file to a given loop device:
```shell
sudo losetup /dev/{{loop}} /{{path/to/file}}
```
#### Attach a file to a new free loop device and scan the device for partitions:
```shell
sudo losetup --show --partscan -f /{{path/to/file}}
```
#### Attach a file to a read-only loop device:
```shell
sudo losetup --read-only /dev/{{loop}} /{{path/to/file}}
```
#### Detach all loop devices:
```shell
sudo losetup -D
```
#### Detach a given loop device:
```shell
sudo losetup -d /dev/{{loop}}
```
{% endraw %}{% raw %}
<h2 id="lrunzip">
  <a href="/en/linux/lrunzip.html">lrunzip</a> <a href="#lrunzip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A large file decompression program.
> See also `lrzip`, `lrztar`, `lrzuntar`.

#### Decompress a file:
```shell
lrunzip {{filename.lrz}}
```
#### Decompress a file using a specific number of processor threads:
```shell
lrunzip -p {{8}} {{filename.lrz}}
```
#### Decompress a file and silently overwrite files if they exist:
```shell
lrunzip -f {{filename.lrz}}
```
#### Keep broken or damaged files instead of deleting them when decompressing:
```shell
lrunzip -K {{filename.lrz}}
```
#### Specify output file name and/or path:
```shell
lrunzip -o {{outfilename}} {{filename.lrz}}
```
{% endraw %}{% raw %}
<h2 id="lrzip">
  <a href="/en/linux/lrzip.html">lrzip</a> <a href="#lrzip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A large file compression program.
> See also `lrunzip`, `lrztar`, `lrzuntar`.

#### Compress a file with LZMA - slow compression, fast decompression:
```shell
lrzip {{filename}}
```
#### Compress a file with BZIP2 - good middle ground for compression/speed:
```shell
lrzip -b {{filename}}
```
#### Compress with ZPAQ - extreme compression, but very slow:
```shell
lrzip -z {{filename}}
```
#### Compress with LZO - light compression, extremely fast decompression:
```shell
lrzip -l {{filename}}
```
#### Compress a file and password protect/encrypt it:
```shell
lrzip -e {{filename}}
```
#### Override the number of processor threads to use:
```shell
lrzip -p {{8}} {{filename}}
```
{% endraw %}{% raw %}
<h2 id="lrztar">
  <a href="/en/linux/lrztar.html">lrztar</a> <a href="#lrztar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A wrapper for `lrzip` to simplify compression of directories.
> See also: `tar`, `lrzuntar`, `lrunzip`.

#### Archive a directory with `tar`, then compress:
```shell
lrztar {{path/to/directory}}
```
#### Same as above, with ZPAQ - extreme compression, but very slow:
```shell
lrztar -z {{path/to/directory}}
```
#### Specify the output file:
```shell
lrztar -o {{path/to/file}} {{path/to/directory}}
```
#### Override the number of processor threads to use:
```shell
lrztar -p {{8}} {{path/to/directory}}
```
#### Force overwriting of existing files:
```shell
lrztar -f {{path/to/directory}}
```
{% endraw %}{% raw %}
<h2 id="lrzuntar">
  <a href="/en/linux/lrzuntar.html">lrzuntar</a> <a href="#lrzuntar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A wrapper for `lrunzip` to simplify decompression of directories.
> See also: `lrztar`, `lrzip`.

#### Decompress from a file to the current directory:
```shell
lrzuntar {{path/to/archive.tar.lrz}}
```
#### Decompress from a file to the current directory using a specific number of processor threads:
```shell
lrzuntar -p {{8}} {{path/to/archive.tar.lrz}}
```
#### Decompress from a file to the current directory and silently overwrite items that already exist:
```shell
lrzuntar -f {{archive.tar.lrz}}
```
#### Specify the output path:
```shell
lrzuntar -O {{path/to/directory}} {{archive.tar.lrz}}
```
#### Delete the compressed file after decompression:
```shell
lrzuntar -D {{path/to/archive.tar.lrz}}
```
{% endraw %}{% raw %}
<h2 id="lsattr">
  <a href="/en/linux/lsattr.html">lsattr</a> <a href="#lsattr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List file attributes on a Linux filesystem.

#### Display the attributes of the files in the current directory:
```shell
lsattr
```
#### List the attributes of files in a particular path:
```shell
lsattr {{path}}
```
#### List file attributes recursively in the current and subsequent directories:
```shell
lsattr -R
```
#### Show attributes of all the files in the current directory, including hidden ones:
```shell
lsattr -a
```
#### Display attributes of directories in the current directory:
```shell
lsattr -d
```
{% endraw %}{% raw %}
<h2 id="lsb_release">
  <a href="/en/linux/lsb_release.html">lsb_release</a> <a href="#lsb_release"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Provides certain LSB (Linux Standard Base) and distribution-specific information.

#### Print all available information:
```shell
lsb_release -a
```
#### Print a description (usually the full name) of the operating system:
```shell
lsb_release -d
```
#### Print only the operating system name (ID), suppressing the field name:
```shell
lsb_release -i -s
```
#### Print the release number and codename of the distribution, suppressing the field names:
```shell
lsb_release -rcs
```
{% endraw %}{% raw %}
<h2 id="lsblk">
  <a href="/en/linux/lsblk.html">lsblk</a> <a href="#lsblk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lists information about devices.

#### List all storage devices in a tree-like format:
```shell
lsblk
```
#### Also list empty devices:
```shell
lsblk -a
```
#### Print the SIZE column in bytes rather than in a human-readable format:
```shell
lsblk -b
```
#### Output info about filesystems:
```shell
lsblk -f
```
#### Use ASCII characters for tree formatting:
```shell
lsblk -i
```
#### Output info about block-device topology:
```shell
lsblk -t
```
#### Exclude the devices specified by the comma-separated list of major device numbers:
```shell
lsblk -e {{1,7}}
```
#### Display a customized summary using a comma-separated list of columns:
```shell
lsblk --output {{NAME}},{{SERIAL}},{{MODEL}},{{TRAN}},{{TYPE}},{{SIZE}},{{FSTYPE}},{{MOUNTPOINT}}
```
{% endraw %}{% raw %}
<h2 id="lscpu">
  <a href="/en/linux/lscpu.html">lscpu</a> <a href="#lscpu"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Displays information about the CPU architecture.

#### Display information about all CPUs:
```shell
lscpu
```
#### Display information in a table:
```shell
lscpu --extended
```
#### Display only information about offline CPUs in a table:
```shell
lscpu --extended --offline
```
{% endraw %}{% raw %}
<h2 id="lshw">
  <a href="/en/linux/lshw.html">lshw</a> <a href="#lshw"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List detailed information about hardware configurations as root user.

#### Launch the GUI:
```shell
sudo lshw -X
```
#### List all hardwares in tabular format:
```shell
sudo lshw -short
```
#### List all disks and storage controllers in tabular format:
```shell
sudo lshw -class disk -class storage -short
```
#### Save all network interfaces to an HTML file:
```shell
sudo lshw -class network -html > {{interfaces.html}}
```
{% endraw %}{% raw %}
<h2 id="lslocks">
  <a href="/en/linux/lslocks.html">lslocks</a> <a href="#lslocks"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List local system locks.

#### List all local system locks:
```shell
lslocks
```
#### List locks with defined column headers:
```shell
lslocks --output {{PID}},{{COMMAND}},{{PATH}}
```
#### List locks producing a raw output (no columns), and without column headers:
```shell
lslocks --raw --noheadings
```
#### List locks by PID input:
```shell
lslocks --pid {{PID}}
```
#### List locks with json output to stdout:
```shell
lslocks --json
```
{% endraw %}{% raw %}
<h2 id="lslogins">
  <a href="/en/linux/lslogins.html">lslogins</a> <a href="#lslogins"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show information about users on a Linux system.
> More information: <https://man7.org/linux/man-pages/man1/lslogins.1.html>.

#### Display users in the system:
```shell
lslogins
```
#### Display users belonging to a specific group:
```shell
lslogins --groups={{groups}}
```
#### Display user accounts:
```shell
lslogins --user-accs
```
#### Display last logins:
```shell
lslogins --last
```
#### Display system accounts:
```shell
lslogins --system-accs
```
#### Display supplementary groups:
```shell
lslogins --supp-groups
```
{% endraw %}{% raw %}
<h2 id="lsmod">
  <a href="/en/linux/lsmod.html">lsmod</a> <a href="#lsmod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Shows the status of linux kernel modules.
> See also `modprobe`, which loads kernel modules.

#### List all currently loaded kernel modules:
```shell
lsmod
```
{% endraw %}{% raw %}
<h2 id="lspci">
  <a href="/en/linux/lspci.html">lspci</a> <a href="#lspci"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List all PCI devices.

#### Show a brief list of devices:
```shell
lspci
```
#### Display additional info:
```shell
lspci -v
```
#### Display drivers and modules handling each device:
```shell
lspci -k
```
#### Show a specific device:
```shell
lspci -s {{00:18.3}}
```
#### Dump info in a readable form:
```shell
lspci -vm
```
{% endraw %}{% raw %}
<h2 id="lsscsi">
  <a href="/en/linux/lsscsi.html">lsscsi</a> <a href="#lsscsi"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List SCSI devices (or hosts) and their attributes.

#### List all SCSI devices:
```shell
lsscsi
```
#### List all SCSI devices with detailed attributes:
```shell
lsscsi -L
```
#### List all SCSI devices with human readable disk capacity:
```shell
lsscsi -s
```
{% endraw %}{% raw %}
<h2 id="lsusb">
  <a href="/en/linux/lsusb.html">lsusb</a> <a href="#lsusb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display information about USB buses and devices connected to them.

#### List all the USB devices available:
```shell
lsusb
```
#### List the USB hierarchy as a tree:
```shell
lsusb -t
```
#### List verbose information about USB devices:
```shell
lsusb --verbose
```
#### List detailed information about a USB device:
```shell
lsusb -D {{device}}
```
#### List devices with a specified vendor and product id only:
```shell
lsusb -d {{vendor}}:{{product}}
```
{% endraw %}{% raw %}
<h2 id="ltrace">
  <a href="/en/linux/ltrace.html">ltrace</a> <a href="#ltrace"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display dynamic library calls of a process.
> More information: <https://manned.org/ltrace>.

#### Print (trace) library calls of a program binary:
```shell
ltrace ./{{program}}
```
#### Count library calls. Print a handy summary at the bottom:
```shell
ltrace -c {{path/to/program}}
```
#### Trace calls to malloc and free, omit those done by libc:
```shell
ltrace -e malloc+free-@libc.so* {{path/to/program}}
```
#### Write to file instead of terminal:
```shell
ltrace -o {{file}} {{path/to/program}}
```
{% endraw %}{% raw %}
<h2 id="lvcreate">
  <a href="/en/linux/lvcreate.html">lvcreate</a> <a href="#lvcreate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Creates a logical volume in an existing volume group. A volume group is a collection of logical and physical volumes.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/lvcreate.8.html>.

#### Create a logical volume of 10 gigabytes in the volume group vg1:
```shell
lvcreate -L {{10G}} {{vg1}}
```
#### Create a 1500 megabyte linear logical volume named mylv in the volume group vg1:
```shell
lvcreate -L {{1500}} -n {{mylv}} {{vg1}}
```
#### Create a logical volume called mylv that uses 60% of the total space in volume group vg1:
```shell
lvcreate -l {{60%VG}} -n {{mylv}} {{vg1}}
```
#### Create a logical volume called mylv that uses all of the unallocated space in the volume group vg1:
```shell
lvcreate -l {{100%FREE}} -n {{mylv}} {{vg1}}
```
{% endraw %}{% raw %}
<h2 id="lvdisplay">
  <a href="/en/linux/lvdisplay.html">lvdisplay</a> <a href="#lvdisplay"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display information about Logical Volume Manager (LVM) logical volumes.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/lvdisplay.8.html>.

#### Display information about all logical volumes:
```shell
sudo lvdisplay
```
#### Display information about all logical volumes in volume group vg1:
```shell
sudo lvdisplay {{vg1}}
```
#### Display information about logical volume lv1 in volume group vg1:
```shell
sudo lvdisplay {{vg1/lv1}}
```
{% endraw %}{% raw %}
<h2 id="lvextend">
  <a href="/en/linux/lvextend.html">lvextend</a> <a href="#lvextend"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Increase the size of a logical volume.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/lvextend.8.html>.

#### Increase a volume's size to 120GB:
```shell
lvextend --size {{120G}} {{logical_volume}}
```
#### Increase a volume's size by 40GB as well as the underlying filesystem:
```shell
lvextend --size +{{40G}} -r {{logical_volume}}
```
#### Increase a volume's size to 100% of the free physical volume space:
```shell
lvextend --size {{100}}%FREE {{logical_volume}}
```
{% endraw %}{% raw %}
<h2 id="lvm">
  <a href="/en/linux/lvm.html">lvm</a> <a href="#lvm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage physical volumes, volume groups, and logical volumes using the Logical Volume Manager (LVM) interactive shell.
> More information: <https://man7.org/linux/man-pages/man8/lvm.8.html>.

#### Start the Logical Volume Manager interactive shell:
```shell
sudo lvm
```
#### List the Logical Volume Manager commands:
```shell
sudo lvm help
```
#### Initialize a drive or partition to be used as a physical volume:
```shell
sudo lvm pvcreate {{/dev/sdXY}}
```
#### Display information about physical volumes:
```shell
sudo lvm pvdisplay
```
#### Create a volume group called vg1 from the physical volume on `/dev/sdXY`:
```shell
sudo lvm vgcreate {{vg1}} {{/dev/sdXY}}
```
#### Display information about volume groups:
```shell
sudo lvm vgdisplay
```
#### Create a logical volume with size 10G from volume group vg1:
```shell
sudo lvm lvcreate -L {{10G}} {{vg1}}
```
#### Display information about logical volumes:
```shell
sudo lvm lvdisplay
```
{% endraw %}{% raw %}
<h2 id="lvreduce">
  <a href="/en/linux/lvreduce.html">lvreduce</a> <a href="#lvreduce"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Reduce the size of a logical volume.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/lvreduce.8.html>.

#### Reduce a volume's size to 120GB:
```shell
lvreduce --size {{120G}} {{logical_volume}}
```
#### Reduce a volume's size by 40GB as well as the underlying filesystem:
```shell
lvreduce --size -{{40G}} -r {{logical_volume}}
```
{% endraw %}{% raw %}
<h2 id="lvremove">
  <a href="/en/linux/lvremove.html">lvremove</a> <a href="#lvremove"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remove one or more logical volumes.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/lvremove.8.html>.

#### Remove a logical volume in a volume group:
```shell
sudo lvremove {{volume_group}}/{{logical_volume}}
```
#### Remove all logical volumes in a volume group:
```shell
sudo lvremove {{volume_group}}
```
{% endraw %}{% raw %}
<h2 id="lvresize">
  <a href="/en/linux/lvresize.html">lvresize</a> <a href="#lvresize"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Change the size of a logical volume.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/lvresize.8.html>.

#### Change the size of a logical volume to 120GB:
```shell
lvresize --size {{120G}} {{volume_group}}/{{logical_volume}}
```
#### Extend the size of a logical volume as well as the underlying filesystem by 120GB:
```shell
lvresize --size +{{120G}} --resizefs {{volume_group}}/{{logical_volume}}
```
#### Extend the size of a logical volume to 100% of the free physical volume space:
```shell
lvresize --size {{100}}%FREE {{volume_group}}/{{logical_volume}}
```
#### Reduce the size of a logical volume as well as the underlying filesystem by 120GB:
```shell
lvresize --size -{{120G}} --resizefs {{volume_group}}/{{logical_volume}}
```
{% endraw %}{% raw %}
<h2 id="lvs">
  <a href="/en/linux/lvs.html">lvs</a> <a href="#lvs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display information about logical volumes.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/lvs.8.html>.

#### Display information about logical volumes:
```shell
lvs
```
#### Display all logical volumes:
```shell
lvs -a
```
#### Change default display to show more details:
```shell
lvs -v
```
#### Display only specific fields:
```shell
lvs -o {{field_name_1}},{{field_name_2}}
```
#### Append field to default display:
```shell
lvs -o +{{field_name}}
```
#### Suppress heading line:
```shell
lvs --noheadings
```
#### Use a separator to separate fields:
```shell
lvs --separator {{=}}
```
{% endraw %}{% raw %}
<h2 id="lxc">
  <a href="/en/linux/lxc.html">lxc</a> <a href="#lxc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage Linux containers using the lxd REST API.
> Any container names or patterns can be prefixed with the name of a remote server.

#### List local containers matching a string. Omit the string to list all local containers:
```shell
lxc list {{match_string}}
```
#### List images matching a string. Omit the string to list all images:
```shell
lxc image list [{{remote}}:]{{match_string}}
```
#### Create a new container from an image:
```shell
lxc init [{{remote}}:]{{image}} {{container}}
```
#### Start a container:
```shell
lxc start [{{remote}}:]{{container}}
```
#### Stop a container:
```shell
lxc stop [{{remote}}:]{{container}}
```
#### Show detailed info about a container:
```shell
lxc info [{{remote}}:]{{container}}
```
#### Take a snapshot of a container:
```shell
lxc snapshot [{{remote}}:]{{container}} {{snapshot}}
```
{% endraw %}{% raw %}
<h2 id="lxterminal">
  <a href="/en/linux/lxterminal.html">lxterminal</a> <a href="#lxterminal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Terminal emulator for LXDE.
> More information: <https://wiki.lxde.org/en/LXTerminal>.

#### Open an LXTerminal window:
```shell
lxterminal
```
#### Open an LXTerminal window, run a command, and then exit:
```shell
lxterminal -e "{{command}}"
```
#### Open an LXTerminal window with multiple tabs:
```shell
lxterminal --tabs={{tab_name1,tab_name2,...}}
```
#### Open an LXTerminal window with a specific title:
```shell
lxterminal --title={{title_name}}
```
#### Open an LXTerminal window with a specific working directory:
```shell
lxterminal --working-directory={{path/to/directory}}
```
{% endraw %}{% raw %}
<h2 id="lynis">
  <a href="/en/linux/lynis.html">lynis</a> <a href="#lynis"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> System and security auditing tool.
> More information: <https://cisofy.com/documentation/lynis/>.

#### Check that Lynis is up-to-date:
```shell
sudo lynis update info
```
#### Run a security audit of the system:
```shell
sudo lynis audit system
```
#### Run a security audit of a Dockerfile:
```shell
sudo lynis audit dockerfile {{path/to/dockerfile}}
```
{% endraw %}{% raw %}
<h2 id="mac2unix">
  <a href="/en/linux/mac2unix.html">mac2unix</a> <a href="#mac2unix"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Change macOS-style line endings to Unix-style.
> Replaces LF with CR.

#### Change the line endings of a file:
```shell
mac2unix {{filename}}
```
#### Create a copy with Unix-style line endings:
```shell
mac2unix -n {{filename}} {{new_filename}}
```
{% endraw %}{% raw %}
<h2 id="macchanger">
  <a href="/en/linux/macchanger.html">macchanger</a> <a href="#macchanger"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line utility for manipulating network interface MAC addresses.

#### View the current and permanent MAC addresses of a interface:
```shell
macchanger --show {{interface}}
```
#### Set interface to a random MAC:
```shell
macchanger --random {{interface}}
```
#### Set interface to a specific MAC:
```shell
macchanger --mac {{XX:XX:XX:XX:XX:XX}} {{interface}}
```
#### Reset interface to its permanent hardware MAC:
```shell
macchanger --permanent {{interface}}
```
{% endraw %}{% raw %}
<h2 id="maim">
  <a href="/en/linux/maim.html">maim</a> <a href="#maim"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Screenshot utility.
> More information: <https://github.com/naelstrof/maim>.

#### Capture a screenshot and save it to the given path:
```shell
maim {{path/to/screenshot.png}}
```
#### Capture a screenshot of the selected region:
```shell
maim --select {{path/to/screenshot.png}}
```
#### Capture a screenshot of the selected region and save it in the clipboard (requires `xclip`):
```shell
maim --select | xclip -selection clipboard -target image/png
```
#### Capture a screenshot of the current active window (requires `xdotool`):
```shell
maim --window $(xdotool getactivewindow) {{path/to/screenshot.png}}
```
{% endraw %}{% raw %}
<h2 id="makepkg">
  <a href="/en/linux/makepkg.html">makepkg</a> <a href="#makepkg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Creates a package installable with the `pacman` package manager.
> Runs the commands from a `PKGBUILD` file to build the package.
> More information: <https://wiki.archlinux.org/index.php/Makepkg>.

#### Make a package (run in the same directory as a `PKGBUILD`):
```shell
makepkg
```
#### Make a package and install its dependencies:
```shell
makepkg --syncdeps
```
#### Same as above, but install the package with `pacman` when done:
```shell
makepkg --syncdeps --install
```
#### Make a package, but skip source checksums:
```shell
makepkg --skipchecksums
```
{% endraw %}{% raw %}
<h2 id="mandb">
  <a href="/en/linux/mandb.html">mandb</a> <a href="#mandb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage the pre-formatted manual page database.
> More information: <https://man7.org/linux/man-pages/man8/mandb.8.html>.

#### Purge and process manual pages:
```shell
mandb
```
#### Update a single entry:
```shell
mandb --filename {{path/to/file}}
```
#### Create entries from scratch instead of updating:
```shell
mandb --create
```
#### Only process user databases:
```shell
mandb --user-db
```
#### Do not purge obsolete entries:
```shell
mandb --no-purge
```
#### Check the validity of manual pages:
```shell
mandb --test
```
{% endraw %}{% raw %}
<h2 id="manpath">
  <a href="/en/linux/manpath.html">manpath</a> <a href="#manpath"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Determine the search path for manual pages.

#### Display the search path used to find man pages:
```shell
manpath
```
#### Show the entire global manpath:
```shell
manpath --global
```
{% endraw %}{% raw %}
<h2 id="mcookie">
  <a href="/en/linux/mcookie.html">mcookie</a> <a href="#mcookie"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generates random 128 bit hexadecimal numbers.

#### Generate a random number:
```shell
mcookie
```
#### Generate a random number, using the contents of a file as a seed for the randomness:
```shell
mcookie --file {{path/to/file}}
```
#### Generate a random number, using a specific number of bytes from a file as a seed for the randomness:
```shell
mcookie --file {{path/to/file}} --max-size {{number_of_bytes}}
```
#### Print the details of the randomness used, such as the origin and seed for each source:
```shell
mcookie --verbose
```
{% endraw %}{% raw %}
<h2 id="mdadm">
  <a href="/en/linux/mdadm.html">mdadm</a> <a href="#mdadm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> RAID management utility.
> More information: <https://manned.org/mdadm>.

#### Create array:
```shell
mdadm --create {{/dev/md/MyRAID}} --level {{raid_level}} --raid-devices {{number_of_disks}} {{/dev/sdXN}}
```
#### Stop array:
```shell
mdadm --stop {{/dev/md0}}
```
#### Mark disk as failed:
```shell
mdadm --fail {{/dev/md0}} {{/dev/sdXN}}
```
#### Remove disk:
```shell
mdadm --remove {{/dev/md0}} {{/dev/sdXN}}
```
#### Add disk to array:
```shell
mdadm --assemble {{/dev/md0}} {{/dev/sdXN}}
```
#### Show RAID info:
```shell
mdadm --detail {{/dev/md0}}
```
{% endraw %}{% raw %}
<h2 id="mdbook">
  <a href="/en/linux/mdbook.html">mdbook</a> <a href="#mdbook"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create online books by writing makrdown files.
> More information: <https://rust-lang.github.io/mdBook/>.

#### Create a mdbook project in the current directory:
```shell
mdbook init
```
#### Create a mdbook project in a specific directory:
```shell
mdbook init {{path/to/directory}}
```
#### Clean the directory with the generated book:
```shell
mdbook clean
```
#### Serve a book at `http://localhost:3000`, auto build when file changes:
```shell
mdbook serve
```
#### Watch a set of Markdown files and automatically build when a file is changed:
```shell
mdbook watch
```
{% endraw %}{% raw %}
<h2 id="medusa">
  <a href="/en/linux/medusa.html">Medusa</a> <a href="#medusa"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A modular and parallel login brute-forcer for a variety of protocols.

#### Execute brute force against an FTP server using a file containing usernames and a file containing passwords:
```shell
medusa -M ftp -h host -U {{path/to/username_file}} -P {{path/to/password_file}}
```
#### Execute a login attempt against a HTTP server using the username, password and user-agent specified:
```shell
medusa -M HTTP -h host -u {{username}} -p {{password}} -m USER-AGENT:"{{Agent}}"
```
#### Execute a brute force against a MySQL server using a file containing usernames and a hash:
```shell
medusa -M mysql -h host -U {{path/to/username_file}} -p {{hash}} -m PASS:HASH
```
#### Execute a brute force against a list of SMB servers using a username and a pwdump file:
```shell
medusa -M smbnt -H {{path/to/hosts_file}} -C {{path/to/pwdump_file}} -u {{username}} -m PASS:HASH
```
{% endraw %}{% raw %}
<h2 id="microcom">
  <a href="/en/linux/microcom.html">microcom</a> <a href="#microcom"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A minimalistic terminal program, used to access remote devices via a serial, CAN or telnet connection from the console.

#### Open a serial port using the specified baud rate:
```shell
microcom --port {{path/to/serial_port}} --speed {{baud_rate}}
```
#### Establish a telnet connection to the specified host:
```shell
microcom --telnet {{hostname}}:{{port}}
```
{% endraw %}{% raw %}
<h2 id="mimetype">
  <a href="/en/linux/mimetype.html">mimetype</a> <a href="#mimetype"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Automatically determine the MIME type of a file.

#### Print the MIME type of a given file:
```shell
mimetype {{path/to/file}}
```
#### Display only the MIME type, and not the filename:
```shell
mimetype --brief {{path/to/file}}
```
#### Display a description of the MIME type:
```shell
mimetype --describe {{path/to/file}}
```
#### Determine the MIME type of stdin (does not check a filename):
```shell
{{some_command}} | mimetype --stdin
```
#### Display debug information about how the MIME type was determined:
```shell
mimetype --debug {{path/to/file}}
```
#### Display all the possible MIME types of a given file in confidence order:
```shell
mimetype --all {{path/to/file}}
```
#### Explicitly specify the 2-letter language code of the output:
```shell
mimetype --language {{path/to/file}}
```
{% endraw %}{% raw %}
<h2 id="mke2fs">
  <a href="/en/linux/mke2fs.html">mke2fs</a> <a href="#mke2fs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Creates a Linux filesystem inside a partition.

#### Create an ext2 filesystem in partition 1 of device b (`sdb1`):
```shell
mkfs.ext2 {{/dev/sdb1}}
```
#### Create an ext3 filesystem in partition 1 of device b (`sdb1`):
```shell
mkfs.ext3 {{/dev/sdb1}}
```
#### Create an ext4 filesystem in partition 1 of device b (`sdb1`):
```shell
mkfs.ext4 {{/dev/sdb1}}
```
{% endraw %}{% raw %}
<h2 id="mkfs.btrfs">
  <a href="/en/linux/mkfs.btrfs.html">mkfs.btrfs</a> <a href="#mkfs.btrfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create a btrfs filesystem.
> Defaults to `raid1`, which specifies 2 copies of a given data block spread across 2 different devices.
> More information: <https://btrfs.wiki.kernel.org/index.php/Manpage/mkfs.btrfs>.

#### Create a btrfs filesystem on a single device:
```shell
sudo mkfs.btrfs --metadata single --data single {{/dev/sda}}
```
#### Create a btrfs filesystem on multiple devices with raid1:
```shell
sudo mkfs.btrfs --metadata raid1 --data raid1 {{/dev/sda}} {{/dev/sdb}} {{/dev/sdN}}
```
#### Set a label for the filesystem:
```shell
sudo mkfs.btrfs --label "{{label}}" {{/dev/sda}} [{{/dev/sdN}}]
```
{% endraw %}{% raw %}
<h2 id="mkfs.cramfs">
  <a href="/en/linux/mkfs.cramfs.html">mkfs.cramfs</a> <a href="#mkfs.cramfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Creates a ROM filesystem inside a partition.

#### Create a ROM filesystem inside partition 1 on device b (`sdb1`):
```shell
mkfs.cramfs {{/dev/sdb1}}
```
#### Create a ROM filesystem with a volume-name:
```shell
mkfs.cramfs -n {{volume_name}} {{/dev/sdb1}}
```
{% endraw %}{% raw %}
<h2 id="mkfs.exfat">
  <a href="/en/linux/mkfs.exfat.html">mkfs.exfat</a> <a href="#mkfs.exfat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Creates an exfat filesystem inside a partition.

#### Create an exfat filesystem inside partition 1 on device b (`sdb1`):
```shell
mkfs.exfat {{/dev/sdb1}}
```
#### Create filesystem with a volume-name:
```shell
mkfs.exfat -n {{volume_name}} {{/dev/sdb1}}
```
#### Create filesystem with a volume-id:
```shell
mkfs.exfat -i {{volume_id}} {{/dev/sdb1}}
```
{% endraw %}{% raw %}
<h2 id="mkfs.ext4">
  <a href="/en/linux/mkfs.ext4.html">mkfs.ext4</a> <a href="#mkfs.ext4"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Creates an ext4 filesystem inside a partition.

#### Create an ext4 filesystem inside partition 1 on device b (`sdb1`):
```shell
sudo mkfs.ext4 {{/dev/sdb1}}
```
#### Create an ext4 filesystem with a volume-label:
```shell
sudo mkfs.ext4 -L {{volume_label}} {{/dev/sdb1}}
```
{% endraw %}{% raw %}
<h2 id="mkfs.fat">
  <a href="/en/linux/mkfs.fat.html">mkfs.fat</a> <a href="#mkfs.fat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Creates an MS-DOS filesystem inside a partition.

#### Create a fat filesystem inside partition 1 on device b (`sdb1`):
```shell
mkfs.fat {{/dev/sdb1}}
```
#### Create filesystem with a volume-name:
```shell
mkfs.fat -n {{volume_name}} {{/dev/sdb1}}
```
#### Create filesystem with a volume-id:
```shell
mkfs.fat -i {{volume_id}} {{/dev/sdb1}}
```
#### Use 5 instead of 2 file allocation tables:
```shell
mkfs.fat -f 5 {{/dev/sdb1}}
```
{% endraw %}{% raw %}
<h2 id="mkfs">
  <a href="/en/linux/mkfs.html">mkfs</a> <a href="#mkfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Build a Linux filesystem on a hard disk partition.
> This command is deprecated in favor of filesystem specific mkfs.<type> utils.

#### Build a Linux ext2 filesystem on a partition:
```shell
mkfs {{path/to/partition}}
```
#### Build a filesystem of a specified type:
```shell
mkfs -t {{ext4}} {{path/to/partition}}
```
#### Build a filesystem of a specified type and check for bad blocks:
```shell
mkfs -c -t {{ntfs}} {{path/to/partition}}
```
{% endraw %}{% raw %}
<h2 id="mkfs.minix">
  <a href="/en/linux/mkfs.minix.html">mkfs.minix</a> <a href="#mkfs.minix"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Creates a Minix filesystem inside a partition.

#### Create a Minix filesystem inside partition 1 on device b (`sdb1`):
```shell
mkfs.minix {{/dev/sdb1}}
```
{% endraw %}{% raw %}
<h2 id="mkfs.ntfs">
  <a href="/en/linux/mkfs.ntfs.html">mkfs.ntfs</a> <a href="#mkfs.ntfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Creates a NTFS filesystem inside a partition.

#### Create a NTFS filesystem inside partition 1 on device b (`sdb1`):
```shell
mkfs.ntfs {{/dev/sdb1}}
```
#### Create filesystem with a volume-label:
```shell
mkfs.ntfs -L {{volume_label}} {{/dev/sdb1}}
```
#### Create filesystem with specific UUID:
```shell
mkfs.ntfs -U {{UUID}} {{/dev/sdb1}}
```
{% endraw %}{% raw %}
<h2 id="mkfs.vfat">
  <a href="/en/linux/mkfs.vfat.html">mkfs.vfat</a> <a href="#mkfs.vfat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Creates an MS-DOS filesystem inside a partition.

#### Create a vfat filesystem inside partition 1 on device b (`sdb1`):
```shell
mkfs.vfat {{/dev/sdb1}}
```
#### Create filesystem with a volume-name:
```shell
mkfs.vfat -n {{volume_name}} {{/dev/sdb1}}
```
#### Create filesystem with a volume-id:
```shell
mkfs.vfat -i {{volume_id}} {{/dev/sdb1}}
```
#### Use 5 instead of 2 file allocation tables:
```shell
mkfs.vfat -f 5 {{/dev/sdb1}}
```
{% endraw %}{% raw %}
<h2 id="mkinitcpio">
  <a href="/en/linux/mkinitcpio.html">mkinitcpio</a> <a href="#mkinitcpio"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generates initial ramdisk environments for booting the Linux kernel based on the specified preset(s).
> More information: <https://man.archlinux.org/man/mkinitcpio.8>.

#### Perform a dry run (print what would be done without actually doing it):
```shell
mkinitcpio
```
#### Generate a ramdisk environment based on the `linux` preset:
```shell
mkinitcpio --preset {{linux}}
```
#### Generate a ramdisk environment based on the `linux-lts` preset:
```shell
mkinitcpio --preset {{linux-lts}}
```
#### Generate ramdisk environments based on all existing presets (used to regenerate all the initramfs images after a change in `/etc/mkinitcpio.conf`):
```shell
mkinitcpio --allpresets
```
#### Generate an initramfs image using an alternative configuration file:
```shell
mkinitcpio --config {{path/to/mkinitcpio.conf}} --generate {{path/to/initramfs.img}}
```
#### Generate an initramfs image for a kernel other than the one currently running (the installed kernel releases can be found in `/usr/lib/modules/`):
```shell
mkinitcpio --kernel {{kernel_version}} --generate {{path/to/initramfs.img}}
```
#### List all available hooks:
```shell
mkinitcpio --listhooks
```
#### Display help for a specific hook:
```shell
mkinitcpio --hookhelp {{hook_name}}
```
{% endraw %}{% raw %}
<h2 id="mkisofs">
  <a href="/en/linux/mkisofs.html">mkisofs</a> <a href="#mkisofs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create ISO files from directories.
> Also aliased as `genisoimage`.

#### Create an ISO from a directory:
```shell
mkisofs -o {{filename.iso}} {{path/to/source_directory}}
```
#### Set the disc label when creating an ISO:
```shell
mkisofs -o {{filename.iso}} -V "{{label_name}}" {{path/to/source_directory}}
```
{% endraw %}{% raw %}
<h2 id="mklost+found">
  <a href="/en/linux/mklost+found.html">mklost+found</a> <a href="#mklost+found"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create a lost+found directory.
> More information: <https://manned.org/mklost+found>.

#### Create a `lost+found` directory in the current directory:
```shell
mklost+found
```
{% endraw %}{% raw %}
<h2 id="mknod">
  <a href="/en/linux/mknod.html">mknod</a> <a href="#mknod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create block or character device special files.
> More information: <https://www.gnu.org/software/coreutils/mknod>.

#### Create a block device:
```shell
sudo mknod {{path/to/device_file}} b {{major_device_number}} {{minor_device_number}}
```
#### Create a character device:
```shell
sudo mknod {{path/to/device_file}} c {{major_device_number}} {{minor_device_number}}
```
#### Create a FIFO (queue) device:
```shell
sudo mknod {{path/to/device_file}} p
```
#### Create a device file with default SELinux security context:
```shell
sudo mknod -Z {{path/to/device_file}} {{type}} {{major_device_number}} {{minor_device_number}}
```
{% endraw %}{% raw %}
<h2 id="mkswap">
  <a href="/en/linux/mkswap.html">mkswap</a> <a href="#mkswap"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sets up a Linux swap area on a device or in a file.

#### Setup a given partition as swap area:
```shell
sudo mkswap {{/dev/sdb7}}
```
#### Use a given file as swap area:
```shell
sudo mkswap {{path/to/file}}
```
#### Check a partition for bad blocks before creating the swap area:
```shell
sudo mkswap -c {{/dev/sdb7}}
```
#### Specify a label for the file (to allow `swapon` to use the label):
```shell
sudo mkswap -L {{swap1}} {{path/to/file}}
```
{% endraw %}{% raw %}
<h2 id="mmcli">
  <a href="/en/linux/mmcli.html">mmcli</a> <a href="#mmcli"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Control and monitor the ModemManager.
> More information: <https://www.freedesktop.org/software/ModemManager/man/latest/mmcli.1.html>.

#### List SMS messages available on the modem:
```shell
sudo mmcli --modem={{modem}} --messaging-list-sms
```
#### Delete a message from the modem, specifying its path:
```shell
sudo mmcli --modem={{modem}} --messaging-delete-sms={{path/to/message_file}}
```
{% endraw %}{% raw %}
<h2 id="mocp">
  <a href="/en/linux/mocp.html">mocp</a> <a href="#mocp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Music on Console (MOC) audio player.
> More information: <https://manned.org/mocp>.

#### Launch the MOC terminal UI:
```shell
mocp
```
#### Launch the MOC terminal UI in a specific directory:
```shell
mocp {{path/to/directory}}
```
#### Start the MOC server in the background, without launching the MOC terminal UI:
```shell
mocp --server
```
#### Add a specific song to the play queue while MOC is in the background:
```shell
mocp --enqueue {{path/to/audio_file}}
```
#### Add songs recursively to the play queue while MOC is in the background:
```shell
mocp --append {{path/to/directory}}
```
#### Clear the play queue while MOC is in the background:
```shell
mocp --clear
```
#### Play or stop the currently queued song while MOC is in the background:
```shell
mocp --{{play|stop}}
```
#### Stop the MOC server while it's in the background:
```shell
mocp --exit
```
{% endraw %}{% raw %}
<h2 id="modinfo">
  <a href="/en/linux/modinfo.html">modinfo</a> <a href="#modinfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Extract information about a Linux kernel module.

#### List all attributes of a kernel module:
```shell
modinfo {{kernel_module}}
```
#### List the specified attribute only:
```shell
modinfo -F {{author|description|license|parm|filename}} {{kernel_module}}
```
{% endraw %}{% raw %}
<h2 id="modprobe">
  <a href="/en/linux/modprobe.html">modprobe</a> <a href="#modprobe"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Add or remove modules from the Linux kernel.

#### Pretend to load a module into the kernel, but don't actually do it:
```shell
sudo modprobe --dry-run {{module_name}}
```
#### Load a module into the kernel:
```shell
sudo modprobe {{module_name}}
```
#### Remove a module from the kernel:
```shell
sudo modprobe --remove {{module_name}}
```
#### Remove a module and those that depend on it from the kernel:
```shell
sudo modprobe --remove-dependencies {{module_name}}
```
#### Show a kernel module's dependencies:
```shell
sudo modprobe --show-depends {{module_name}}
```
{% endraw %}{% raw %}
<h2 id="module">
  <a href="/en/linux/module.html">module</a> <a href="#module"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Modify a users' environment using the module command.
> More information: <https://lmod.readthedocs.io/en/latest/010_user.html>.

#### Display available modules:
```shell
module avail
```
#### Search for a module by name:
```shell
module spider {{module_name}}
```
#### Load a module:
```shell
module load {{module_name}}
```
#### Display loaded modules:
```shell
module list
```
#### Unload a specific loaded module:
```shell
module {{module_name}}
```
#### Unload all loaded modules:
```shell
module purge
```
{% endraw %}{% raw %}
<h2 id="mono">
  <a href="/en/linux/mono.html">mono</a> <a href="#mono"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Runtime for the .NET Framework.
> More information: <https://www.mono-project.com/docs/>.

#### Run a .NET assembly in debug mode:
```shell
mono --debug {{path/to/program.exe}}
```
#### Run a .NET assembly:
```shell
mono {{path/to/program.exe}}
```
{% endraw %}{% raw %}
<h2 id="mons">
  <a href="/en/linux/mons.html">mons</a> <a href="#mons"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool to quickly manage two displays.
> More information: <https://github.com/Ventto/mons>.

#### Enable only the primary monitor:
```shell
mons -o
```
#### Enable only the secondary monitor:
```shell
mons -s
```
#### Duplicate the primary monitor onto the secondary monitor, using the resolution of the primary monitor:
```shell
mons -d
```
#### Mirror the primary monitor onto the secondary monitor, using the resolution of the secondary monitor:
```shell
mons -m
```
{% endraw %}{% raw %}
<h2 id="mountpoint">
  <a href="/en/linux/mountpoint.html">mountpoint</a> <a href="#mountpoint"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Test if a directory is a filesystem mountpoint.

#### Check if a directory is a mountpoint:
```shell
mountpoint {{path/to/directory}}
```
#### Check if a directory is a mountpoint without showing any output:
```shell
mountpoint -q {{path/to/directory}}
```
#### Show major/minor numbers of a mountpoint's filesystem:
```shell
mountpoint --fs-devno {{path/to/directory}}
```
{% endraw %}{% raw %}
<h2 id="mpstat">
  <a href="/en/linux/mpstat.html">mpstat</a> <a href="#mpstat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Report CPU statistics.

#### Display CPU statistics every 2 seconds:
```shell
mpstat {{2}}
```
#### Display 5 reports, one by one, at 2 second intervals:
```shell
mpstat {{2}} {{5}}
```
#### Display 5 reports, one by one, from a given processor, at 2 second intervals:
```shell
mpstat -P {{0}} {{2}} {{5}}
```
{% endraw %}{% raw %}
<h2 id="mssh">
  <a href="/en/linux/mssh.html">mssh</a> <a href="#mssh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> GTK+ based SSH client for interacting with multiple SSH servers at once.

#### Open a new window and connect to multiple SSH servers:
```shell
mssh {{user@host1}} {{user@host2}} {{...}}
```
#### Open a new window and connect to a group of servers predefined in `~/.mssh_clusters`:
```shell
mssh --alias {{alias_name}}
```
{% endraw %}{% raw %}
<h2 id="mullvad">
  <a href="/en/linux/mullvad.html">mullvad</a> <a href="#mullvad"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI client for Mullvad VPN.
> More information: <https://mullvad.net/>.

#### Link your mullvad account with the specified account number:
```shell
mullvad account set {{account_number}}
```
#### Enable LAN access while VPN is on:
```shell
mullvad lan set allow
```
#### Establish the VPN tunnel:
```shell
mullvad connect
```
#### Check status of VPN tunnel:
```shell
mullvad status
```
{% endraw %}{% raw %}
<h2 id="mycli">
  <a href="/en/linux/mycli.html">mycli</a> <a href="#mycli"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A CLI for MySQL, MariaDB, and Percona with auto-completion and syntax highlighting.

#### Connect to a database with the currently logged in user:
```shell
mycli {{database_name}}
```
#### Connect to a database with the specified user:
```shell
mycli -u {{user}} {{database_name}}
```
#### Connect to a database on the specified host with the specified user:
```shell
mycli -u {{user}} -h {{host}} {{database_name}}
```
{% endraw %}{% raw %}
<h2 id="n">
  <a href="/en/linux/n.html">n</a> <a href="#n"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool to manage multiple node versions.

#### Install a given version of node. If the version is already installed, it will be activated:
```shell
n {{version}}
```
#### Display installed versions and interactively activate one of them:
```shell
n
```
#### Remove a version:
```shell
n rm {{version}}
```
#### Execute a file with a given version:
```shell
n use {{version}} {{file.js}}
```
#### Output binary path for a version:
```shell
n bin {{version}}
```
{% endraw %}{% raw %}
<h2 id="named">
  <a href="/en/linux/named.html">named</a> <a href="#named"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Execute the DNS (Dynamic Name Service) server daemon that converts host names to IP addresses and vice versa.
> More information: <https://manned.org/named>.

#### Read the default configuration file `/etc/named.conf`, read any initial data and listen for queries:
```shell
named
```
#### Read a custom configuration file:
```shell
named -c {{path/to/named.conf}}
```
#### Use IPv4 or IPv6 only, even if the host machine is capable of utilising other protocols:
```shell
named {{-4|-6}}
```
#### Listen for queries on a specific port instead of the default port 53:
```shell
named -p {{port}}
```
#### Run the server in the foreground and do not daemonize:
```shell
named -f
```
{% endraw %}{% raw %}
<h2 id="namei">
  <a href="/en/linux/namei.html">namei</a> <a href="#namei"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Follows a pathname (which can be a symbolic link) until a terminal point is found (a file/directory/char device etc).
> This program is useful for finding "too many levels of symbolic links" problems.

#### Resolve the pathnames specified as the argument parameters:
```shell
namei {{path/to/a}} {{path/to/b}} {{path/to/c}}
```
#### Display the results in a long-listing format:
```shell
namei --long {{path/to/a}} {{path/to/b}} {{path/to/c}}
```
#### Show the mode bits of each file type in the style of `ls`:
```shell
namei --modes {{path/to/a}} {{path/to/b}} {{path/to/c}}
```
#### Show owner and group name of each file:
```shell
namei --owners {{path/to/a}} {{path/to/b}} {{path/to/c}}
```
#### Don't follow symlinks while resolving:
```shell
namei --nosymlinks {{path/to/a}} {{path/to/b}} {{path/to/c}}
```
{% endraw %}{% raw %}
<h2 id="nautilus">
  <a href="/en/linux/nautilus.html">nautilus</a> <a href="#nautilus"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Default file explorer for GNOME desktop environment.
> Also known as GNOME Files.
> More information: <https://manned.org/nautilus>.

#### Launch Nautilus:
```shell
nautilus
```
#### Launch Nautilus as root user:
```shell
sudo nautilus
```
#### Launch Nautilus and display a specific directory:
```shell
nautilus {{path/to/directory}}
```
#### Launch Nautilus with a specific file or directory selected:
```shell
nautilus --select {{path/to/file_or_directory}}
```
#### Launch Nautilus in a separated window:
```shell
nautilus --new-window
```
#### Close all Nautilus instances:
```shell
nautilus --quit
```
#### Display help:
```shell
nautilus --help
```
{% endraw %}{% raw %}
<h2 id="ncat">
  <a href="/en/linux/ncat.html">ncat</a> <a href="#ncat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Use the normal `cat` functionality over networks.

#### Listen for input on the specified port and write it to the specified file:
```shell
ncat -l {{port}} > {{path/to/file}}
```
#### Accept multiple connections and keep ncat open after they have been closed:
```shell
ncat -lk {{port}}
```
#### Write output of specified file to the specified host on the specified port:
```shell
ncat {{address}} {{port}} < {{path/to/file}}
```
{% endraw %}{% raw %}
<h2 id="ncdu">
  <a href="/en/linux/ncdu.html">ncdu</a> <a href="#ncdu"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Disk usage analyzer with an ncurses interface.

#### Analyze the current working directory:
```shell
ncdu
```
#### Analyze a given directory:
```shell
ncdu {{path/to/directory}}
```
#### Save results to a file:
```shell
ncdu -o {{path/to/file}}
```
#### Exclude files that match a pattern, argument can be given multiple times to add more patterns:
```shell
ncdu --exclude '{{*.txt}}'
```
{% endraw %}{% raw %}
<h2 id="ndctl">
  <a href="/en/linux/ndctl.html">ndctl</a> <a href="#ndctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility for managing Non-Volatile DIMMs.

#### Create an 'fsdax' mode namespace:
```shell
ndctl create-namespace --mode={{fsdax}}
```
#### Change the mode of a namespace to 'raw':
```shell
ndctl create-namespace --reconfigure={{namespaceX.Y}} --mode={{raw}}
```
#### Check a sector mode namespace for consistency, and repair if needed:
```shell
ndctl check-namespace --repair {{namespaceX.Y}}
```
#### List all namespaces, regions, and buses (including disabled ones):
```shell
ndctl list --namespaces --regions --buses --idle
```
#### List a specific namespace and include lots of additional information:
```shell
ndctl list -vvv --namespace={{namespaceX.Y}}
```
#### Run a monitor to watch for SMART health events for NVDIMMs on the 'ACPI.NFIT' bus:
```shell
ndctl monitor --bus={{ACPI.NFIT}}
```
#### Remove a namespace (when applicable) or reset it to an initial state:
```shell
ndctl destroy-namespace --force {{namespaceX.Y}}
```
{% endraw %}{% raw %}
<h2 id="nemo">
  <a href="/en/linux/nemo.html">nemo</a> <a href="#nemo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> File manager and graphical shell for Cinnamon.
> More information: <https://github.com/linuxmint/nemo>.

#### Open a new window showing the user's home directory:
```shell
nemo
```
#### Open a new window showing the current directory:
```shell
nemo .
```
#### Close all open nemo windows:
```shell
nemo --quit
```
{% endraw %}{% raw %}
<h2 id="nethogs">
  <a href="/en/linux/nethogs.html">nethogs</a> <a href="#nethogs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Monitor bandwidth usage per process.
> More information: <https://github.com/raboof/nethogs>.

#### Start nethogs as root (default device is eth0):
```shell
sudo nethogs
```
#### Monitor bandwidth on specific device:
```shell
sudo nethogs {{device}}
```
#### Monitor bandwidth on multiple devices:
```shell
sudo nethogs {{device1}} {{device2}}
```
#### Specify refresh rate:
```shell
sudo nethogs -t {{seconds}}
```
{% endraw %}{% raw %}
<h2 id="netselect-apt">
  <a href="/en/linux/netselect-apt.html">netselect-apt</a> <a href="#netselect-apt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create a `sources.list` file for a Debian mirror with the lowest latency.
> More information: <https://manpages.debian.org/buster/netselect-apt/netselect-apt.1.html>.

#### Create `sources.list` using the lowest latency server:
```shell
sudo netselect-apt
```
#### Specify Debian branch, stable is used by default:
```shell
sudo netselect-apt {{testing}}
```
#### Include non-free section:
```shell
sudo netselect-apt --non-free
```
#### Specify a country for the mirror list lookup:
```shell
sudo netselect-apt -c {{India}}
```
{% endraw %}{% raw %}
<h2 id="netselect">
  <a href="/en/linux/netselect.html">netselect</a> <a href="#netselect"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Speed test for choosing a fast network server.
> More information: <https://github.com/apenwarr/netselect>.

#### Choose the server with the lowest latency:
```shell
sudo netselect {{host_1}} {{host_2}}
```
#### Display nameserver resolution and statistics:
```shell
sudo netselect -vv {{host_1}} {{host_2}}
```
#### Define maximum TTL (time to live):
```shell
sudo netselect -m {{10}} {{host_1}} {{host_2}}
```
#### Print fastest N servers among the hosts:
```shell
sudo netselect -s {{N}} {{host_1}} {{host_2}} {{host_3}}
```
#### List available options:
```shell
netselect
```
{% endraw %}{% raw %}
<h2 id="netstat">
  <a href="/en/linux/netstat.html">netstat</a> <a href="#netstat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Displays network-related information such as open connections, open socket ports, etc.
> More information: <https://man7.org/linux/man-pages/man8/netstat.8.html>.

#### List all ports:
```shell
netstat --all
```
#### List all listening ports:
```shell
netstat --listening
```
#### List listening TCP ports:
```shell
netstat --tcp
```
#### Display PID and program names:
```shell
netstat --program
```
#### List information continuously:
```shell
netstat --continuous
```
#### List routes and do not resolve IP addresses to hostnames:
```shell
netstat --route --numeric
```
#### List listening TCP and UDP ports (+ user and process if you're root):
```shell
netstat --listening --program --numeric --tcp --udp --extend
```
{% endraw %}{% raw %}
<h2 id="newgrp">
  <a href="/en/linux/newgrp.html">newgrp</a> <a href="#newgrp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Switch primary group membership.

#### Change user's primary group membership:
```shell
newgrp {{group_name}}
```
#### Reset primary group membership to user's default group in `/etc/passwd`:
```shell
newgrp
```
{% endraw %}{% raw %}
<h2 id="nft">
  <a href="/en/linux/nft.html">nft</a> <a href="#nft"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Allows configuration of tables, chains and rules provided by the Linux kernel firewall.
> Nftables replaces iptables.

#### View current configuration:
```shell
sudo nft list ruleset
```
#### Add a new table with family "inet" and table "filter":
```shell
sudo nft add table {{inet}} {{filter}}
```
#### Add a new chain to accept all inbound traffic:
```shell
sudo nft add chain {{inet}} {{filter}} {{input}} \{ type {{filter}} hook {{input}} priority {{0}} \; policy {{accept}} \}
```
#### Add a new rule to accept several TCP ports:
```shell
sudo nft add rule {{inet}} {{filter}} {{input}} {{tcp}} {{dport \{ telnet, ssh, http, https \} accept}}
```
#### Show rule handles:
```shell
sudo nft --handle --numeric list chain {{family}} {{table}} {{chain}}
```
#### Delete a rule:
```shell
sudo nft delete rule {{inet}} {{filter}} {{input}} handle {{3}}
```
#### Save current configuration:
```shell
sudo nft list ruleset > {{/etc/nftables.conf}}
```
{% endraw %}{% raw %}
<h2 id="nixos-rebuild">
  <a href="/en/linux/nixos-rebuild.html">nixos-rebuild</a> <a href="#nixos-rebuild"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Reconfigure a NixOS machine.
> More information: <https://nixos.org/nixos/manual/#sec-changing-config>.

#### Build and switch to the new configuration, making it the boot default:
```shell
sudo nixos-rebuild switch
```
#### Build and switch to the new configuration, making it the boot default and naming the boot entry:
```shell
sudo nixos-rebuild switch -p {{name}}
```
#### Build and switch to the new configuration, making it the boot default and installing updates:
```shell
sudo nixos-rebuild switch --upgrade
```
#### Rollback changes to the configuration, switching to the previous generation:
```shell
sudo nixos-rebuild switch --rollback
```
#### Build the new configuration and make it the boot default without switching to it:
```shell
sudo nixos-rebuild boot
```
#### Build and activate the new configuration, but don't make a boot entry (for testing purposes):
```shell
sudo nixos-rebuild test
```
#### Build the configuration and open it in a virtual machine:
```shell
sudo nixos-rebuild build-vm
```
{% endraw %}{% raw %}
<h2 id="nm">
  <a href="/en/linux/nm.html">nm</a> <a href="#nm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List symbol names in object files.

#### List global (extern) functions in a file (prefixed with T):
```shell
nm -g {{file.o}}
```
#### List only undefined symbols in a file:
```shell
nm -u {{file.o}}
```
#### List all symbols, even debugging symbols:
```shell
nm -a {{file.o}}
```
#### Demangle C++ symbols (make them readable):
```shell
nm --demangle {{file.o}}
```
{% endraw %}{% raw %}
<h2 id="nmcli-connection">
  <a href="/en/linux/nmcli-connection.html">nmcli connection</a> <a href="#nmcli-connection"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Connection management with NetworkManager.
> More information: <https://man.archlinux.org/man/nmcli.1>.

#### List all NetworkManager connections (shows name, uuid, type and device):
```shell
nmcli connection
```
#### Activate a connection by specifying an uuid:
```shell
nmcli connection up uuid {{uuid}}
```
#### Deactivate a connection:
```shell
nmcli connection down uuid {{uuid}}
```
#### Create an auto-configured dual stack connection:
```shell
nmcli connection add ifname {{interface_name}} type {{ethernet}} ipv4.method {{auto}} ipv6.method {{auto}}
```
#### Create a static IPv6-only connection:
```shell
nmcli connection add ifname {{interface_name}} type {{ethernet}} ip6 {{2001:db8::2/64}} gw6 {{2001:db8::1}} ipv6.dns {{2001:db8::1}} ipv4.method {{ignore}}
```
#### Create a static IPv4-only connection:
```shell
nmcli connection add ifname {{interface_name}} type {{ethernet}} ip4 {{10.0.0.7/8}} gw4 {{10.0.0.1}} ipv4.dns {{10.0.0.1}} ipv6.method {{ignore}}
```
{% endraw %}{% raw %}
<h2 id="nmcli-device">
  <a href="/en/linux/nmcli-device.html">nmcli device</a> <a href="#nmcli-device"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Hardware device management with NetworkManager.
> More information: <https://man.archlinux.org/man/nmcli.1>.

#### Print the statuses of all network interfaces:
```shell
nmcli device status
```
#### Print the available Wi-Fi access points:
```shell
nmcli device wifi
```
#### Connect to the Wi-Fi network with a specified name and password:
```shell
nmcli device wifi connect {{ssid}} password {{password}}
```
#### Print password and QR code for the current Wi-Fi network:
```shell
nmcli device wifi show-password
```
{% endraw %}{% raw %}
<h2 id="nmcli">
  <a href="/en/linux/nmcli.html">nmcli</a> <a href="#nmcli"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line tool for controlling NetworkManager.
> More information: <https://man.archlinux.org/man/nmcli.1>.

#### Check the nmcli version:
```shell
nmcli --version
```
#### Call general help:
```shell
nmcli --help
```
#### Call help on a command:
```shell
nmcli {{command}} --help
```
#### Execute an `nmcli` command:
```shell
nmcli {{command}}
```
{% endraw %}{% raw %}
<h2 id="nmon">
  <a href="/en/linux/nmon.html">nmon</a> <a href="#nmon"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A system administrator, tuner, and benchmark tool.

#### Start nmon:
```shell
nmon
```
#### Save records to file ("-s 300 -c 288" by default):
```shell
nmon -f
```
#### Save records to file with a total of 240 measurements, by taking 30 seconds between each measurement:
```shell
nmon -f -s {{30}} -c {{240}}
```
{% endraw %}{% raw %}
<h2 id="nmtui">
  <a href="/en/linux/nmtui.html">nmtui</a> <a href="#nmtui"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Text user interface for controlling NetworkManager.
> Use arrow keys to navigate, enter to select an option.

#### Open the user interface:
```shell
nmtui
```
#### Show a list of available connections, with the option to activate or deactivate them:
```shell
nmtui connect
```
#### Connect to a given network:
```shell
nmtui connect {{name|uuid|device|SSID}}
```
#### Edit/Add/Delete a given network:
```shell
nmtui edit {{name|id}}
```
#### Set the system hostname:
```shell
nmtui hostname
```
{% endraw %}{% raw %}
<h2 id="nologin">
  <a href="/en/linux/nologin.html">nologin</a> <a href="#nologin"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Alternative shell that prevents a user from logging in.

#### Set a user's login shell to `nologin` to prevent the user from logging in:
```shell
chsh -s {{user}} nologin
```
#### Customize message for users with the login shell of `nologin`:
```shell
echo "{{declined_login_message}}" > /etc/nologin.txt
```
{% endraw %}{% raw %}
<h2 id="notify-send">
  <a href="/en/linux/notify-send.html">notify-send</a> <a href="#notify-send"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Uses the current desktop environment's notification system to create a notification.

#### Show a notification with the title "Test" and the content "This is a test":
```shell
notify-send "{{Test}}" "{{This is a test}}"
```
#### Show a notification with a custom icon:
```shell
notify-send -i {{icon.png}} "{{Test}}" "{{This is a test}}"
```
#### Show a notification for 5 seconds:
```shell
notify-send -t 5000 "{{Test}}" "{{This is a test}}"
```
#### Show a notification with an app's icon:
```shell
notify-send "{{Test}}" --icon={{google-chrome}}
```
{% endraw %}{% raw %}
<h2 id="nsenter">
  <a href="/en/linux/nsenter.html">nsenter</a> <a href="#nsenter"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run a new command in a running process' namespace.
> Particularly useful for docker images or chroot jails.
> More information: <https://github.com/jpetazzo/nsenter/>.

#### Run command in existing processes network namespace:
```shell
nsenter -t {{pid}} -n {{command}} {{command_arguments}}
```
#### Run a new command in an existing processes ps-table namespace:
```shell
nsenter -t {{pid}} -p {{command}} {{command_arguments}}
```
#### Run command in existing processes IPC namespace:
```shell
nsenter -t {{pid}} -i {{command}} {{command_arguments}}
```
{% endraw %}{% raw %}
<h2 id="nsnake">
  <a href="/en/linux/nsnake.html">nsnake</a> <a href="#nsnake"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Snake game in the terminal.
> More information: <https://github.com/alexdantas/nsnake/>.

#### Start a snake game:
```shell
nsnake
```
#### Navigate the snake:
```shell
{{Up|Down|Left|Right}} arrow key
```
#### Pause/unpause the game:
```shell
p
```
#### Quit the game:
```shell
q
```
#### Show help during the game:
```shell
h
```
{% endraw %}{% raw %}
<h2 id="ntfsfix">
  <a href="/en/linux/ntfsfix.html">ntfsfix</a> <a href="#ntfsfix"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Fix common problems on an NTFS partition.

#### Fix a given NTFS partition:
```shell
sudo ntfsfix {{/dev/sdXN}}
```
{% endraw %}{% raw %}
<h2 id="ntpq">
  <a href="/en/linux/ntpq.html">ntpq</a> <a href="#ntpq"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Query the Network Time Protocol (NTP) daemon.
> More information: <https://www.eecis.udel.edu/~mills/ntp/html/ntpq.html>.

#### Start `ntpq` in interactive mode:
```shell
ntpq --interactive
```
#### Print a list of NTP peers:
```shell
ntpq --peers
```
#### Print a list of NTP peers without resolving hostnames from IP addresses:
```shell
ntpq --numeric --peers
```
#### Use `ntpq` in debugging mode:
```shell
ntpq --debug-level
```
#### Print NTP system variables values:
```shell
ntpq --command={{rv}}
```
{% endraw %}{% raw %}
<h2 id="numactl">
  <a href="/en/linux/numactl.html">numactl</a> <a href="#numactl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Control NUMA policy for processes or shared memory.
> More information: <https://man7.org/linux/man-pages/man8/numactl.8.html>.

#### Run a command on node 0 with memory allocated on node 0 and 1:
```shell
numactl --cpunodebind={{0}} --membind={{0,1}} -- {{command}} {{command_arguments}}
```
#### Run a command on CPUs (cores) 0-4 and 8-12 of the current cpuset:
```shell
numactl --physcpubind={{+0-4,8-12}} -- {{command}} {{command_arguments}}
```
#### Run a command with its memory interleaved on all CPUs:
```shell
numactl --interleave={{all}} -- {{command}} {{command_arguments}}
```
{% endraw %}{% raw %}
<h2 id="numlockx">
  <a href="/en/linux/numlockx.html">numlockx</a> <a href="#numlockx"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Control the number lock key status in X11 sessions.
> More information: <http://www.mike-devlin.com/linux/README-numlockx.htm>.

#### Show the current number lock status:
```shell
numlockx status
```
#### Turn the number lock on:
```shell
numlockx on
```
#### Turn the number lock off:
```shell
numlockx off
```
#### Toggle the current state:
```shell
numlockx toggle
```
{% endraw %}{% raw %}
<h2 id="openfortivpn">
  <a href="/en/linux/openfortivpn.html">openfortivpn</a> <a href="#openfortivpn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A VPN client, for Fortinet's proprietary PPP+SSL VPN solution.
> More information: <https://github.com/adrienverge/openfortivpn>.

#### Connect to a VPN with a username and password:
```shell
openfortivpn --username={{username}} --password={{password}}
```
#### Connect to a VPN using a specific configuration file (defaults to `/etc/openfortivpn/config`):
```shell
sudo openfortivpn --config={{path/to/config}}
```
#### Connect to a VPN by specifying the host and port:
```shell
openfortivpn {{host}}:{{port}}
```
#### Trust a given gateway by passing in its certificate's sha256 sum:
```shell
openfortivpn --trusted-cert={{sha256_sum}}
```
{% endraw %}{% raw %}
<h2 id="openrc">
  <a href="/en/linux/openrc.html">openrc</a> <a href="#openrc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The OpenRC service manager.
> See also `rc-status`, `rc-update`, and `rc-service`.
> More information: <https://wiki.gentoo.org/wiki/OpenRC>.

#### Change to a specific runlevel:
```shell
sudo openrc {{runlevel_name}}
```
#### Change to a specific runlevel, but don't stop any existing services:
```shell
sudo openrc --no-stop {{runlevel_name}}
```
{% endraw %}{% raw %}
<h2 id="openvpn3">
  <a href="/en/linux/openvpn3.html">openvpn3</a> <a href="#openvpn3"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> OpenVPN 3 Linux client.
> More information: <https://community.openvpn.net/openvpn/wiki/OpenVPN3Linux>.

#### Start a new VPN session:
```shell
openvpn3 session-start --config {{path/to/config.conf}}
```
#### List established sessions:
```shell
openvpn3 sessions-list
```
#### Disconnect the currently established session started with given configuration:
```shell
openvpn3 session-manage --config {{path/to/config.conf}} --disconnect
```
#### Import VPN configuration:
```shell
openvpn3 config-import --config {{path/to/config.conf}}
```
#### List imported configurations:
```shell
openvpn3 configs-list
```
{% endraw %}{% raw %}
<h2 id="opkg">
  <a href="/en/linux/opkg.html">opkg</a> <a href="#opkg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A lightweight package manager used to install OpenWrt packages.

#### Install a package:
```shell
opkg install {{package}}
```
#### Remove a package:
```shell
opkg remove {{package}}
```
#### Update the list of available packages:
```shell
opkg update
```
#### Upgrade all the installed packages:
```shell
opkg upgrade
```
#### Upgrade one or more specific package(s):
```shell
opkg upgrade {{package(s)}}
```
#### Display information for a specific package:
```shell
opkg info {{package}}
```
#### List all the available packages:
```shell
opkg list
```
{% endraw %}{% raw %}
<h2 id="pacaur">
  <a href="/en/linux/pacaur.html">pacaur</a> <a href="#pacaur"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A utility for Arch Linux to build and install packages from the Arch User Repository.

#### Synchronize and update all packages (includes AUR):
```shell
pacaur -Syu
```
#### Synchronize and update only AUR packages:
```shell
pacaur -Syua
```
#### Install a new package (includes AUR):
```shell
pacaur -S {{package_name}}
```
#### Remove a package and its dependencies (includes AUR packages):
```shell
pacaur -Rs {{package_name}}
```
#### Search the package database for a keyword (includes AUR):
```shell
pacaur -Ss {{keyword}}
```
#### List all currently installed packages (includes AUR packages):
```shell
pacaur -Qs
```
{% endraw %}{% raw %}
<h2 id="paccache">
  <a href="/en/linux/paccache.html">paccache</a> <a href="#paccache"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A pacman cache cleaning utility.

#### Remove all but the 3 most recent package versions from the pacman cache:
```shell
paccache -r
```
#### Set the number of package versions to keep:
```shell
paccache -rk {{num_versions}}
```
#### Perform a dry-run and show the number of candidate packages for deletion:
```shell
paccache -d
```
#### Move candidate packages to a directory instead of deleting them:
```shell
paccache -m {{path/to/directory}}
```
{% endraw %}{% raw %}
<h2 id="pacman---database">
  <a href="/en/linux/pacman-database.html">pacman --database</a> <a href="#pacman---database"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Operate on the Arch Linux package database.
> Modify certain attributes of the installed packages.
> More information: <https://man.archlinux.org/man/pacman.8>.

#### Display help:
```shell
pacman --database --help
```
#### Mark a package as implicitly installed:
```shell
sudo pacman --database --asdeps {{package_name}}
```
#### Mark a package as explicitly installed:
```shell
sudo pacman --database --asexplicit {{package_name}}
```
#### Check that all the package dependencies are installed:
```shell
pacman --database --check
```
#### Check the repositories to ensure all specified dependencies are available:
```shell
pacman --database --check --check
```
#### Display only error messages:
```shell
pacman --database --check --quiet
```
{% endraw %}{% raw %}
<h2 id="pacman---deptest">
  <a href="/en/linux/pacman-deptest.html">pacman --deptest</a> <a href="#pacman---deptest"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Check each dependency specified and return a list of dependencies that are not currently satisfied on the system.
> More information: <https://man.archlinux.org/man/pacman.8>.

#### Print the package names of the dependencies that aren't installed:
```shell
pacman --deptest {{package_name1}} {{package_name2}}
```
#### Check if the installed package satisfies the given minimum version:
```shell
pacman --deptest "{{bash>=5}}"
```
#### Check if a later version of a package is installed:
```shell
pacman --deptest "{{bash>5}}"
```
#### Display help:
```shell
pacman --deptest --help
```
{% endraw %}{% raw %}
<h2 id="pacman---files">
  <a href="/en/linux/pacman-files.html">pacman --files</a> <a href="#pacman---files"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux package manager utility.
> See also `pkgfile`.
> More information: <https://man.archlinux.org/man/pacman.8>.

#### Display help:
```shell
pacman --files --help
```
#### Update the package database:
```shell
sudo pacman --files --refresh
```
#### Find the package that owns a specific file:
```shell
pacman --files {{filename}}
```
#### Find the package that owns a specific file, using a regular expression:
```shell
pacman --files --regex '{{regular_expression}}'
```
#### List only the package names:
```shell
pacman --files --quiet {{filename}}
```
#### List the files owned by a specific package:
```shell
pacman --files --list {{package_name}}
```
#### List only the absolute path to the files:
```shell
pacman --query --list --quiet {{package_name}}
```
{% endraw %}{% raw %}
<h2 id="pacman-mirrors">
  <a href="/en/linux/pacman-mirrors.html">pacman-mirrors</a> <a href="#pacman-mirrors"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate a pacman mirrorlist for Manjaro Linux.
> Every run of pacman-mirrors requires you to synchronize your database and update your system using `sudo pacman -Syyu`.
> More information: <https://wiki.manjaro.org/index.php?title=Pacman-mirrors>.

#### Generate a mirrorlist using the default settings:
```shell
sudo pacman-mirrors --fasttrack
```
#### Get the status of the current mirrors:
```shell
pacman-mirrors --status
```
#### Display the current branch:
```shell
pacman-mirrors --get-branch
```
#### Switch to a different branch:
```shell
sudo pacman-mirrors --api --set-branch {{stable|unstable|testing}}
```
#### Generate a mirrorlist, only using mirrors in your country:
```shell
sudo pacman-mirrors --geoip
```
{% endraw %}{% raw %}
<h2 id="pacman---query">
  <a href="/en/linux/pacman-query.html">pacman --query</a> <a href="#pacman---query"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux package manager utility.
> More information: <https://man.archlinux.org/man/pacman.8>.

#### List installed packages and versions:
```shell
pacman --query
```
#### List only packages and versions that were explicitly installed:
```shell
pacman --query --explicit
```
#### Find which package owns a file:
```shell
pacman --query --owns {{filename}}
```
#### Display information about an installed package:
```shell
pacman --query --info {{package_name}}
```
#### List files owned by a package:
```shell
pacman --query --list {{package_name}}
```
#### List orphan packages (installed as dependencies but not required by any package):
```shell
pacman --query --unrequired --deps --quiet
```
#### List installed packages not found in the repositories:
```shell
pacman --query --foreign
```
#### List outdated packages:
```shell
pacman --query --upgrades
```
{% endraw %}{% raw %}
<h2 id="pacman---remove">
  <a href="/en/linux/pacman-remove.html">pacman --remove</a> <a href="#pacman---remove"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux package manager utility.
> More information: <https://man.archlinux.org/man/pacman.8>.

#### Display help for this subcommand:
```shell
pacman --remove --help
```
#### Remove a package and its dependencies:
```shell
sudo pacman --remove --recursive {{package_name}}
```
#### Remove a package and both its dependencies and configuration files:
```shell
sudo pacman --remove --recursive --nosave {{package_name}}
```
#### Remove a package without prompting:
```shell
sudo pacman --remove --noconfirm {{package_name}}
```
#### Remove orphan packages (installed as dependencies but not required by any package):
```shell
sudo pacman --remove --recursive --nosave $(pacman --query --unrequired --deps --quiet)
```
#### Remove a package and all packages that depend on it:
```shell
sudo pacman --remove --cascade {{package_name}}
```
#### List packages that would be affected (does not remove any packages):
```shell
pacman --remove --print {{package_name}}
```
{% endraw %}{% raw %}
<h2 id="pacman---sync">
  <a href="/en/linux/pacman-sync.html">pacman --sync</a> <a href="#pacman---sync"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux package manager utility.
> More information: <https://man.archlinux.org/man/pacman.8>.

#### Install a new package:
```shell
sudo pacman --sync {{package_name}}
```
#### Synchronize and update all packages (add `--downloadonly` to download the packages and not update them):
```shell
sudo pacman --sync --refresh --sysupgrade
```
#### Update all packages and install a new one without prompting:
```shell
sudo pacman --sync --refresh --sysupgrade --noconfirm {{package_name}}
```
#### Search the package database for a regular expression or keyword:
```shell
pacman --sync --search "{{search_pattern}}"
```
#### Display information about a package:
```shell
pacman --sync --info {{package_name}}
```
#### Overwrite conflicting files during a package update:
```shell
sudo pacman --sync --refresh --sysupgrade --overwrite {{path/to/file}}
```
#### Synchronize and update all packages, but ignore a specific package (can be used more than once):
```shell
sudo pacman --sync --refresh --sysupgrade --ignore {{package_name}}
```
#### Remove not installed packages and unused repositories from the cache (use two `--clean` flags to clean all packages):
```shell
sudo pacman --sync --clean
```
{% endraw %}{% raw %}
<h2 id="pacman---upgrade">
  <a href="/en/linux/pacman-upgrade.html">pacman --upgrade</a> <a href="#pacman---upgrade"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux package manager utility.
> More information: <https://man.archlinux.org/man/pacman.8>.

#### Display help:
```shell
pacman --upgrade --help
```
#### Install one or more packages from files:
```shell
sudo pacman --upgrade {{path/to/package1.pkg.tar.zst}} {{path/to/package2.pkg.tar.zst}}
```
#### Install a package without prompting:
```shell
sudo pacman --upgrade --noconfirm {{path/to/package.pkg.tar.zst}}
```
#### Overwrite conflicting files during a package installation:
```shell
sudo pacman --upgrade --overwrite {{path/to/file}} {{path/to/package.pkg.tar.zst}}
```
#### Install a package, skipping the dependency version checks:
```shell
sudo pacman --upgrade --nodeps {{path/to/package.pkg.tar.zst}}
```
#### List packages that would be affected (does not install any packages):
```shell
pacman --query --print {{path/to/package.pkg.tar.zst}}
```
{% endraw %}{% raw %}
<h2 id="pacman">
  <a href="/en/linux/pacman.html">pacman</a> <a href="#pacman"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux package manager utility.
> More information: <https://man.archlinux.org/man/pacman.8>.

#### Synchronize and update all packages:
```shell
pacman --sync --refresh --sysupgrade
```
#### Install a new package:
```shell
pacman --sync {{package_name}}
```
#### Remove a package and its dependencies:
```shell
pacman --remove --recursive {{package_name}}
```
#### Search the package database for a regular expression or keyword:
```shell
pacman --sync --search "{{search_pattern}}"
```
#### List installed packages and versions:
```shell
pacman --query
```
#### List only the explicitly installed packages and versions:
```shell
pacman --query --explicit
```
#### List orphan packages (installed as dependencies but not actually required by any package):
```shell
pacman --query --unrequired --deps --quiet
```
#### Empty the entire pacman cache:
```shell
pacman --sync --clean --clean
```
{% endraw %}{% raw %}
<h2 id="pacman4console">
  <a href="/en/linux/pacman4console.html">pacman4console</a> <a href="#pacman4console"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A text-based console game inspired by the original Pacman.
> More information: <https://github.com/YoctoForBeaglebone/pacman4console>.

#### Start a game at Level 1:
```shell
pacman4console
```
#### Start a game on a certain level (there are nine official levels):
```shell
pacman4console --level={{level_number}}
```
#### Start the pacman4console level editor, saving to a specified text file:
```shell
pacman4consoleedit {{path/to/level_file}}
```
#### Play a custom level:
```shell
pacman4console --level={{path/to/level_file}}
```
{% endraw %}{% raw %}
<h2 id="pacstrap">
  <a href="/en/linux/pacstrap.html">pacstrap</a> <a href="#pacstrap"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux install script to install packages to the specified new root directory.
> More information: <https://man.archlinux.org/man/pacstrap.8>.

#### Install the `base` package, Linux kernel and firmware for common hardware:
```shell
pacstrap {{path/to/new/root}} {{base}} {{linux}} {{linux-firmware}}
```
#### Install the `base` package, Linux LTS kernel and `base-devel` build tools:
```shell
pacstrap {{path/to/new/root}} {{base}} {{base-devel}} {{linux-lts}}
```
#### Install packages without copy the host's mirrorlist to the target:
```shell
pacstrap -M {{path/to/new/root}} {{packages}}
```
#### Use an alternate configuration file for Pacman:
```shell
pacstrap -C {{path/to/pacman.conf}} {{path/to/new/root}} {{packages}}
```
#### Install packages using the package cache on the host instead of on the target:
```shell
pacstrap -c {{path/to/new/root}} {{packages}}
```
#### Install packages without copy the host's pacman keyring to the target:
```shell
pacstrap -G {{path/to/new/root}} {{packages}}
```
#### Install packages in interactive mode (prompts for confirmation):
```shell
pacstrap -i {{path/to/new/root}} {{packages}}
```
#### Install packages using package files:
```shell
pacstrap -U {{path/to/new/root}} {{path/to/package1}} {{path/to/package2}}
```
{% endraw %}{% raw %}
<h2 id="pamac">
  <a href="/en/linux/pamac.html">pamac</a> <a href="#pamac"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line utility for the GUI package manager pamac.
> If you can't see the AUR packages, enable it in `/etc/pamac.conf` or in the GUI.
> More information: <https://wiki.manjaro.org/index.php/Pamac>.

#### Install a new package:
```shell
pamac install {{package_name}}
```
#### Remove a package and its no longer required dependencies (orphans):
```shell
pamac remove --orphans {{package_name}}
```
#### Search the package database for a package:
```shell
pamac search {{package_name}}
```
#### List installed packages:
```shell
pamac list --installed
```
#### Check for package updates:
```shell
pamac checkupdates
```
#### Upgrade all packages:
```shell
pamac upgrade
```
{% endraw %}{% raw %}
<h2 id="parted">
  <a href="/en/linux/parted.html">parted</a> <a href="#parted"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A partition manipulation program.
> See also: `partprobe`.
> More information: <https://www.gnu.org/software/parted/parted.html>.

#### List partitions on all block devices:
```shell
sudo parted --list
```
#### Start interactive mode with the specified disk selected:
```shell
sudo parted {{/dev/sdX}}
```
#### Create a new partition table of the specified label-type:
```shell
sudo parted --script {{/dev/sdX}} mklabel {{aix|amiga|bsd|dvh|gpt|loop|mac|msdos|pc98|sun}}
```
#### Show partition information in interactive mode:
```shell
print
```
#### Select a disk in interactive mode:
```shell
select {{/dev/sdX}}
```
#### Create a 16GB partition with the specified filesystem in interactive mode:
```shell
mkpart {{primary|logical|extended}} {{btrfs|ext2|ext3|ext4|fat16|fat32|hfs|hfs+|linux-swap|ntfs|reiserfs|udf|xfs}} {{0%}} {{16G}}
```
#### Resize a partition in interactive mode:
```shell
resizepart {{/dev/sdXN}} {{end_position_of_partition}}
```
#### Remove a partition in interactive mode:
```shell
rm {{/dev/sdXN}}
```
{% endraw %}{% raw %}
<h2 id="partprobe">
  <a href="/en/linux/partprobe.html">partprobe</a> <a href="#partprobe"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Notify the operating system kernel of partition table changes.
> More information: <https://manned.org/partprobe>.

#### Notify the operating system kernel of partition table changes:
```shell
sudo partprobe
```
#### Notify the kernel of partition table changes and show a summary of devices and their partitions:
```shell
sudo partprobe --summary
```
#### Show a summary of devices and their partitions but don't notify the kernel:
```shell
sudo partprobe --summary --dry-run
```
{% endraw %}{% raw %}
<h2 id="partx">
  <a href="/en/linux/partx.html">partx</a> <a href="#partx"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Parse a partition table and tell the kernel about it.
> More information: <https://man7.org/linux/man-pages/man8/partx.8.html>.

#### List the partitions on a block device or disk image:
```shell
sudo partx --list {{path/to/device_or_disk_image}}
```
#### Add all the partitions found in a given block device to the kernel:
```shell
sudo partx --add --verbose {{path/to/device_or_disk_image}}
```
#### Delete all the partitions found from the kernel (does not alter partitions on disk):
```shell
sudo partx --delete {{path/to/device_or_disk_image}}
```
{% endraw %}{% raw %}
<h2 id="paru">
  <a href="/en/linux/paru.html">paru</a> <a href="#paru"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An AUR helper and pacman wrapper.
> More information: <https://github.com/Morganamilo/paru>.

#### Interactively search for and install a package:
```shell
paru {{package_name_or_seach_term}}
```
#### Synchronize and update all packages:
```shell
paru
```
#### Upgrade AUR packages:
```shell
paru -Sua
```
#### Get information about a package:
```shell
paru -Si {{package_name}}
```
#### Download `PKGBUILD` and other package source files from the AUR or ABS:
```shell
paru --getpkgbuild {{package_name}}
```
#### Display the `PKGBUILD` file of a package:
```shell
paru --getpkgbuild --print {{package_name}}
```
{% endraw %}{% raw %}
<h2 id="pasuspender">
  <a href="/en/linux/pasuspender.html">pasuspender</a> <a href="#pasuspender"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Temporarily suspends `pulseaudio` while another command is running to allow access to alsa.

#### Suspend pulseaudio while running `jackd`:
```shell
pasuspender -- {{jackd -d alsa --device hw:0}}
```
{% endraw %}{% raw %}
<h2 id="pdfgrep">
  <a href="/en/linux/pdfgrep.html">pdfgrep</a> <a href="#pdfgrep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Search text in PDF files.

#### Find lines that match pattern in a PDF:
```shell
pdfgrep {{pattern}} {{file.pdf}}
```
#### Include file name and page number for each matched line:
```shell
pdfgrep --with-filename --page-number {{pattern}} {{file.pdf}}
```
#### Do a case insensitive search for lines that begin with "foo" and return the first 3 matches:
```shell
pdfgrep --max-count {{3}} --ignore-case {{'^foo'}} {{file.pdf}}
```
#### Find pattern in files with a `.pdf` extension in the current directory recursively:
```shell
pdfgrep --recursive {{pattern}}
```
#### Find pattern on files that match a specific glob in the current directory recursively:
```shell
pdfgrep --recursive --include {{'*book.pdf'}} {{pattern}}
```
{% endraw %}{% raw %}
<h2 id="perf">
  <a href="/en/linux/perf.html">perf</a> <a href="#perf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Framework for linux performance counter measurements.

#### Display basic performance counter stats for a command:
```shell
perf stat {{gcc hello.c}}
```
#### Display system-wide real time performance counter profile:
```shell
sudo perf top
```
#### Run a command and record its profile into `perf.data`:
```shell
sudo perf record {{command}}
```
#### Read `perf.data` (created by `perf record`) and display the profile:
```shell
sudo perf report
```
{% endraw %}{% raw %}
<h2 id="rename">
  <a href="/en/linux/perl-rename.html">rename</a> <a href="#rename"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rename multiple files.
> NOTE: this page refers to the command from the `perl-rename` Arch Linux package.

#### Rename files using a Perl Common Regular Expression (substitute 'foo' with 'bar' wherever found):
```shell
rename {{'s/foo/bar/'}} {{*}}
```
#### Dry-run - display which renames would occur without performing them:
```shell
rename -n {{'s/foo/bar/'}} {{*}}
```
#### Force renaming even if the operation would remove existing destination files:
```shell
rename -f {{'s/foo/bar/'}} {{*}}
```
#### Convert filenames to lower case (use `-f` in case-insensitive filesystems to prevent "already exists" errors):
```shell
rename 'y/A-Z/a-z/' {{*}}
```
#### Replace whitespace with underscores:
```shell
rename 's/\s+/_/g' {{*}}
```
{% endraw %}{% raw %}
<h2 id="phar">
  <a href="/en/linux/phar.html">phar</a> <a href="#phar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create, update or extract PHP archives (PHAR).

#### Add space-separated files or directories to a Phar file:
```shell
phar add -f {{path/to/phar_file}} {{files_or_directories}}
```
#### Display the contents of a Phar file:
```shell
phar list -f {{path/to/phar_file}}
```
#### Delete the specified file or directory from a Phar file:
```shell
phar delete -f {{path/to/phar_file}} -e {{file_or_directory}}
```
#### Display full usage information and available hashing/compression algorithms:
```shell
phar help
```
#### Compress or uncompress files and directories in a Phar file:
```shell
phar compress -f {{path/to/phar_file}} -c {{algorithm}}
```
#### Get information about a Phar file:
```shell
phar info -f {{path/to/phar_file}}
```
#### Sign a Phar file with a specific hash algorithm:
```shell
phar sign -f {{path/to/phar_file}} -h {{algorithm}}
```
#### Sign a Phar file with an OpenSSL private key:
```shell
phar sign -f {{path/to/phar_file}} -h openssl -y {{path/to/private_key}}
```
{% endraw %}{% raw %}
<h2 id="photorec">
  <a href="/en/linux/photorec.html">photorec</a> <a href="#photorec"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Deleted file recovery tool.
> It is recommended to write recovered files to a disk separate to the one being recovered from.
> More information: <https://www.cgsecurity.org/wiki/PhotoRec>.

#### Run PhotoRec on a specific device:
```shell
sudo photorec {{/dev/sdb}}
```
#### Run PhotoRec on a disk image (`image.dd`):
```shell
sudo photorec {{path/to/image.dd}}
```
{% endraw %}{% raw %}
<h2 id="phpdismod">
  <a href="/en/linux/phpdismod.html">phpdismod</a> <a href="#phpdismod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Disable PHP extensions on Debian-based OSes.

#### Disable the json extension for every SAPI of every PHP version:
```shell
sudo phpdismod {{json}}
```
#### Disable the json extension for PHP 7.3 with the cli SAPI:
```shell
sudo phpdismod -v {{7.3}} -s {{cli}} {{json}}
```
{% endraw %}{% raw %}
<h2 id="phpenmod">
  <a href="/en/linux/phpenmod.html">phpenmod</a> <a href="#phpenmod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Enable PHP extensions on Debian-based OSes.

#### Enable the json extension for every SAPI of every PHP version:
```shell
sudo phpenmod {{json}}
```
#### Enable the json extension for PHP 7.3 with the cli SAPI:
```shell
sudo phpenmod -v {{7.3}} -s {{cli}} {{json}}
```
{% endraw %}{% raw %}
<h2 id="phpquery">
  <a href="/en/linux/phpquery.html">phpquery</a> <a href="#phpquery"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> PHP extension manager for Debian-based OSes.

#### List available PHP versions:
```shell
sudo phpquery -V
```
#### List available SAPIs for PHP 7.3:
```shell
sudo phpquery -v {{7.3}} -S
```
#### List enabled extensions for PHP 7.3 with the cli SAPI:
```shell
sudo phpquery -v {{7.3}} -s {{cli}} -M
```
#### Check if the json extension is enabled for PHP 7.3 with the apache2 SAPI:
```shell
sudo phpquery -v {{7.3}} -s {{apache2}} -m {{json}}
```
{% endraw %}{% raw %}
<h2 id="physlock">
  <a href="/en/linux/physlock.html">physlock</a> <a href="#physlock"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lock all consoles and virtual terminals.
> More information: <http://github.com/muennich/physlock>.

#### Lock every console (require current user or root to unlock):
```shell
physlock
```
#### Mute kernel messages on console while locked:
```shell
physlock -m
```
#### Disable SysRq mechanism while locked:
```shell
physlock -s
```
#### Display a message before the password prompt:
```shell
physlock -p "{{Locked!}}"
```
#### Fork and detach physlock (useful for suspend or hibernate scripts):
```shell
physlock -d
```
{% endraw %}{% raw %}
<h2 id="pi">
  <a href="/en/linux/pi.html">pi</a> <a href="#pi"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compute decimal Archimedes' constant Pi on the command-line.
> More information: <http://manpages.ubuntu.com/manpages/trusty/man1/pi.1.html>.

#### Display 100 decimal digits of Archimedes' constant Pi:
```shell
pi
```
#### Display a specified number of decimal digits of Archimedes' constant Pi:
```shell
pi {{number}}
```
#### Display help:
```shell
pi --help
```
#### Display version:
```shell
pi --version
```
#### Display recommended readings:
```shell
pi --bibliography
```
{% endraw %}{% raw %}
<h2 id="pidof">
  <a href="/en/linux/pidof.html">pidof</a> <a href="#pidof"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Gets the ID of a process using its name.

#### List all process IDs with given name:
```shell
pidof {{bash}}
```
#### List a single process ID with given name:
```shell
pidof -s {{bash}}
```
#### List process IDs including scripts with given name:
```shell
pidof -x {{script.py}}
```
#### Kill all processes with given name:
```shell
kill "$(pidof {{name}})" 
```
{% endraw %}{% raw %}
<h2 id="pidstat">
  <a href="/en/linux/pidstat.html">pidstat</a> <a href="#pidstat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show system resource usage, including CPU, memory, IO etc.

#### Show CPU statistics at a 2 second interval for 10 times:
```shell
pidstat {{2}} {{10}}
```
#### Show page faults and memory utilization:
```shell
pidstat -r
```
#### Show input/output usage per process id:
```shell
pidstat -d
```
#### Show information on a specific PID:
```shell
pidstat -p {{PID}}
```
#### Show memory statistics for all processes whose command name include "fox" or "bird":
```shell
pidstat -C "{{fox|bird}}" -r -p ALL
```
{% endraw %}{% raw %}
<h2 id="pihole">
  <a href="/en/linux/pihole.html">pihole</a> <a href="#pihole"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Terminal interface for the Pi-Hole ad-blocking DNS server.
> More information: <https://pi-hole.net>.

#### Check the Pi-hole daemon's status:
```shell
pihole status
```
#### Monitor detailed system status:
```shell
pihole chronometer
```
#### Start or stop the daemon:
```shell
pihole {{enable|disable}}
```
#### Restart the daemon (not the server itself):
```shell
pihole restartdns
```
#### Whitelist or blacklist a domain:
```shell
pihole {{whitelist|blacklist}} {{example.com}}
```
#### Search the lists for a domain:
```shell
pihole query {{example.com}}
```
{% endraw %}{% raw %}
<h2 id="pivpn">
  <a href="/en/linux/pivpn.html">pivpn</a> <a href="#pivpn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Easy security-hardened OpenVPN setup and manager.
> Originally designed for the Raspberry Pi, but works on other Linux devices too.
> More information: <http://www.pivpn.io/>.

#### Add a new client device:
```shell
sudo pivpn add
```
#### List all client devices:
```shell
sudo pivpn list
```
#### List currently connected devices and their statistics:
```shell
sudo pivpn clients
```
#### Revoke a previously authenticated device:
```shell
sudo pivpn revoke
```
#### Uninstall PiVPN:
```shell
sudo pivpn uninstall
```
{% endraw %}{% raw %}
<h2 id="pkg-config">
  <a href="/en/linux/pkg-config.html">pkg-config</a> <a href="#pkg-config"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Provide the details of installed libraries for compiling applications.
> More information: <https://www.freedesktop.org/wiki/Software/pkg-config/>.

#### Get the list of libraries and their dependencies:
```shell
pkg-config --libs {{library1 library2 ...}}
```
#### Get the list of libraries, their dependencies, and proper cflags for gcc:
```shell
pkg-config --cflags --libs {{library1 library2 ...}}
```
#### Compile your code with libgtk-3, libwebkit2gtk-4.0 and all their dependencies:
```shell
c++ example.cpp $(pkg-config --cflags --libs gtk+-3.0 webkit2gtk-4.0) -o example
```
{% endraw %}{% raw %}
<h2 id="pkgadd">
  <a href="/en/linux/pkgadd.html">pkgadd</a> <a href="#pkgadd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Add a package to a CRUX system.

#### Install a local software package:
```shell
pkgadd {{package_name}}
```
#### Update an already installed package from a local package:
```shell
pkgadd -u {{package_name}}
```
{% endraw %}{% raw %}
<h2 id="pkgfile">
  <a href="/en/linux/pkgfile.html">pkgfile</a> <a href="#pkgfile"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool for searching files from packages in the official repositories on arch-based systems.
> See also `pacman files`, describing the usage of `pacman --files`.
> More information: <https://man.archlinux.org/man/extra/pkgfile/pkgfile.1>.

#### Synchronize the pkgfile database:
```shell
sudo pkgfile --update
```
#### Search for a package that owns a specific file:
```shell
pkgfile {{filename}}
```
#### List all files provided by a package:
```shell
pkgfile --list {{package_name}}
```
#### List only files provided by a package located within the `bin` or `sbin` directory:
```shell
pkgfile --list --binaries {{package_name}}
```
#### Search for a package that owns a specific file using case insensitive matching:
```shell
pkgfile --ignorecase {{filename}}
```
#### Search for a package that owns a specific file in the `bin` or `sbin` directory:
```shell
pkgfile --binaries {{filename}}
```
#### Search for a package that owns a specific file, displaying the package version:
```shell
pkgfile --verbose {{filename}}
```
#### Search for a package that owns a specific file in a specific repository:
```shell
pkgfile --repo {{repository_name}} {{filename}}
```
{% endraw %}{% raw %}
<h2 id="pkginfo">
  <a href="/en/linux/pkginfo.html">pkginfo</a> <a href="#pkginfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Query the package database on a CRUX system.

#### List installed packages and their versions:
```shell
pkginfo -i
```
#### List files owned by a package:
```shell
pkginfo -l {{package_name}}
```
#### List the owner(s) of files matching a pattern:
```shell
pkginfo -o {{pattern}}
```
#### Print the footprint of a file:
```shell
pkginfo -f {{file}}
```
{% endraw %}{% raw %}
<h2 id="pkgmk">
  <a href="/en/linux/pkgmk.html">pkgmk</a> <a href="#pkgmk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Make a binary package for use with pkgadd on CRUX.

#### Make and download a package:
```shell
pkgmk -d
```
#### Install the package after making it:
```shell
pkgmk -d -i
```
#### Upgrade the package after making it:
```shell
pkgmk -d -u
```
#### Ignore the footprint when making a package:
```shell
pkgmk -d -if
```
#### Ignore the MD5 sum when making a package:
```shell
pkgmk -d -im
```
#### Update the package's footprint:
```shell
pkgmk -uf
```
{% endraw %}{% raw %}
<h2 id="pkgrm">
  <a href="/en/linux/pkgrm.html">pkgrm</a> <a href="#pkgrm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remove a package from a CRUX system.

#### Remove an installed package:
```shell
pkgrm {{package_name}}
```
{% endraw %}{% raw %}
<h2 id="playerctl">
  <a href="/en/linux/playerctl.html">playerctl</a> <a href="#playerctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility to control different media players.
> More information: <https://github.com/altdesktop/playerctl>.

#### Toggle play:
```shell
playerctl play-pause
```
#### Next media:
```shell
playerctl next
```
#### Previous media:
```shell
playerctl previous
```
#### List all players:
```shell
playerctl --list-all
```
#### Send a command to a specific player:
```shell
playerctl --player={{player_name}} {{command}}
```
#### Send a command to all players:
```shell
playerctl --all-players {{command}}
```
#### Show now playing:
```shell
playerctl metadata --format "Now playing: {{artist}} - {{album}} - {{title}}"
```
{% endraw %}{% raw %}
<h2 id="pmount">
  <a href="/en/linux/pmount.html">pmount</a> <a href="#pmount"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mount arbitrary hotpluggable devices as a normal user.
> More information: <https://manned.org/pmount>.

#### Mount a device below `/media/` (using device as mount point):
```shell
pmount {{/dev/to/block/device}}
```
#### Mount a device with a specific filesystem type to `/media/label`:
```shell
pmount --type {{filesystem}} {{/dev/to/block/device}} {{label}}
```
#### Mount a CD-ROM (filesystem type ISO9660) in read-only mode:
```shell
pmount --type {{iso9660}} --read-only {{/dev/cdrom}}
```
#### Mount an NTFS-formatted disk, forcing read-write access:
```shell
pmount --type {{ntfs}} --read-write {{/dev/sdX}}
```
#### Display all mounted removable devices:
```shell
pmount
```
{% endraw %}{% raw %}
<h2 id="ports">
  <a href="/en/linux/ports.html">ports</a> <a href="#ports"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Update/list the ports tree on a CRUX system.

#### Update the ports tree:
```shell
ports -u
```
#### List the ports in the current tree:
```shell
ports -l
```
#### Check the differences between installed packages and the ports tree:
```shell
ports -d
```
{% endraw %}{% raw %}
<h2 id="postfix">
  <a href="/en/linux/postfix.html">postfix</a> <a href="#postfix"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Postfix mail transfer agent (MTA) control program.
> See also `dovecot`, a mail delivery agent (MDA) that integrates with Postfix.
> More information: <http://postfix.org>.

#### Check the configuration:
```shell
sudo postfix check
```
#### Check the status of the Postfix daemon:
```shell
sudo postfix status
```
#### Start Postfix:
```shell
sudo postfix start
```
#### Gracefully stop Postfix:
```shell
sudo postfix stop
```
#### Flush the mail queue:
```shell
sudo postfix flush
```
#### Reload the configuration files:
```shell
sudo postfix reload
```
{% endraw %}{% raw %}
<h2 id="poweroff">
  <a href="/en/linux/poweroff.html">poweroff</a> <a href="#poweroff"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Power off the system.
> More information: <https://www.man7.org/linux/man-pages/man8/poweroff.8.html>.

#### Power off the system:
```shell
poweroff
```
#### Halt the system (same as `halt`):
```shell
poweroff --halt
```
#### Reboot the system (same as `reboot`):
```shell
poweroff --reboot
```
#### Shut down immediately without contacting the system manager:
```shell
poweroff --force --force
```
#### Write the wtmp shutdown entry without shutting down the system:
```shell
poweroff --wtmp-only
```
{% endraw %}{% raw %}
<h2 id="powertop">
  <a href="/en/linux/powertop.html">powertop</a> <a href="#powertop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Optimize battery power usage.

#### Calibrate power usage measurements:
```shell
sudo powertop --calibrate
```
#### Generate HTML power usage report in the current directory:
```shell
sudo powertop --html={{power_report.html}}
```
#### Tune to optimal settings:
```shell
sudo powertop --auto-tune
```
{% endraw %}{% raw %}
<h2 id="rename">
  <a href="/en/linux/prename.html">rename</a> <a href="#rename"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rename multiple files.
> NOTE: this page refers to the command from the `prename` Fedora package.

#### Rename files using a Perl Common Regular Expression (substitute 'foo' with 'bar' wherever found):
```shell
rename {{'s/foo/bar/'}} {{*}}
```
#### Dry-run - display which renames would occur without performing them:
```shell
rename -n {{'s/foo/bar/'}} {{*}}
```
#### Force renaming even if the operation would remove existing destination files:
```shell
rename -f {{'s/foo/bar/'}} {{*}}
```
#### Convert filenames to lower case (use `-f` in case-insensitive filesystems to prevent "already exists" errors):
```shell
rename 'y/A-Z/a-z/' {{*}}
```
#### Replace whitespace with underscores:
```shell
rename 's/\s+/_/g' {{*}}
```
{% endraw %}{% raw %}
<h2 id="print">
  <a href="/en/linux/print.html">print</a> <a href="#print"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An alias to a `run-mailcap`'s action print.
> Originally `run-mailcap` is used to process mime-type/file.

#### Print action can be used to print any file on default run-mailcap tool:
```shell
print {{filename}}
```
#### With `run-mailcap`:
```shell
run-mailcap --action=print {{filename}}
```
{% endraw %}{% raw %}
<h2 id="progress">
  <a href="/en/linux/progress.html">progress</a> <a href="#progress"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display/Monitor the progress of running coreutils.
> More information: <https://github.com/Xfennec/progress>.

#### Show the progress of running coreutils:
```shell
progress
```
#### Show the progress of running coreutils in quiet mode:
```shell
progress -q
```
#### Launch and monitor a single long-running command:
```shell
{{command}} & progress -mp $!
```
{% endraw %}{% raw %}
<h2 id="protontricks">
  <a href="/en/linux/protontricks.html">protontricks</a> <a href="#protontricks"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A simple wrapper that does Winetricks things for Proton enabled games, requires Winetricks.
> More information: <https://github.com/Matoking/protontricks>.

#### Show the protontricks help message:
```shell
protontricks
```
#### Run the protontricks GUI:
```shell
protontricks --gui
```
#### Run Winetricks for a specific game:
```shell
protontricks {{appid}} {{winetricks_args}}
```
#### Run a command within a games installation directory:
```shell
protontricks -c {{command}} {{appid}}
```
{% endraw %}{% raw %}
<h2 id="prt-get">
  <a href="/en/linux/prt-get.html">prt-get</a> <a href="#prt-get"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The CRUX package manager.

#### Install a package:
```shell
prt-get install {{package_name}}
```
#### Install a package with dependency handling:
```shell
prt-get depinst {{package_name}}
```
#### Update a package manually:
```shell
prt-get upgrade {{package_name}}
```
#### Remove a package:
```shell
prt-get remove {{package_name}}
```
#### Upgrade the system from the local ports tree:
```shell
prt-get sysup
```
#### Search the ports tree:
```shell
prt-get search {{package_name}}
```
#### Search for a file in a package:
```shell
prt-get fsearch {{file}}
```
{% endraw %}{% raw %}
<h2 id="pstree">
  <a href="/en/linux/pstree.html">pstree</a> <a href="#pstree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A convenient tool to show running processes as a tree.

#### Display a tree of processes:
```shell
pstree
```
#### Display a tree of processes with PIDs:
```shell
pstree -p
```
#### Display all process trees rooted at processes owned by specified user:
```shell
pstree {{user}}
```
{% endraw %}{% raw %}
<h2 id="ptx">
  <a href="/en/linux/ptx.html">ptx</a> <a href="#ptx"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate a permuted index of words from one or more text files.
> More information: <https://www.gnu.org/software/coreutils/ptx>.

#### Generate a permuted index where the first field of each line is an index reference:
```shell
ptx --references {{path/to/file}}
```
#### Generate a permuted index with automatically generated index references:
```shell
ptx --auto-reference {{path/to/file}}
```
#### Generate a permuted index with a fixed width:
```shell
ptx --width={{width_in_columns}} {{path/to/file}}
```
#### Generate a permuted index with a list of filtered words:
```shell
ptx --only-file={{path/to/filter}} {{path/to/file}}
```
#### Generate a permuted index with SYSV-style behaviors:
```shell
ptx --traditional {{path/to/file}}
```
{% endraw %}{% raw %}
<h2 id="pulseaudio">
  <a href="/en/linux/pulseaudio.html">pulseaudio</a> <a href="#pulseaudio"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The pulseaudio sound system daemon and manager.
> More information: <https://www.freedesktop.org/wiki/Software/PulseAudio/>.

#### Check if pulseaudio is running (a non-zero exit code means it is not running):
```shell
pulseaudio --check
```
#### Start the pulseaudio daemon in the background:
```shell
pulseaudio --start
```
#### Kill the running pulseaudio daemon:
```shell
pulseaudio --kill
```
#### List available modules:
```shell
pulseaudio --dump-modules
```
#### Load a module into the currently running daemon with the specified arguments:
```shell
pulseaudio --load="{{module_name}} {{arguments}}"
```
{% endraw %}{% raw %}
<h2 id="pvcreate">
  <a href="/en/linux/pvcreate.html">pvcreate</a> <a href="#pvcreate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Initialize a disk or partition for use as a physical volume.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/pvcreate.8.html>.

#### Initialize the `/dev/sda1` volume for use by LVM:
```shell
pvcreate {{/dev/sda1}}
```
#### Force the creation without any confirmation prompts:
```shell
pvcreate --force {{/dev/sda1}}
```
{% endraw %}{% raw %}
<h2 id="pvdisplay">
  <a href="/en/linux/pvdisplay.html">pvdisplay</a> <a href="#pvdisplay"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display information about Logical Volume Manager (LVM) physical volumes.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/pvdisplay.8.html>.

#### Display information about all physical volumes:
```shell
sudo pvdisplay
```
#### Display information about the physical volume on drive `/dev/sdXY`:
```shell
sudo pvdisplay {{/dev/sdXY}}
```
{% endraw %}{% raw %}
<h2 id="pvs">
  <a href="/en/linux/pvs.html">pvs</a> <a href="#pvs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display information about physical volumes.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/pvs.8.html>.

#### Display information about physical volumes:
```shell
pvs
```
#### Display non-physical volumes:
```shell
pvs -a
```
#### Change default display to show more details:
```shell
pvs -v
```
#### Display only specific fields:
```shell
pvs -o {{field_name_1}},{{field_name_2}}
```
#### Append field to default display:
```shell
pvs -o +{{field_name}}
```
#### Suppress heading line:
```shell
pvs --noheadings
```
#### Use separator to separate fields:
```shell
pvs --separator {{special_character}}
```
{% endraw %}{% raw %}
<h2 id="pwdx">
  <a href="/en/linux/pwdx.html">pwdx</a> <a href="#pwdx"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print working directory of a process.

#### Print current working directory of a process:
```shell
pwdx {{process_id}}
```
{% endraw %}{% raw %}
<h2 id="pwgen">
  <a href="/en/linux/pwgen.html">pwgen</a> <a href="#pwgen"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate pronounceable passwords.

#### Generate random password with s[y]mbols:
```shell
pwgen -y {{length}}
```
#### Generate secure, hard-to-memorize passwords:
```shell
pwgen -s {{length}}
```
#### Generate password with at least one capital letter in them:
```shell
pwgen -c {{length}}
```
{% endraw %}{% raw %}
<h2 id="qjoypad">
  <a href="/en/linux/qjoypad.html">qjoypad</a> <a href="#qjoypad"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Translate input from gamepads or joysticks into keyboard strokes or mouse actions.
> More information: <http://qjoypad.sourceforge.net/>.

#### Start QJoyPad:
```shell
qjoypad
```
#### Start QJoyPad and look for devices in a specific directory:
```shell
qjoypad --device={{path/to/directory}}
```
#### Start QJoyPad but don't show a system tray icon:
```shell
qjoypad --notray
```
#### Start QJoyPad and force the window manager to use a system tray icon:
```shell
qjoypad --force-tray
```
#### Force a running instance of QJoyPad to update its list of devices and layouts:
```shell
qjoypad --update
```
#### Load the given layout in an already running instance of QJoyPad, or start QJoyPad using the given layout:
```shell
qjoypad "{{layout}}"
```
{% endraw %}{% raw %}
<h2 id="qsub">
  <a href="/en/linux/qsub.html">qsub</a> <a href="#qsub"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Submits a script to the queue management system TORQUE.

#### Submit a script with default settings (depends on TORQUE settings):
```shell
qsub {{script.sh}}
```
#### Submit a script with a specified wallclock runtime limit of 1 hour, 2 minutes and 3 seconds:
```shell
qsub -l walltime={{1}}:{{2}}:{{3}} {{script.sh}}
```
#### Submit a script that is executed on 2 nodes using 4 cores per node:
```shell
qsub -l nodes={{2}}:ppn={{4}} {{script.sh}}
```
#### Submit a script to a specific queue. Note that different queues can have different maximum and minimum runtime limits:
```shell
qsub -q {{queue_name}} {{script.sh}}
```
{% endraw %}{% raw %}
<h2 id="qtchooser">
  <a href="/en/linux/qtchooser.html">qtchooser</a> <a href="#qtchooser"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A wrapper used to select between Qt development binary versions.
> More information: <https://manned.org/qtchooser>.

#### List available Qt versions from the configuration files:
```shell
qtchooser --list-versions
```
#### Print environment information:
```shell
qtchooser --print-env
```
#### Run the specified tool using the specified Qt version:
```shell
qtchooser --run-tool={{tool}} --qt={{version_name}}
```
#### Add a Qt version entry to be able to choose from:
```shell
qtchooser --install {{version_name}} {{path/to/qmake}}
```
#### Display all available options:
```shell
qtchooser --help
```
{% endraw %}{% raw %}
<h2 id="quotacheck">
  <a href="/en/linux/quotacheck.html">quotacheck</a> <a href="#quotacheck"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Scan a filesystem for disk usage; create, check and repair quota files.
> It is best to run quota check with quotas turned off to prevent damage or loss to quota files.

#### Check quotas on all mounted non-NFS filesystems:
```shell
sudo quotacheck --all
```
#### Force check even if quotas are enabled (this can cause damage or loss to quota files):
```shell
sudo quotacheck --force {{mountpoint}}
```
#### Check quotas on a given filesystem in debug mode:
```shell
sudo quotacheck --debug {{mountpoint}}
```
#### Check quotas on a given filesystem, displaying the progress:
```shell
sudo quotacheck --verbose {{mountpoint}}
```
#### Check user quotas:
```shell
sudo quotacheck --user {{user}} {{mountpoint}}
```
#### Check group quotas:
```shell
sudo quotacheck --group {{group}} {{mountpoint}}
```
{% endraw %}{% raw %}
<h2 id="radeontop">
  <a href="/en/linux/radeontop.html">radeontop</a> <a href="#radeontop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show utilisation of AMD GPUs.
> More information: <https://github.com/clbr/radeontop>.

#### Show the utilisation of the default AMD GPU:
```shell
sudo radeontop
```
#### Enable colourised output:
```shell
sudo radeontop --colour
```
#### Select a specific GPU (the bus number is the first number in the output of `lspci`):
```shell
sudo radeontop --bus {{bus_number}}
```
#### Specify the display refresh rate (higher means more GPU overhead):
```shell
sudo radeontop --ticks {{samples_per_second}}
```
{% endraw %}{% raw %}
<h2 id="rankmirrors">
  <a href="/en/linux/rankmirrors.html">rankmirrors</a> <a href="#rankmirrors"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rank a list of Pacman mirrors by connection and opening speed.
> Writes the new mirrorlist to stdout.
> More information: <https://wiki.archlinux.org/index.php/mirrors>.

#### Rank a mirror list:
```shell
rankmirrors {{/etc/pacman.d/mirrorlist}}
```
#### Output only a given number of the top ranking servers:
```shell
rankmirrors -n {{number}} {{/etc/pacman.d/mirrorlist}}
```
#### Be verbose when generating the mirrorlist:
```shell
rankmirrors -v {{/etc/pacman.d/mirrorlist}}
```
#### Test only a specific URL:
```shell
rankmirrors --url {{url}}
```
#### Output only the response times instead of a full mirrorlist:
```shell
rankmirrors --times {{/etc/pacman.d/mirrorlist}}
```
{% endraw %}{% raw %}
<h2 id="rc-service">
  <a href="/en/linux/rc-service.html">rc-service</a> <a href="#rc-service"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Locate and run OpenRC services with arguments.
> See also `openrc`.

#### Show a service's status:
```shell
rc-service {{service_name}} status
```
#### Start a service:
```shell
sudo rc-service {{service_name}} start
```
#### Stop a service:
```shell
sudo rc-servie {{service_name}} stop
```
#### Restart a service:
```shell
sudo rc-service {{service_name}} restart
```
#### Simulate running a service's custom command:
```shell
sudo rc-service --dry-run {{service_name}} {{command_name}}
```
#### Actually run a service's custom command:
```shell
sudo rc-service {{service_name}} {{command_name}}
```
#### Resolve the location of a service definition on disk:
```shell
sudo rc-service --resolve {{service_name}}
```
{% endraw %}{% raw %}
<h2 id="rc-status">
  <a href="/en/linux/rc-status.html">rc-status</a> <a href="#rc-status"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show status info about runlevels.
> See also `openrc`.

#### Show a summary of services and their status:
```shell
rc-status
```
#### Include services in all runlevels in the summary:
```shell
rc-status --all
```
#### List services that have crashed:
```shell
rc-status --crashed
```
#### List manually started services:
```shell
rc-status --manual
```
#### List supervised services:
```shell
rc-status --supervised
```
#### Get the current runlevel:
```shell
rc-status --runlevel
```
#### List all runlevels:
```shell
rc-status --list
```
{% endraw %}{% raw %}
<h2 id="rc-update">
  <a href="/en/linux/rc-update.html">rc-update</a> <a href="#rc-update"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Add and remove OpenRC services to and from runlevels.
> See also `openrc`.

#### List all services and the runlevels they are added to:
```shell
rc-update show
```
#### Add a service to a runlevel:
```shell
sudo rc-update add {{service_name}} {{runlevel}}
```
#### Delete a service from a runlevel:
```shell
sudo rc-update delete {{service_name}} {{runlevel}}
```
#### Delete a service from all runlevels:
```shell
sudo rc-update --all delete {{service_name}}
```
{% endraw %}{% raw %}
<h2 id="rdesktop">
  <a href="/en/linux/rdesktop.html">rdesktop</a> <a href="#rdesktop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remote Desktop Protocol client.
> It can be used to connect the remote computer using the RDP protocol.

#### Connect to a remote computer (default port is 3389):
```shell
rdesktop -u {{username}} -p {{password}} {{host:port}}
```
#### Simple Examples:
```shell
rdesktop -u Administrator -p passwd123 192.168.1.111:3389
```
#### Connect to a remote computer with full screen (press `Ctrl + Alt + Enter` to exist):
```shell
rdesktop -u {{username}} -p {{password}} -f {{host:port}}
```
#### Use the customed resolution (use the letter 'x' between the number):
```shell
rdesktop -u {{username}} -p {{password}} -g 1366x768 {{host:port}}
```
#### Connect to a remote computer using domain user:
```shell
rdesktop -u {{username}} -p {{password}} -d {{domainname}} {{host:port}}
```
#### Use the 16 bit color (speed up):
```shell
rdesktop -u {{username}} -p {{password}} -a 16 {{host:port}}
```
{% endraw %}{% raw %}
<h2 id="readelf">
  <a href="/en/linux/readelf.html">readelf</a> <a href="#readelf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Displays information about ELF files.
> More information: <http://man7.org/linux/man-pages/man1/readelf.1.html>.

#### Display all information about the ELF file:
```shell
readelf -all {{path/to/binary}}
```
#### Display all the headers present in the ELF file:
```shell
readelf --headers {{path/to/binary}}
```
#### Display the entries in symbol table section of the ELF file, if it has one:
```shell
readelf --symbols {{path/to/binary}}
```
#### Display the information contained in the ELF header at the start of the file:
```shell
readelf --file-header {{path/to/binary}}
```
{% endraw %}{% raw %}
<h2 id="reboot">
  <a href="/en/linux/reboot.html">reboot</a> <a href="#reboot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Reboot the system.
> More information: <https://www.man7.org/linux/man-pages/man8/reboot.8.html>.

#### Reboot the system:
```shell
reboot
```
#### Power off the system (same as `poweroff`):
```shell
reboot --poweroff
```
#### Halt the system (same as `halt`):
```shell
reboot --halt
```
#### Reboot immediately without contacting the system manager:
```shell
reboot --force --force
```
#### Write the wtmp shutdown entry without rebooting the system:
```shell
reboot --wtmp-only
```
{% endraw %}{% raw %}
<h2 id="reflector">
  <a href="/en/linux/reflector.html">reflector</a> <a href="#reflector"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch script to fetch and sort mirrorlists.

#### Get all mirrors, sort for download speed and save them:
```shell
sudo reflector --sort {{rate}} --save {{/etc/pacman.d/mirrorlist}}
```
#### Only get German HTTPS mirrors:
```shell
reflector --country {{Germany}} --protocol {{https}}
```
#### Only get the 10 recently sync'd mirrors:
```shell
reflector --latest {{10}}
```
{% endraw %}{% raw %}
<h2 id="rename">
  <a href="/en/linux/rename.html">rename</a> <a href="#rename"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rename multiple files.
> NOTE: this page refers to the command from the `util-linux` package.
> For the Perl version, see `file-rename` or `perl-rename`.
> Warning: This command has no safeguards and will overwrite files without prompting.

#### Rename files using simple substitutions (substitute 'foo' with 'bar' wherever found):
```shell
rename {{foo}} {{bar}} {{*}}
```
#### Dry-run - display which renames would occur without performing them:
```shell
rename -vn {{foo}} {{bar}} {{*}}
```
#### Do not overwrite existing files:
```shell
rename -o {{foo}} {{bar}} {{*}}
```
#### Change file extensions:
```shell
rename {{.ext}} {{.bak}} {{*.ext}}
```
#### Prepend "foo" to all filenames in the current directory:
```shell
rename {{''}} {{'foo'}} {{*}}
```
#### Rename a group of increasingly numbered files zero-padding the numbers up to 3 digits:
```shell
rename {{foo}} {{foo00}} {{foo?}} && rename {{foo}} {{foo0}} {{foo??}}
```
{% endraw %}{% raw %}
<h2 id="reportbug">
  <a href="/en/linux/reportbug.html">reportbug</a> <a href="#reportbug"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bug report tool of Debian distribution.
> More information: <https://manpages.debian.org/buster/reportbug/reportbug.1.en.html>.

#### Generate a bug report about a specific package, then send it by e-mail:
```shell
reportbug {{package}}
```
#### Report a bug that is not about a specific package (general problem, infrastructure, etc.):
```shell
reportbug other
```
#### Write the bug report to a file instead of sending it by e-mail:
```shell
reportbug -o {{filename}} {{package}}
```
{% endraw %}{% raw %}
<h2 id="repquota">
  <a href="/en/linux/repquota.html">repquota</a> <a href="#repquota"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display a summary of existing file quotas for a filesystem.

#### Report stats for all quotas in use:
```shell
sudo repquota -all
```
#### Report quota stats for all users, even those who aren't using any of their quota:
```shell
sudo repquota -v {{filesystem}}
```
#### Report on quotas for users only:
```shell
repquota --user {{filesystem}}
```
#### Report on quotas for groups only:
```shell
sudo repquota --group {{filesystem}}
```
#### Report on used quota and limits in a human-readable format:
```shell
sudo repquota --human-readable {{filesystem}}
```
#### Report on all quotas for users and groups in a human-readable format:
```shell
sudo repquota -augs
```
{% endraw %}{% raw %}
<h2 id="reset">
  <a href="/en/linux/reset.html">reset</a> <a href="#reset"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Reinitialises the current terminal. Clears the entire terminal screen.

#### Reinitialise the current terminal:
```shell
reset
```
#### Display the terminal type instead:
```shell
reset -q
```
{% endraw %}{% raw %}
<h2 id="resize2fs">
  <a href="/en/linux/resize2fs.html">resize2fs</a> <a href="#resize2fs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Resize an ext2, ext3 or ext4 filesystem.
> Does not resize the underlying partition, and the filesystem must be unmounted.

#### Automatically resize a filesystem:
```shell
resize2fs {{/dev/sdXN}}
```
#### Resize the filesystem to a size of 40G, displaying a progress bar:
```shell
resize2fs -p {{/dev/sdXN}} {{40G}}
```
#### Shrink the filesystem to its minimum possible size:
```shell
resize2fs -M {{/dev/sdXN}}
```
{% endraw %}{% raw %}
<h2 id="resolveip">
  <a href="/en/linux/resolveip.html">resolveip</a> <a href="#resolveip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Resolve hostnames to their IP addresses and vice versa.
> More information: <https://mariadb.com/kb/en/resolveip/>.

#### Resolve a hostname to an IP address:
```shell
resolveip {{example.org}}
```
#### Resolve an IP address to a hostname:
```shell
resolveip {{1.1.1.1}}
```
#### Silent mode. Produces less output:
```shell
resolveip --silent {{example.org}}
```
{% endraw %}{% raw %}
<h2 id="rfkill">
  <a href="/en/linux/rfkill.html">rfkill</a> <a href="#rfkill"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Enable and disable wireless devices.

#### List devices:
```shell
rfkill
```
#### Filter by columns:
```shell
rfkill -o {{ID,TYPE,DEVICE}}
```
#### Block devices by type (e.g. bluetooth, wlan):
```shell
rfkill block {{bluetooth}}
```
#### Unblock devices by type (e.g. bluetooth, wlan):
```shell
rfkill unblock {{wlan}}
```
#### Output in JSON format:
```shell
rfkill -J
```
{% endraw %}{% raw %}
<h2 id="rig">
  <a href="/en/linux/rig.html">rig</a> <a href="#rig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility to piece together a random first name, last name, street number and address, along with a geographically consistent (ie, they all match the same area) city, state, ZIP code, and area code.
> More information: <https://manpages.ubuntu.com/manpages/focal/man6/rig.6.html>.

#### Display a random name (male or female) and address:
```shell
rig
```
#### Display a [m]ale (or [f]emale) random name and address:
```shell
rig -{{m|f}}
```
#### Use data files from a specific directory (default is `/usr/share/rig`):
```shell
rig -d {{path/to/directory}}
```
#### Display a specific number of identities:
```shell
rig -c {{number}}
```
#### Display a specific number of female identities:
```shell
rig -f -c {{number}}
```
{% endraw %}{% raw %}
<h2 id="rofi">
  <a href="/en/linux/rofi.html">rofi</a> <a href="#rofi"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An application launcher and window switcher.
> More information: <https://github.com/davatorium/rofi>.

#### Show the list of apps:
```shell
rofi -show drun
```
#### Show the list of all commands:
```shell
rofi -show run
```
#### Switch between windows:
```shell
rofi -show window
```
#### Pipe a list of items to stdin and print the selected item to stdout:
```shell
printf "{{Choice1\nChoice2\nChoice3}}" | rofi -dmenu
```
{% endraw %}{% raw %}
<h2 id="rolldice">
  <a href="/en/linux/rolldice.html">rolldice</a> <a href="#rolldice"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Roll virtual dice.
> More information: <https://manned.org/rolldice>.

#### Roll a single 20 sided dice:
```shell
rolldice d{{20}}
```
#### Roll two six sided dice and drop the lowest roll:
```shell
rolldice {{2}}d{{6}}s{{1}}
```
#### Roll two 20 sided dice and add a modifier value:
```shell
rolldice {{2}}d{{20}}{{+5}}
```
#### Roll a 20 sided dice two times:
```shell
rolldice {{2}}xd{{20}}
```
{% endraw %}{% raw %}
<h2 id="rpcclient">
  <a href="/en/linux/rpcclient.html">rpcclient</a> <a href="#rpcclient"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> MS-RPC client tool (part of the samba suite).
> More information: <https://www.samba.org/samba/docs/current/man-html/rpcclient.1.html>.

#### Connect to a remote host:
```shell
rpcclient --user {{domain}}\{{username}}%{{password}} {{ip}}
```
#### Connect to a remote host on a domain without a password:
```shell
rpcclient --user {{username}} --workgroup {{domain}} --no-pass {{ip}}
```
#### Connect to a remote host, passing the password hash:
```shell
rpcclient --user {{domain}}\{{username}} --pw-nt-hash {{ip}}
```
#### Execute shell commands on a remote host:
```shell
rpcclient --user {{domain}}\{{username}}%{{password}} --command {{semicolon_separated_commands}} {{ip}}
```
#### Display domain users:
```shell
rpcclient $> enumdomusers
```
#### Display privileges:
```shell
rpcclient $> enumprivs
```
#### Display information about a specific user:
```shell
rpcclient $> queryuser {{username|rid}}
```
#### Create a new user in the domain:
```shell
rpcclient $> createdomuser {{username}}
```
{% endraw %}{% raw %}
<h2 id="rpcinfo">
  <a href="/en/linux/rpcinfo.html">rpcinfo</a> <a href="#rpcinfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Makes an RPC call to an RPC server and reports what it finds.

#### Show full table of all RPC services registered on localhost:
```shell
rpcinfo
```
#### Show concise table of all RPC services registered on localhost:
```shell
rpcinfo -s {{localhost}}
```
#### Display table of statistics of rpcbind operations on localhost:
```shell
rpcinfo -m
```
#### Display list of entries of given service name (mountd) and version number (2) on a remote nfs share:
```shell
rpcinfo -l {{remote_nfs_server_ip}} {{mountd}} {{2}}
```
#### Delete the registration for version 1 of the mountd service for all transports:
```shell
rpcinfo -d {{mountd}} {{1}}
```
{% endraw %}{% raw %}
<h2 id="rpm">
  <a href="/en/linux/rpm.html">rpm</a> <a href="#rpm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> RPM Package Manager.

#### Show version of httpd package:
```shell
rpm -q {{httpd}}
```
#### List versions of all matching packages:
```shell
rpm -qa '{{mariadb*}}'
```
#### Forcibly install a package regardless of currently installed versions:
```shell
rpm -U {{package_name.rpm}} --force
```
#### Identify owner of a file and show version of the package:
```shell
rpm -qf {{/etc/postfix/main.cf}}
```
#### List package-owned files:
```shell
rpm -ql {{kernel}}
```
#### Show scriptlets from an RPM file:
```shell
rpm -qp --scripts {{package_name.rpm}}
```
#### Show changed, missing and/or incorrectly installed files of matching packages:
```shell
rpm -Va '{{php-*}}'
```
{% endraw %}{% raw %}
<h2 id="rpmbuild">
  <a href="/en/linux/rpmbuild.html">rpmbuild</a> <a href="#rpmbuild"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> RPM Package Build tool.
> More information: <https://docs.fedoraproject.org/en-US/quick-docs/creating-rpm-packages/>.

#### Build binary and source packages:
```shell
rpmbuild -ba {{path/to/spec_file}}
```
#### Build a binary package without source package:
```shell
rpmbuild -bb {{path/to/spec_file}}
```
#### Specify additional variables when building a package:
```shell
rpmbuild -bb {{path/to/spec_file}} --define "{{variable1}} {{value1}}" --define "{{variable2}} {{value2}}"
```
{% endraw %}{% raw %}
<h2 id="rspamc">
  <a href="/en/linux/rspamc.html">rspamc</a> <a href="#rspamc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line client for rspamd servers.

#### Train the bayesian filter to recognise an email as spam:
```shell
rspamc learn_spam {{path/to/email_file}}
```
#### Train the bayesian filter to recognise an email as ham:
```shell
rspamc learn_ham {{path/to/email_file}}
```
#### Generate a manual report on an email:
```shell
rspamc symbols {{path/to/email_file}}
```
#### Show server statistics:
```shell
rspamc stat
```
{% endraw %}{% raw %}
<h2 id="rtcwake">
  <a href="/en/linux/rtcwake.html">rtcwake</a> <a href="#rtcwake"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Enter a system sleep state until specified wakeup time relative to your bios clock.

#### Show whether an alarm is set or not:
```shell
sudo rtcwake -m show -v
```
#### Suspend to ram and wakeup after 10 seconds:
```shell
sudo rtcwake -m mem -s {{10}}
```
#### Suspend to disk (higher power saving) and wakeup 15 minutes later:
```shell
sudo rtcwake -m disk --date +{{15}}min
```
#### Freeze the system (more efficient than suspend-to-ram but linux > 3.9 required) and wakeup at a given date and time:
```shell
sudo rtcwake -m freeze --date {{YYYYMMDDhhmm}}
```
#### Disable a previously set alarm:
```shell
sudo rtcwake -m disable
```
#### Perform a dry run to wakeup the computer at a given time. (Press Ctrl + C to abort):
```shell
sudo rtcwake -m on --date {{hh:ss}}
```
{% endraw %}{% raw %}
<h2 id="rtorrent">
  <a href="/en/linux/rtorrent.html">rtorrent</a> <a href="#rtorrent"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Download torrents over the command-line.

#### Add a torrent file or magnet to be downloaded:
```shell
rtorrent {{torrent_or_magnet}}
```
#### Start the download:
```shell
<Ctrl>S
```
#### View details about downloading torrent:
```shell
->
```
#### Close rtorrent safely:
```shell
<Ctrl>Q
```
{% endraw %}{% raw %}
<h2 id="run-mailcap">
  <a href="/en/linux/run-mailcap.html">run-mailcap</a> <a href="#run-mailcap"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run MailCap Programs.
> Run mailcap view, see, edit, compose, print - execute programs via entries in the mailcap file (or any of its aliases) will use the given action to process each mime-type/file.

#### Individual actions/programs on run-mailcap can be invoked with action flag:
```shell
run-mailcap --action=ACTION [--option[=value]]
```
#### In simple language:
```shell
run-mailcap --action=ACTION {{filename}}
```
#### Turn on extra information:
```shell
run-mailcap --action=ACTION --debug {{filename}}
```
#### Ignore any "copiousoutput" directive and forward output to standard output:
```shell
run-mailcap --action=ACTION --nopager {{filename}}
```
#### Display the found command without actually executing it:
```shell
run-mailcap --action=ACTION --norun {{filename}}
```
{% endraw %}{% raw %}
<h2 id="runcon">
  <a href="/en/linux/runcon.html">runcon</a> <a href="#runcon"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run a program in a different SELinux security context.
> With neither context nor command, print the current security context.
> More information: <https://www.gnu.org/software/coreutils/runcon>.

#### Determine the current domain:
```shell
runcon
```
#### Specify the domain to run a command in:
```shell
runcon -t {{domain}}_t {{command}}
```
#### Specify the context role to run a command with:
```shell
runcon -r {{role}}_r {{command}}
```
#### Specify the full context to run a command with:
```shell
runcon {{user}}_u:{{role}}_r:{{domain}}_t {{command}}
```
{% endraw %}{% raw %}
<h2 id="runuser">
  <a href="/en/linux/runuser.html">runuser</a> <a href="#runuser"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run commands as a specific user and group without asking for password (needs root privileges).

#### Run command as a different user:
```shell
runuser {{user}} -c '{{command}}'
```
#### Run command as a different user and group:
```shell
runuser {{user}} -g {{group}} -c '{{command}}'
```
#### Start a login shell as a specific user:
```shell
runuser {{user}} -l
```
#### Specify a shell for running instead of the default shell (also works for login):
```shell
runuser {{user}} -s {{/bin/sh}}
```
#### Preserve the entire environment of root (only if `--login` is not specified):
```shell
runuser {{user}} --preserve-environment -c '{{command}}'
```
{% endraw %}{% raw %}
<h2 id="rusnapshot">
  <a href="/en/linux/rusnapshot.html">rusnapshot</a> <a href="#rusnapshot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> BTRFS snapshotting utility written in Rust.
> More information: <https://github.com/Edu4rdSHL/rusnapshot>.

#### Create a snapshot using a config file:
```shell
sudo rusnapshot --config {{path/to/config.toml}} --cr
```
#### List created snapshots:
```shell
sudo rusnapshot -c {{path/to/config.toml}} --list
```
#### Delete a snapshot by ID or the name of the snapshot:
```shell
sudo rusnapshot -c {{path/to/config.toml}} --del --id {{snapshot_id}}
```
#### Delete all `hourly` snapshots:
```shell
sudo rusnapshot -c {{path/to/config.toml}} --list --keep {{0}} --clean --kind {{hourly}}
```
#### Create a read-write snapshot:
```shell
sudo rusnapshot -c {{path/to/config.toml}} --cr --rw
```
#### Restore a snapshot:
```shell
sudo rusnapshot -c {{path/to/config.toml}} --id {{snapshot_id}} --restore
```
{% endraw %}{% raw %}
<h2 id="sa">
  <a href="/en/linux/sa.html">sa</a> <a href="#sa"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Summarizes accounting information. Part of the acct package.
> Shows commands called by users, including basic info on CPU time spent processing and I/O rates.

#### Display executable invocations per user (username not displayed):
```shell
sudo sa
```
#### Display executable invocations per user, showing responsible usernames:
```shell
sudo sa --print-users
```
#### List resources used recently per user:
```shell
sudo sa --user-summary
```
{% endraw %}{% raw %}
<h2 id="sacct">
  <a href="/en/linux/sacct.html">sacct</a> <a href="#sacct"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display accounting data from the Slurm service.
> More information: <https://slurm.schedmd.com/sacct.html>.

#### Display job id, job name, partition, account, number of allocated cpus, job state, and job exit codes for recent jobs:
```shell
sacct
```
#### Display job id, job state, job exit code for recent jobs:
```shell
sacct --brief
```
#### Display the allocations of a job:
```shell
sacct --jobs {{job_id}} --allocations
```
#### Display elapsed time, job name, number of requested CPUs, and memory requested of a job:
```shell
sacct --jobs {{job_id}} --format={{elapsed}},{{jobname}},{{reqcpus}},{{reqmem}}
```
{% endraw %}{% raw %}
<h2 id="sacctmgr">
  <a href="/en/linux/sacctmgr.html">sacctmgr</a> <a href="#sacctmgr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> View, setup, and manage Slurm accounts.
> More information: <https://slurm.schedmd.com/sacctmgr.html>.

#### Show current configuration:
```shell
sacctmgr show configuration
```
#### Add a cluster to the slurm database:
```shell
sacctmgr add cluster {{cluster_name}}
```
#### Add an account to the slurm database:
```shell
sacctmgr add account {{account_name}} cluster={{cluster_of_account}}
```
#### Show details of user/association/cluster/account:
```shell
sacctmgr show {{user/association/cluster/account}}
```
{% endraw %}{% raw %}
<h2 id="sam">
  <a href="/en/linux/sam.html">sam</a> <a href="#sam"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> AWS Serverless Application Model (SAM) CLI.
> More information: <https://github.com/awslabs/aws-sam-cli>.

#### Initialize a serverless application:
```shell
sam init
```
#### Initialize a serverless application with a specific runtime:
```shell
sam init --runtime {{python3.7}}
```
#### Package a SAM application:
```shell
sam package
```
#### Build your Lambda function code:
```shell
sam build
```
#### Run your serverless application locally:
```shell
sam local start-api
```
#### Deploy an AWS SAM application:
```shell
sam deploy
```
{% endraw %}{% raw %}
<h2 id="sar">
  <a href="/en/linux/sar.html">sar</a> <a href="#sar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Monitor performance of various Linux subsystems.

#### Report I/O and transfer rate issued to physical devices, one per second (press CTRL+C to quit):
```shell
sar -b {{1}}
```
#### Report a total of 10 network device statistics, one per 2 seconds:
```shell
sar -n DEV {{2}} {{10}}
```
#### Report CPU utilization, one per 2 seconds:
```shell
sar -u ALL {{2}}
```
#### Report a total of 20 memory utilization statistics, one per second:
```shell
sar -r ALL {{1}} {{20}}
```
#### Report the run queue length and load averages, one per second:
```shell
sar -q {{1}}
```
#### Report paging statistics, one per 5 seconds:
```shell
sar -B {{5}}
```
{% endraw %}{% raw %}
<h2 id="sbatch">
  <a href="/en/linux/sbatch.html">sbatch</a> <a href="#sbatch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Submit a batch job to the SLURM scheduler.

#### Submit a batch job:
```shell
sbatch {{path/to/job.sh}}
```
#### Submit a batch job with a custom name:
```shell
sbatch --job-name={{myjob}} {{path/to/job.sh}}
```
#### Submit a batch job with a time limit of 30 minutes:
```shell
sbatch --time={{00:30:00}} {{path/to/job.sh}}
```
#### Submit a job and request multiple nodes:
```shell
sbatch --nodes={{3}} {{path/to/job.sh}}
```
{% endraw %}{% raw %}
<h2 id="scancel">
  <a href="/en/linux/scancel.html">scancel</a> <a href="#scancel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cancel a Slurm job.
> More information: <https://slurm.schedmd.com/scancel.html>.

#### Cancel a job using its ID:
```shell
scancel {{job_id}}
```
#### Cancel all jobs from a user:
```shell
scancel {{user_name}}
```
{% endraw %}{% raw %}
<h2 id="scanimage">
  <a href="/en/linux/scanimage.html">scanimage</a> <a href="#scanimage"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Scan images with the Scanner Access Now Easy API.
> More information: <http://sane-project.org/man/scanimage.1.html>.

#### List available scanners to ensure the target device is connected and recognized:
```shell
scanimage -L
```
#### Scan an image and save it to a file:
```shell
scanimage --format={{pnm|tiff|png|jpeg}} > {{path/to/new_image}}
```
{% endraw %}{% raw %}
<h2 id="schroot">
  <a href="/en/linux/schroot.html">schroot</a> <a href="#schroot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run command or start an interactive shell with a different root directory. More customizable than `chroot`.
> More information: <https://wiki.debian.org/Schroot>.

#### Run a command in a specific chroot:
```shell
schroot --chroot {{chroot}} {{command}}
```
#### Run a command with options in a specific chroot:
```shell
schroot --chroot {{chroot}} {{command}} -- {{command_options}}
```
#### Run a command in all available chroots:
```shell
schroot --all {{command}}
```
#### Start an interactive shell with in a specific chroot as a specific user:
```shell
schroot --chroot {{chroot}} --user {{user}}
```
#### List available chroots:
```shell
schroot --list
```
{% endraw %}{% raw %}
<h2 id="scontrol">
  <a href="/en/linux/scontrol.html">scontrol</a> <a href="#scontrol"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> View information about and modify jobs.
> More information: <https://slurm.schedmd.com/scontrol.html>.

#### Show information for job:
```shell
scontrol show job {{job_id}}
```
#### Suspend a comma-separated list of running jobs:
```shell
scontrol suspend {{job_id}}
```
#### Resume a comma-separated list of suspended jobs:
```shell
scontrol resume {{job_id}}
```
#### Hold a comma-separated list of queued jobs (Use `release` command to permit the jobs to be scheduled):
```shell
scontrol hold {{job_id}}
```
#### Release a comma-separated list of suspended job:
```shell
scontrol release {{job_id}}
```
{% endraw %}{% raw %}
<h2 id="screenkey">
  <a href="/en/linux/screenkey.html">screenkey</a> <a href="#screenkey"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A screencast tool to display keys pressed.
> More information: <https://www.thregr.org/~wavexx/software/screenkey/>.

#### Display keys which are currently being pressed on the screen:
```shell
screenkey
```
#### Display keys and mouse buttons which are currently being pressed on the screen:
```shell
screenkey --mouse
```
#### Launch the settings menu of screenkey:
```shell
screenkey --show-settings
```
#### Launch screenkey at a specific position:
```shell
screenkey --position {{top|center|bottom|fixed}}
```
#### Change the format of the key modifiers displayed on screen:
```shell
screenkey --mods-mode {{normal|emacs|mac|win|tux}}
```
#### Change the appearance of screenkey:
```shell
screenkey --bg-color "{{#a1b2c3}}" --font {{Hack}} --font-color {{yellow}} --opacity {{0.8}}
```
#### Drag and select a window on screen to display screenkey:
```shell
screenkey --position fixed --geometry {{$(slop -n -f '%g')}}
```
{% endraw %}{% raw %}
<h2 id="script">
  <a href="/en/linux/script.html">script</a> <a href="#script"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Record all terminal output to file.

#### Record a new session to a file named `typescript` in the current directory:
```shell
script
```
#### Record a new session to a custom filepath:
```shell
script {{path/to/session.out}}
```
#### Record a new session, appending to an existing file:
```shell
script -a {{path/to/session.out}}
```
#### Record timing information (data is outputted to the standard error):
```shell
script -t 2> {{path/to/timingfile}}
```
{% endraw %}{% raw %}
<h2 id="scriptreplay">
  <a href="/en/linux/scriptreplay.html">scriptreplay</a> <a href="#scriptreplay"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Replay a typescript created by the `script` command to the standard output.

#### Replay a typescript at the speed it was recorded:
```shell
scriptreplay {{path/to/timing_file}} {{path/to/typescript}}
```
#### Replay a typescript at double the original speed:
```shell
scriptreplay {{path/to/timingfile}} {{path/to/typescript}} 2
```
#### Replay a typescript at half the original speed:
```shell
scriptreplay {{path/to/timingfile}} {{path/to/typescript}} 0.5
```
{% endraw %}{% raw %}
<h2 id="scrot">
  <a href="/en/linux/scrot.html">scrot</a> <a href="#scrot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Screen capture utility.
> More information: <https://github.com/resurrecting-open-source-projects/scrot>.

#### Capture a screenshot and save it to the current directory with the current date as the filename:
```shell
scrot
```
#### Capture a screenshot and save it as `capture.png`:
```shell
scrot {{capture.png}}
```
#### Capture a screenshot interactively:
```shell
scrot --select
```
#### Capture a screenshot from the currently focused window:
```shell
scrot --focused
```
#### Display a countdown of 10 seconds before taking a screenshot:
```shell
scrot --count --delay {{10}}
```
{% endraw %}{% raw %}
<h2 id="see">
  <a href="/en/linux/see.html">see</a> <a href="#see"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Alias to `run-mailcap`'s view.
> An alias to a `run-mailcap`'s action print.

#### See action can be used to view any file (usually image) on default mailcap explorer:
```shell
see {{filename}}
```
#### Using with `run-mailcap`:
```shell
run-mailcap --action=view {{filename}}
```
{% endraw %}{% raw %}
<h2 id="semanage">
  <a href="/en/linux/semanage.html">semanage</a> <a href="#semanage"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> SELinux Policy Management tool.
> More information: <https://manned.org/semanage>.

#### Output local customizations:
```shell
semanage -S {{store}} -o {{path/to/output_file}}
```
#### Take a set of commands from a specified file and load them in a single transaction:
```shell
semanage -S {{store}} -i {{path/to/input_file}}
```
#### Manage booleans. Booleans allow the administrator to modify the confinement of processes based on the current configuration:
```shell
semanage boolean -S {{store}} {{--delete|--modify|--list|--noheading|--deleteall}} {{-on|-off}} -F {{boolean|boolean_file}}
```
#### Manage policy modules:
```shell
semanage module -S {{store}} {{--add|--delete|--list|--modify}} {{--enable|--disable}} {{module_name}}
```
#### Disable/Enable dontaudit rules in policy:
```shell
semanage dontaudit -S {{store}} {{on|off}}
```
{% endraw %}{% raw %}
<h2 id="sensible-browser">
  <a href="/en/linux/sensible-browser.html">sensible-browser</a> <a href="#sensible-browser"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Open the default browser.

#### Open a new window of the default browser:
```shell
sensible-browser
```
#### Open a URL in the default browser:
```shell
sensible-browser {{url}}
```
{% endraw %}{% raw %}
<h2 id="sensible-editor">
  <a href="/en/linux/sensible-editor.html">sensible-editor</a> <a href="#sensible-editor"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Open the default editor.

#### Open a file in the default editor:
```shell
sensible-editor {{file}}
```
#### Open a file in the default editor, with the cursor at the end of the file:
```shell
sensible-editor + {{file}}
```
#### Open a file in the default editor, with the cursor at the beginning of line 10:
```shell
sensible-editor +10 {{file}}
```
#### Open 3 files in vertically split editor windows at the same time:
```shell
sensible-editor -O3 {{file_1}} {{file_2}} {{file_3}}
```
{% endraw %}{% raw %}
<h2 id="sensors">
  <a href="/en/linux/sensors.html">sensors</a> <a href="#sensors"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Report sensors information.

#### Show the current readings of all sensor chips:
```shell
sensors
```
#### Show temperatures in degrees Fahrenheit:
```shell
sensors --fahrenheit
```
{% endraw %}{% raw %}
<h2 id="service">
  <a href="/en/linux/service.html">service</a> <a href="#service"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage services by running init scripts.
> The full script path should be omitted (`/etc/init.d/` is assumed).

#### List the name and status of all services:
```shell
service --status-all
```
#### Start/Stop/Restart/Reload service (start/stop should always be available):
```shell
service {{service_name}} {{start|stop|restart|reload}}
```
#### Do a full restart (runs script twice with start and stop):
```shell
service {{service_name}} --full-restart
```
#### Show the current status of a service:
```shell
service {{service_name}} status
```
{% endraw %}{% raw %}
<h2 id="setfacl">
  <a href="/en/linux/setfacl.html">setfacl</a> <a href="#setfacl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Set file access control lists (ACL).

#### Modify ACL of a file for user with read and write access:
```shell
setfacl -m u:{{username}}:rw {{file}}
```
#### Modify default ACL of a file for all users:
```shell
setfacl -d -m u::rw {{file}}
```
#### Remove ACL of a file for an user:
```shell
setfacl -x u:{{username}} {{file}}
```
#### Remove all ACL entries of a file:
```shell
setfacl -b {{file}}
```
{% endraw %}{% raw %}
<h2 id="setxkbmap">
  <a href="/en/linux/setxkbmap.html">setxkbmap</a> <a href="#setxkbmap"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Set the keyboard using the X Keyboard Extension.

#### Set the keyboard in French AZERTY:
```shell
setxkbmap {{fr}}
```
#### Set multiple keyboard layouts, their variants and switching option:
```shell
setxkbmap -layout {{us,de}} -variant {{,qwerty}} -option {{'grp:alt_caps_toggle'}}
```
#### Get help:
```shell
setxkbmap -help
```
#### List all layouts:
```shell
localectl list-x11-keymap-layouts
```
#### List variants for the layout:
```shell
localectl list-x11-keymap-variants {{de}}
```
#### List available switching options:
```shell
localectl list-x11-keymap-options | grep grp:
```
{% endraw %}{% raw %}
<h2 id="sfill">
  <a href="/en/linux/sfill.html">sfill</a> <a href="#sfill"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Securely overwrite the free space and inodes of the partition where the specified directory resides.
> More information: <https://manned.org/sfill>.

#### Overwrite free space and inodes of a disk with 38 writes (slow but secure):
```shell
sfill {{/path/to/mounted_disk_directory}}
```
#### Overwrite free space and inodes of a disk with 6 writes (fast but less secure) and show status:
```shell
sfill -l -v {{/path/to/mounted_disk_directory}}
```
#### Overwrite free space and inodes of a disk with 1 write (very fast but insecure) and show status:
```shell
sfill -ll -v {{/path/to/mounted_disk_directory}}
```
#### Overwrite only free space of a disk:
```shell
sfill -I {{/path/to/mounted_disk_directory}}
```
#### Overwrite only free inodes of a disk:
```shell
sfill -i {{/path/to/mounted_disk_directory}}
```
{% endraw %}{% raw %}
<h2 id="shutdown">
  <a href="/en/linux/shutdown.html">shutdown</a> <a href="#shutdown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Shutdown and reboot the system.

#### Power off (halt) immediately:
```shell
shutdown -h now
```
#### Reboot immediately:
```shell
shutdown -r now
```
#### Reboot in 5 minutes:
```shell
shutdown -r +{{5}} &
```
#### Shutdown at 1:00 pm (Uses 24h clock):
```shell
shutdown -h 13:00
```
#### Cancel a pending shutdown/reboot operation:
```shell
shutdown -c
```
{% endraw %}{% raw %}
<h2 id="sic">
  <a href="/en/linux/sic.html">sic</a> <a href="#sic"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Simple IRC client.
> Part of the suckless tools.
> More information: <https://tools.suckless.org/sic/>.

#### Connect to the default host (irc.ofct.net) with the nickname set in the `$USER` environment variable:
```shell
sic
```
#### Connect to a given host, using a given nickname:
```shell
sic -h {{host}} -n {{nickname}}
```
#### Connect to a given host, using a given nickname and password:
```shell
sic -h {{host}} -n {{nickname}} -k {{password}}
```
#### Join a channel:
```shell
:j #{{channel}}<Enter>
```
#### Send a message to a channel or user:
```shell
:m #{{channel|user}}<Enter>
```
#### Set default channel or user:
```shell
:s #{{channel|user}}<Enter>
```
{% endraw %}{% raw %}
<h2 id="silentcast">
  <a href="/en/linux/silentcast.html">silentcast</a> <a href="#silentcast"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Silent screencast creator. Saves in `.mkv` and animated gif formats.
> More information: <https://github.com/colinkeenan/silentcast>.

#### Launch silentcast:
```shell
silentcast
```
#### Launch silentcast on a specific display:
```shell
silentcast --display={{display}}
```
{% endraw %}{% raw %}
<h2 id="sinfo">
  <a href="/en/linux/sinfo.html">sinfo</a> <a href="#sinfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> View information about Slurm nodes and partitions.
> See also `squeue` and `sbatch`, which are also part of the Slurm workload manager.
> More information: <https://slurm.schedmd.com/sinfo.html>.

#### Show a quick summary overview of the cluster:
```shell
sinfo --summarize
```
#### View the detailed status of all partitions across the entire cluster:
```shell
sinfo
```
#### View the detailed status of a specific partition:
```shell
sinfo --partition {{partition_name}}
```
#### View information about idle nodes:
```shell
sinfo --states {{idle}}
```
#### Summarise dead nodes:
```shell
sinfo --dead
```
#### List dead nodes and the reasons why:
```shell
sinfo --list-reasons
```
{% endraw %}{% raw %}
<h2 id="slapt-get">
  <a href="/en/linux/slapt-get.html">slapt-get</a> <a href="#slapt-get"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> An apt like system for Slackware package management.
> Package sources need to be configured in the slapt-getrc file.

#### Update the list of available packages and versions:
```shell
slapt-get --update
```
#### Install a package, or update it to the latest available version:
```shell
slapt-get --install {{package_name}}
```
#### Remove a package:
```shell
slapt-get --remove {{package_name}}
```
#### Upgrade all installed packages to their latest available versions:
```shell
slapt-get --upgrade
```
#### Locate packages of interest by the package name, disk set, or version:
```shell
slapt-get --search {{package_name}}
```
#### Show information about a package:
```shell
slapt-get --show {{package_name}}
```
{% endraw %}{% raw %}
<h2 id="slapt-src">
  <a href="/en/linux/slapt-src.html">slapt-src</a> <a href="#slapt-src"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A utility to automate building of slackbuilds.
> SlackBuild sources need to be configured in the slapt-srcrc file.
> More information: <https://github.com/jaos/slapt-src>.

#### Update the list of available slackbuilds and versions:
```shell
slapt-src --update
```
#### List all available slackbuilds:
```shell
slapt-src --list
```
#### Fetch, build and install the specified slackbuild(s):
```shell
slapt-src --install {{slackbuild_name}}
```
#### Locate slackbuilds of interest by their name or description:
```shell
slapt-src --search {{search_term}}
```
#### Display information about a slackbuild:
```shell
slapt-src --show {{slackbuild_name}}
```
{% endraw %}{% raw %}
<h2 id="slop">
  <a href="/en/linux/slop.html">slop</a> <a href="#slop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Get a selection of the screen.
> More information: <https://github.com/naelstrof/slop>.

#### Wait for the user to make a selection and output its geometry to standard output:
```shell
slop
```
#### Double click, rather than click and drag, to draw a selection:
```shell
slop -D
```
#### Highlight the selection rather than outlining it:
```shell
slop -l
```
#### Specify the output format:
```shell
slop -f {{format_string}}
```
#### Specify the selection rectangle's color:
```shell
slop -c {{red}},{{green}},{{blue}},{{alpha}}
```
{% endraw %}{% raw %}
<h2 id="sm">
  <a href="/en/linux/sm.html">sm</a> <a href="#sm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Displays a short message fullscreen.
> More information: <https://github.com/nomeata/screen-message>.

#### Display a message in full-screen:
```shell
sm "{{Hello World!}}"
```
#### Display a message with inverted colors:
```shell
sm -i "{{Hello World!}}"
```
#### Display a message with a custom foreground color:
```shell
sm -f {{blue}} "{{Hello World!}}"
```
#### Display a message with a custom background color:
```shell
sm -b {{#008888}} "{{Hello World!}}"
```
#### Display a message rotated 3 times (in steps of 90 degrees, counterclockwise):
```shell
sm -r {{3}} "{{Hello World!}}"
```
#### Display a message using the output from another command:
```shell
{{echo "Hello World!"}} | sm -
```
{% endraw %}{% raw %}
<h2 id="smbclient">
  <a href="/en/linux/smbclient.html">smbclient</a> <a href="#smbclient"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> FTP-like client to access SMB/CIFS resources on servers.

#### Connect to a share (user will be prompted for password; `exit` to quit the session):
```shell
smbclient {{//server/share}}
```
#### Connect with a different username:
```shell
smbclient {{//server/share}} --user {{username}}
```
#### Connect with a different workgroup:
```shell
smbclient {{//server/share}} --workgroup {{domain}} --user {{username}}
```
#### Connect with a username and password:
```shell
smbclient {{//server/share}} --user {{username%password}}
```
#### Download a file from the server:
```shell
smbclient {{//server/share}} --directory {{path/to/directory}} --command "get {{file.txt}}"
```
#### Upload a file to the server:
```shell
smbclient {{//server/share}} --directory {{path/to/directory}} --command "put {{file.txt}}"
```
{% endraw %}{% raw %}
<h2 id="smbget">
  <a href="/en/linux/smbget.html">smbget</a> <a href="#smbget"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> `wget`-like utility for downloading files from SMB servers.
> More information: <https://www.samba.org/samba/docs/current/man-html/smbget.1.html>.

#### Download a file from a server:
```shell
smbget {{smb://server/share/file}}
```
#### Download a share or directory recursively:
```shell
smbget --recursive {{smb://server/share}}
```
#### Connect with a username and password:
```shell
smbget {{smb://server/share/file}} --user {{username%password}}
```
#### Require encrypted transfers:
```shell
smbget {{smb://server/share/file}} --encrypt
```
{% endraw %}{% raw %}
<h2 id="smbmap">
  <a href="/en/linux/smbmap.html">smbmap</a> <a href="#smbmap"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> SMB enumeration tool.
> More information: <https://github.com/ShawnDEvans/smbmap>.

#### Display SMB shares and permissions on a host, prompting for user's password or NTLM hash:
```shell
smbmap -u {{username}} --prompt -H {{ip}}
```
#### Display SMB shares and permissions on a host, specifying the domain and passing the password NTLM hash:
```shell
smbmap -u {{username}} --prompt -d {{domain}} -H {{ip}}
```
#### Display SMB shares and list a single level of directories and files:
```shell
smbmap -u {{username}} --prompt -H {{ip}} -r
```
#### Display SMB shares and recursively list a defined number of levels of directories and files:
```shell
smbmap -u {{username}} --prompt -H {{ip}} -R --depth {{3}}
```
#### Display SMB shares and recursively list directories and files, downloading the files matching a regular expression:
```shell
smbmap -u {{username}} --prompt -H {{ip}} -R -A {{pattern}}
```
#### Display SMB shares and recursively list directories and files, searching for file content matching a regular expression:
```shell
smbmap -u {{username}} --prompt -H {{ip}} -R -F {{pattern}}
```
#### Execute a shell command on a remote system:
```shell
smbmap -u {{username}} --prompt -H {{ip}} -x {{command}}
```
#### Upload a file to a remote system:
```shell
smbmap -u {{username}} --prompt -H {{ip}} --upload {{source}} {{destination}}
```
{% endraw %}{% raw %}
<h2 id="smbpasswd">
  <a href="/en/linux/smbpasswd.html">smbpasswd</a> <a href="#smbpasswd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Change a user's SMB password.
> Samba users must also have a local Unix account.

#### Change the current user's SMB password:
```shell
smbpasswd
```
#### Add a specified user to Samba and set password(user should already exist in system):
```shell
smbpasswd -a {{username}}
```
#### Modify an existing Samba user's password:
```shell
smbpasswd {{username}}
```
#### Delete a Samba user:
```shell
smbpasswd -x {{username}}
```
{% endraw %}{% raw %}
<h2 id="snake4">
  <a href="/en/linux/snake4.html">snake4</a> <a href="#snake4"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Snake game in the terminal.
> More information: <https://manpages.debian.org/snake4/snake4.6.en.html>.

#### Start a snake game:
```shell
snake4
```
#### Choose level:
```shell
{{1|2|3|4|5}}
```
#### Navigate the snake:
```shell
{{Up|Down|Left|Right}} arrow key
```
#### Pause game:
```shell
Spacebar
```
#### Quit game:
```shell
q
```
#### Show the high scores:
```shell
snake4 --highscores
```
{% endraw %}{% raw %}
<h2 id="snake4scores">
  <a href="/en/linux/snake4scores.html">snake4scores</a> <a href="#snake4scores"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show the high scores from the snake4 game.
> More information: <https://manpages.debian.org/snake4/snake4.6.en.html>.

#### Show the highscores:
```shell
snake4scores
```
{% endraw %}{% raw %}
<h2 id="snap">
  <a href="/en/linux/snap.html">snap</a> <a href="#snap"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool for managing the "snap" self-contained software packages.
> Similar to what `apt` is for ".deb".

#### Search for a package:
```shell
snap find {{package_name}}
```
#### Install a package:
```shell
snap install {{package_name}}
```
#### Update a package:
```shell
snap refresh {{package_name}}
```
#### Update a package to another channel (track, risk, or branch):
```shell
snap refresh {{package_name}} --channel={{channel}}
```
#### Update all packages:
```shell
snap refresh
```
#### Display basic information about installed snap software:
```shell
snap list
```
#### Uninstall a package:
```shell
snap remove {{package_name}}
```
#### Check for recent snap changes in the system:
```shell
snap changes
```
{% endraw %}{% raw %}
<h2 id="snapper">
  <a href="/en/linux/snapper.html">snapper</a> <a href="#snapper"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Filesystem snapshot management tool.
> More information: <http://snapper.io/manpages/snapper.html>.

#### List snapshot configs:
```shell
snapper list-configs
```
#### Create snapper config:
```shell
snapper -c {{config}} create-config {{path/to/directory}}
```
#### Create a snapshot with a description:
```shell
snapper -c {{config}} create -d "{{snapshot_description}}"
```
#### List snapshots for a config:
```shell
snapper -c {{config}} list
```
#### Delete a snapshot:
```shell
snapper -c {{config}} delete {{snapshot_number}}
```
#### Delete a range of snapshots:
```shell
snapper -c {{config}} delete {{snapshot_X}}-{{snapshot_Y}}
```
{% endraw %}{% raw %}
<h2 id="snmpwalk">
  <a href="/en/linux/snmpwalk.html">snmpwalk</a> <a href="#snmpwalk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> SNMP query tool.
> More information: <https://manned.org/snmpwalk>.

#### Query the system information of a remote host using SNMPv1 and a community string:
```shell
snmpwalk -v1 -c {{community}} {{ip}}
```
#### Query specific system information on a remote host by OID using SNMPv2 on a specified port:
```shell
snmpwalk -v2c -c {{community}} {{ip}}:{{port}} {{oid}}
```
#### Query specific system information on a remote host by OID using SNMPv3 and authentication without encryption:
```shell
snmpwalk -v3 -l {{authNoPriv}} -u {{username}} -a {{MD5|SHA}} -A {{passphrase}} {{ip}} {{oid}}
```
#### Query specific system information on a remote host by OID using SNMPv3, authentication, and encryption:
```shell
snmpwalk -v3 -l {{authPriv}} -u {{username}} -a {{MD5|SHA}} -A {{auth_passphrase}} -x {{DES|AES}} -X {{enc_passphrase}} {{ip}} {{oid}}
```
#### Query specific system information on a remote host by OID using SNMPv3 without authentication or encryption:
```shell
snmpwalk -v3 -l {{noAuthNoPriv}} -u {{username}} {{ip}} {{oid}}
```
{% endraw %}{% raw %}
<h2 id="spectre-meltdown-checker">
  <a href="/en/linux/spectre-meltdown-checker.html">spectre-meltdown-checker</a> <a href="#spectre-meltdown-checker"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Spectre and Meltdown mitigation detection tool.
> More information: <https://manned.org/spectre-meltdown-checker.1>.

#### Check the currently running kernel for Spectre or Meltdown:
```shell
sudo spectre-meltdown-checker
```
#### Check the currently running kernel and show an explanation of the actions to take in order to mitigate a vulnerability:
```shell
sudo spectre-meltdown-checker --explain
```
#### Check for specific variants (defaults to all):
```shell
sudo spectre-meltdown-checker --variant {{1|2|3|3a|4|l1tf|msbds|mfbds|mlpds|mdsum|taa|mcespc|srbds}}
```
#### Display output using a specific output format:
```shell
sudo spectre-meltdown-checker --batch {{text|json|nrpe|prometheus|short}}
```
#### Don't use the `/sys` interface even if present:
```shell
sudo spectre-meltdown-checker --no-sysfs
```
#### Check a non-running kernel:
```shell
sudo spectre-meltdown-checker --kernel {{path/to/kernel_file}}
```
{% endraw %}{% raw %}
<h2 id="speedometer">
  <a href="/en/linux/speedometer.html">speedometer</a> <a href="#speedometer"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Python script that shows a network traffic graph in the terminal.
> More information: <http://excess.org/speedometer>.

#### Show graph for a specific interface:
```shell
speedometer -r {{eth0}} -t {{eth0}}
```
{% endraw %}{% raw %}
<h2 id="spi">
  <a href="/en/linux/spi.html">spi</a> <a href="#spi"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A meta package manager that handles both packages and slackbuilds.
> More information: <https://github.com/gapan/spi>.

#### Update the list of available packages and slackbuilds:
```shell
spi --update
```
#### Install a package or slackbuild:
```shell
spi --install {{package/slackbuild_name}}
```
#### Upgrade all installed packages to the latest versions available:
```shell
spi --upgrade
```
#### Locate packages or slackbuilds of interest by package name or description:
```shell
spi {{search_terms}}
```
#### Display information about a package or slackbuild:
```shell
spi --show {{package/slackbuild_name}}
```
#### Purge the local package and slackbuild caches:
```shell
spi --clean
```
{% endraw %}{% raw %}
<h2 id="squeue">
  <a href="/en/linux/squeue.html">squeue</a> <a href="#squeue"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> View the jobs queued in the SLURM scheduler.

#### View the queue:
```shell
squeue
```
#### View jobs queued by a specific user:
```shell
squeue -u {{username}}
```
#### View the queue and refresh every 5 seconds:
```shell
squeue -i {{5}}
```
#### View the queue with expected start times:
```shell
squeue --start
```
{% endraw %}{% raw %}
<h2 id="sreport">
  <a href="/en/linux/sreport.html">sreport</a> <a href="#sreport"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate reports on jobs, users, and clusters from accounting data.
> More information: <https://slurm.schedmd.com/sreport.html>.

#### Show pipe delimited cluster utilization data:
```shell
sreport --parsable cluster utilization
```
#### Show number of jobs run:
```shell
sreport job sizes printjobcount
```
#### Show users with highest cpu time use:
```shell
sreport user topuser
```
{% endraw %}{% raw %}
<h2 id="srun">
  <a href="/en/linux/srun.html">srun</a> <a href="#srun"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create an interactive slurm job or connect to an existing job.
> More information: <https://slurm.schedmd.com/srun.html>.

#### Submit a basic interactive job:
```shell
srun --pty /bin/bash
```
#### Submit an interactive job with different attributes:
```shell
srun --ntasks-per-node={{num_cores}} --mem-per-cpu={{memory_MB}} --pty /bin/bash
```
#### Connect to a worker node with a job running:
```shell
srun --jobid={{job_id}} --pty /bin/bash
```
{% endraw %}{% raw %}
<h2 id="ss">
  <a href="/en/linux/ss.html">ss</a> <a href="#ss"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility to investigate sockets.
> More information: <https://manned.org/ss.8>.

#### Show all TCP/UDP/RAW/UNIX sockets:
```shell
ss -a {{-t|-u|-w|-x}}
```
#### Filter TCP sockets by states, only/exclude:
```shell
ss {{state/exclude}} {{bucket/big/connected/synchronized/...}}
```
#### Show all TCP sockets connected to the local HTTPS port (443):
```shell
ss -t src :{{443}}
```
#### Show all TCP sockets listening on the local 8080 port:
```shell
ss -lt src :{{8080}}
```
#### Show all TCP sockets along with processes connected to a remote ssh port:
```shell
ss -pt dst :{{ssh}}
```
#### Show all UDP sockets connected on specific source and destination ports:
```shell
ss -u 'sport == :{{source_port}} and dport == :{{destination_port}}'
```
#### Show all TCP IPv4 sockets locally connected on the subnet 192.168.0.0/16:
```shell
ss -4t src {{192.168/16}}
```
{% endraw %}{% raw %}
<h2 id="ssh-add">
  <a href="/en/linux/ssh-add.html">ssh-add</a> <a href="#ssh-add"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage loaded ssh keys in the ssh-agent.
> Ensure that ssh-agent is up and running for the keys to be loaded in it.

#### Add the default ssh keys in `~/.ssh` to the ssh-agent:
```shell
ssh-add
```
#### Add a specific key to the ssh-agent:
```shell
ssh-add {{path/to/private_key}}
```
#### List fingerprints of currently loaded keys:
```shell
ssh-add -l
```
#### Delete a key from the ssh-agent:
```shell
ssh-add -d {{path/to/private_key}}
```
#### Delete all currently loaded keys from the ssh-agent:
```shell
ssh-add -D
```
{% endraw %}{% raw %}
<h2 id="sshuttle">
  <a href="/en/linux/sshuttle.html">sshuttle</a> <a href="#sshuttle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Transparent proxy server that tunnels traffic over an SSH connection.
> Doesn't require root or any special setup on the remote SSH server, though root access on the local machine is prompted for.

#### Forward all IPv4 TCP traffic via a remote SSH server:
```shell
sshuttle --remote={{username}}@{{sshserver}} {{0.0.0.0/0}}
```
#### Also forward all DNS traffic to the server's default DNS resolver:
```shell
sshuttle --dns --remote={{username}}@{{sshserver}} {{0.0.0.0/0}}
```
#### Forward all traffic except that which is bound for a specific subnet:
```shell
sshuttle --remote={{username}}@{{sshserver}} {{0.0.0.0/0}} --exclude {{192.168.0.1/24}}
```
#### Use the tproxy method to forward all IPv4 and IPv6 traffic:
```shell
sshuttle --method=tproxy --remote={{username}}@{{sshserver}} {{0.0.0.0/0}} {{::/0}} --exclude={{your_local_ip_address}} --exclude={{ssh_server_ip_address}}
```
{% endraw %}{% raw %}
<h2 id="sstat">
  <a href="/en/linux/sstat.html">sstat</a> <a href="#sstat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> View information about running jobs.
> More information: <https://slurm.schedmd.com/sstat.html>.

#### Display status information of a comma-separated list of jobs:
```shell
sstat --jobs={{job_id}}
```
#### Display job ID, average CPU and average virtual memory size of a comma-separated list of jobs, with pipes as column delimiters:
```shell
sstat --parsable --jobs={{job_id}} --format={{JobID}},{{AveCPU}},{{AveVMSize}}
```
#### Display list of fields available:
```shell
sstat --helpformat
```
{% endraw %}{% raw %}
<h2 id="steghide">
  <a href="/en/linux/steghide.html">steghide</a> <a href="#steghide"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Steganography tool for JPEG, BMP, WAV and AU file formats.
> More information: <https://github.com/StefanoDeVuono/steghide>.

#### Embed data in a PNG image, prompting for a passphrase:
```shell
steghide embed --coverfile {{path/to/image.png}} --embedfile {{path/to/data.txt}}
```
#### Extract data from a WAV audio file:
```shell
steghide extract --stegofile {{path/to/sound.wav}}
```
#### Display file information, trying to detect an embedded file:
```shell
steghide info {{path/to/file.jpg}}
```
#### Embed data in a JPEG image, using maximum compression:
```shell
steghide embed --coverfile {{path/to/image.jpg}} --embedfile {{path/to/data.txt}} --compress {{9}}
```
#### Get the list of supported encryption algorithms and modes:
```shell
steghide encinfo
```
#### Embed encrypted data in a JPEG image, e.g. with Blowfish in CBC mode:
```shell
steghide embed --coverfile {{path/to/image.jpg}} --embedfile {{path/to/data.txt}} --encryption {{blowfish|...}} {{cbc|...}}
```
{% endraw %}{% raw %}
<h2 id="strace">
  <a href="/en/linux/strace.html">strace</a> <a href="#strace"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Troubleshooting tool for tracing system calls.

#### Start tracing a specific process by its PID:
```shell
strace -p {{pid}}
```
#### Trace a process and filter output by system call:
```shell
strace -p {{pid}} -e {{system_call_name}}
```
#### Count time, calls, and errors for each system call and report a summary on program exit:
```shell
strace -p {{pid}} -c
```
#### Show the time spent in every system call:
```shell
strace -p {{pid}} -T
```
#### Start tracing a program by executing it:
```shell
strace {{program}}
```
#### Start tracing file operations of a program:
```shell
strace -e trace=file {{program}}
```
{% endraw %}{% raw %}
<h2 id="stress">
  <a href="/en/linux/stress.html">stress</a> <a href="#stress"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool to stress test CPU, memory, and IO on a Linux system.

#### Spawn 4 workers to stress test CPU:
```shell
stress -c {{4}}
```
#### Spawn 2 workers to stress test IO and timeout after 5 seconds:
```shell
stress -i {{2}} -t {{5}}
```
#### Spawn 2 workers to stress test memory (each worker allocates 256M bytes):
```shell
stress -m {{2}} --vm-bytes {{256M}}
```
#### Spawn 2 workers spinning on write()/unlink() (each worker writes 1G bytes):
```shell
stress -d {{2}} --hdd-bytes {{1GB}}
```
{% endraw %}{% raw %}
<h2 id="swapoff">
  <a href="/en/linux/swapoff.html">swapoff</a> <a href="#swapoff"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Disables device or file for swapping.

#### Disable a given swap partition:
```shell
swapoff {{/dev/sdb7}}
```
#### Disable a given swap file:
```shell
swapoff {{path/to/file}}
```
#### Disable all swap areas:
```shell
swapoff -a
```
#### Disable swap by label of a device or file:
```shell
swapoff -L {{swap1}}
```
{% endraw %}{% raw %}
<h2 id="swapon">
  <a href="/en/linux/swapon.html">swapon</a> <a href="#swapon"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Enables device or file for swapping.

#### Get swap information:
```shell
swapon -s
```
#### Enable a given swap partition:
```shell
swapon {{/dev/sdb7}}
```
#### Enable a given swap file:
```shell
swapon {{path/to/file}}
```
#### Enable all swap areas:
```shell
swapon -a
```
#### Enable swap by label of a device or file:
```shell
swapon -L {{swap1}}
```
{% endraw %}{% raw %}
<h2 id="swupd">
  <a href="/en/linux/swupd.html">swupd</a> <a href="#swupd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Package management utility for Clear Linux.
> More information: <https://docs.01.org/clearlinux/latest/guides/clear/swupd.html>.

#### Update to latest version:
```shell
sudo swupd update
```
#### Show current version, and check whether a newer one exists:
```shell
swupd check-update
```
#### List installed bundles:
```shell
swupd bundle-list
```
#### Locate the bundle where a wanted package exists:
```shell
swupd search -b {{package}}
```
#### Install a new bundle:
```shell
sudo swupd bundle-add {{bundle}}
```
#### Remove a bundle:
```shell
sudo swupd bundle-remove {{bundle}}
```
#### Correct broken or missing files:
```shell
sudo swupd verify
```
{% endraw %}{% raw %}
<h2 id="sxiv">
  <a href="/en/linux/sxiv.html">sxiv</a> <a href="#sxiv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Simple X Image Viewer.
> More information: <https://github.com/muennich/sxiv>.

#### Open an image:
```shell
sxiv {{path/to/file}}
```
#### Open an image in fullscreen mode:
```shell
sxiv -f {{path/to/file}}
```
#### Open a newline-separated list of images, reading filenames from standard input:
```shell
echo {{path/to/file}} | sxiv -i
```
#### Open a space-separated list of images as a slideshow:
```shell
sxiv -S {{seconds}} {{path/to/file}}
```
#### Open a space-separated list of images in thumbnail mode:
```shell
sxiv -t {{path/to/file}}
```
{% endraw %}{% raw %}
<h2 id="sysctl">
  <a href="/en/linux/sysctl.html">sysctl</a> <a href="#sysctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List and change kernel runtime variables.

#### Show all available variables and their values:
```shell
sysctl -a
```
#### Set a changeable kernel state variable:
```shell
sysctl -w {{section.tunable}}={{value}}
```
#### Get currently open file handlers:
```shell
sysctl fs.file-nr
```
#### Get limit for simultaneous open files:
```shell
sysctl fs.file-max
```
#### Apply changes from `/etc/sysctl.conf`:
```shell
sysctl -p
```
{% endraw %}{% raw %}
<h2 id="systemctl">
  <a href="/en/linux/systemctl.html">systemctl</a> <a href="#systemctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Control the systemd system and service manager.
> More information: <https://www.freedesktop.org/software/systemd/man/systemctl.html>.

#### List failed units:
```shell
systemctl --failed
```
#### Start/Stop/Restart/Reload a service:
```shell
systemctl {{start|stop|restart|reload}} {{unit}}
```
#### Show the status of a unit:
```shell
systemctl status {{unit}}
```
#### Enable/Disable a unit to be started on bootup:
```shell
systemctl {{enable|disable}} {{unit}}
```
#### Mask/Unmask a unit to prevent enablement and manual activation:
```shell
systemctl {{mask|unmask}} {{unit}}
```
#### Reload systemd, scanning for new or changed units:
```shell
systemctl daemon-reload
```
#### Check if a unit is active:
```shell
systemctl is-active {{unit}}
```
#### Check if a unit is enabled:
```shell
systemctl is-enabled {{unit}}
```
{% endraw %}{% raw %}
<h2 id="systemd-analyze">
  <a href="/en/linux/systemd-analyze.html">systemd-analyze</a> <a href="#systemd-analyze"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show timing details about the boot process of units (services, mount points, devices, sockets).

#### List time of each unit to start up:
```shell
systemd-analyze blame
```
#### Print a tree of the time critical chain of units:
```shell
systemd-analyze critical-chain
```
#### Create an SVG file showing when each system service started, highlighting the time that they spent on initialization:
```shell
systemd-analyze plot > {{path/to/file.svg}}
```
#### Plot a dependency graph and convert it to an SVG file:
```shell
systemd-analyze dot | dot -T{{svg}} > {{path/to/file.svg}}
```
{% endraw %}{% raw %}
<h2 id="taskset">
  <a href="/en/linux/taskset.html">taskset</a> <a href="#taskset"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Get or set a process' CPU affinity or start a new process with a defined CPU affinity.

#### Get a running process' CPU affinity by PID:
```shell
taskset --pid --cpu-list {{pid}}
```
#### Set a running process' CPU affinity by PID:
```shell
taskset --pid --cpu-list {{cpu_id}} {{pid}}
```
#### Start a new process with affinity for a single CPU:
```shell
taskset --cpu-list {{cpu_id}} {{command}}
```
#### Start a new process with affinity for multiple non-sequential CPUs:
```shell
taskset --cpu-list {{cpu_id_1}} {{cpu_id_2}} {{cpu_id_3}}
```
#### Start a new process with affinity for CPUs 1 through 4:
```shell
taskset --cpu-list {{cpu_id_1}},{{cpu_id_4}}
```
{% endraw %}{% raw %}
<h2 id="tcpflow">
  <a href="/en/linux/tcpflow.html">tcpflow</a> <a href="#tcpflow"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Capture TCP traffic for debugging and analysis.

#### Show all data on the given interface and port:
```shell
tcpflow -c -i {{eth0}} port {{80}}
```
{% endraw %}{% raw %}
<h2 id="tcpkill">
  <a href="/en/linux/tcpkill.html">tcpkill</a> <a href="#tcpkill"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Kills specified in-progress TCP connections.

#### Kill in-progress connections at a specified interface, host and port:
```shell
tcpkill -i {{eth1}} host {{192.95.4.27}} and port {{2266}}
```
{% endraw %}{% raw %}
<h2 id="tcptraceroute">
  <a href="/en/linux/tcptraceroute.html">tcptraceroute</a> <a href="#tcptraceroute"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A traceroute implementation using TCP packets.
> More information: <https://github.com/mct/tcptraceroute>.

#### Trace the route to a host:
```shell
tcptraceroute {{host}}
```
#### Specify the destination port and packet length in bytes:
```shell
tcptraceroute {{host}} {{destination_port}} {{packet_length}}
```
#### Specify the local source port and source address:
```shell
tcptraceroute {{host}} -p {{source_port}} -s {{source_address}}
```
#### Set the first and maximum TTL:
```shell
tcptraceroute {{host}} -f {{first_ttl}} -m {{max_ttl}}
```
#### Specify the wait time and number of queries per hop:
```shell
tcptraceroute {{host}} -w {{wait_time}} -q {{number_of_queries}}
```
#### Specify the interface:
```shell
tcptraceroute {{host}} -i {{interface}}
```
{% endraw %}{% raw %}
<h2 id="terminator">
  <a href="/en/linux/terminator.html">terminator</a> <a href="#terminator"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arrange multiple GNOME terminals in one window.
> More information: <https://gnome-terminator.org/>.

#### Start terminator window:
```shell
terminator
```
#### Start with a fullscreen window:
```shell
terminator -f
```
#### Split terminals horizontally:
```shell
Ctrl + Shift + O
```
#### Split terminals vertically:
```shell
Ctrl + Shift + E
```
#### Open new tab:
```shell
Ctrl + Shift + T
```
{% endraw %}{% raw %}
<h2 id="thunar">
  <a href="/en/linux/thunar.html">thunar</a> <a href="#thunar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Graphical file manager for XFCE desktop environments.
> More information: <https://docs.xfce.org/xfce/thunar/start>.

#### Open a new window showing the current directory:
```shell
thunar
```
#### Open the bulk rename utility:
```shell
thunar --bulk-rename
```
#### Close all open thunar windows:
```shell
thunar --quit
```
{% endraw %}{% raw %}
<h2 id="tic">
  <a href="/en/linux/tic.html">tic</a> <a href="#tic"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Compile terminfo and install for ncurses.
> More information: <https://pubs.opengroup.org/onlinepubs/007908799/xcurses/terminfo.html>.

#### Compile and install terminfo for a terminal:
```shell
tic -xe {{terminal}} {{path/to/terminal.info}}
```
#### Check terminfo file for errors:
```shell
tic -c {{path/to/terminal.info}}
```
#### Print database locations:
```shell
tic -D
```
{% endraw %}{% raw %}
<h2 id="timedatectl">
  <a href="/en/linux/timedatectl.html">timedatectl</a> <a href="#timedatectl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Control the system time and date.
> More information: <https://manned.org/timedatectl.1>.

#### Check the current system clock time:
```shell
timedatectl
```
#### Set the local time of the system clock directly:
```shell
timedatectl set-time "{{yyyy-MM-dd hh:mm:ss}}"
```
#### List available timezones:
```shell
timedatectl list-timezones
```
#### Set the system timezone:
```shell
timedatectl set-timezone {{timezone}}
```
#### Enable Network Time Protocol (NTP) synchronization:
```shell
timedatectl set-ntp on
```
{% endraw %}{% raw %}
<h2 id="timeshift">
  <a href="/en/linux/timeshift.html">timeshift</a> <a href="#timeshift"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> System restore utility.
> More information: <https://github.com/teejee2008/timeshift>.

#### List snapshots:
```shell
sudo timeshift --list
```
#### Create a new snapshot (if scheduled):
```shell
sudo timeshift --check
```
#### Create a new snapshot (even if not scheduled):
```shell
sudo timeshift --create
```
#### Restore a snapshot (selecting which snapshot to restore interactively):
```shell
sudo timeshift --restore
```
#### Restore a specific snapshot:
```shell
sudo timeshift --restore --snapshot '{{snapshot}}'
```
#### Delete a specific snapshot:
```shell
sudo timeshift --delete --snapshot '{{snapshot}}'
```
{% endraw %}{% raw %}
<h2 id="tlp-stat">
  <a href="/en/linux/tlp-stat.html">tlp-stat</a> <a href="#tlp-stat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool to generate TLP status reports.
> See also `tlp`.
> More information: <https://linrunner.de/tlp/usage/tlp-stat>.

#### Generate status report with configuration and all active settings:
```shell
sudo tlp-stat
```
#### Show battery information:
```shell
sudo tlp-stat -b
```
#### Show configuration:
```shell
sudo tlp-stat -c
```
{% endraw %}{% raw %}
<h2 id="tlp">
  <a href="/en/linux/tlp.html">tlp</a> <a href="#tlp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Advanced power management for Linux.
> See also `tlp-stat`.
> More information: <https://linrunner.de/tlp/>.

#### Apply settings (according to the actual power source):
```shell
sudo tlp start
```
#### Apply battery settings (ignoring the actual power source):
```shell
sudo tlp bat
```
#### Apply AC settings (ignoring the actual power source):
```shell
sudo tlp ac
```
{% endraw %}{% raw %}
<h2 id="toilet">
  <a href="/en/linux/toilet.html">toilet</a> <a href="#toilet"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool to display ASCII-art fonts.
> More information: <http://caca.zoy.org/wiki/toilet>.

#### Generate ASCII art for a given text:
```shell
toilet {{input_text}}
```
#### Generate ASCII art using a custom font file:
```shell
toilet {{input_text}} -f {{font_filename}}
```
#### Generate ASCII art using a filter:
```shell
toilet {{input_text}} --filter {{filter_name}}
```
#### Show available toilet filters:
```shell
toilet --filter list 
```
{% endraw %}{% raw %}
<h2 id="tomb">
  <a href="/en/linux/tomb.html">tomb</a> <a href="#tomb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage encrypted storage directories that can be safely transported and hidden in a filesystem.
> More information: <https://www.dyne.org/software/tomb/>.

#### Create a new tomb with an initial size of 100MB:
```shell
tomb dig -s {{100}} {{encrypted_directory.tomb}}
```
#### Create a new key file that can be used to lock a tomb; user will be prompted for a password for the key:
```shell
tomb forge {{encrypted_directory.tomb.key}}
```
#### Initialize and lock an empty tomb using a key made with `forge`:
```shell
tomb lock {{encrypted_directory.tomb}} -k {{encrypted_directory.tomb.key}}
```
#### Mount a tomb (by default in `/media`) using its key, making it usable as a regular filesystem directory:
```shell
tomb open {{encrypted_directory.tomb}} -k {{encrypted_directory.tomb.key}}
```
#### Close a tomb (fails if the tomb is being used by a process):
```shell
tomb close {{encrypted_directory.tomb}}
```
#### Forcefully close all open tombs, killing any applications using them:
```shell
tomb slam all
```
#### List all open tombs:
```shell
tomb list
```
{% endraw %}{% raw %}
<h2 id="top">
  <a href="/en/linux/top.html">top</a> <a href="#top"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display dynamic real-time information about running processes.

#### Start top:
```shell
top
```
#### Do not show any idle or zombie processes:
```shell
top -i
```
#### Show only processes owned by given user:
```shell
top -u {{username}}
```
#### Sort processes by a field:
```shell
top -o {{field_name}}
```
#### Show the individual threads of a given process:
```shell
top -Hp {{process_id}}
```
#### Show only the processes with the given PID(s), passed as a comma-separated list. (Normally you wouldn't know PIDs off hand. This example picks the PIDs from the process name):
```shell
top -p $(pgrep -d ',' {{process_name}})
```
#### Get help about interactive commands:
```shell
?
```
{% endraw %}{% raw %}
<h2 id="tracepath">
  <a href="/en/linux/tracepath.html">tracepath</a> <a href="#tracepath"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Trace the path to a network host discovering MTU along this path.
> More information: <https://manned.org/tracepath>.

#### A preferred way to trace the path to a host:
```shell
tracepath -p {{33434}} {{host}}
```
#### Specify the initial destination port, useful with non-standard firewall settings:
```shell
tracepath -p {{destination_port}} {{host}} 
```
#### Print both hostnames and numerical IP addresses:
```shell
tracepath -b {{host}}
```
#### Specify a maximum TTL (number of hops):
```shell
tracepath -m {{max_hops}} {{host}}
```
#### Specify the initial packet length (defaults to 65535 for IPv4 and 128000 for IPv6):
```shell
tracepath -l {{packet_length}} {{host}}
```
#### Use only IPv6 addresses:
```shell
tracepath -6 {{host}}
```
{% endraw %}{% raw %}
<h2 id="trap">
  <a href="/en/linux/trap.html">trap</a> <a href="#trap"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Automatically execute commands after receiving signals by processes or the operating system.
> Can be used to perform cleanups for interruptions by the user or other actions.

#### List available signals to set traps for:
```shell
trap -l
```
#### List active traps for the current shell:
```shell
trap -p
```
#### Set a trap to execute commands when one or more signals are detected:
```shell
trap 'echo "Caught signal {{SIGHUP}}"' {{SIGHUP}}
```
#### Remove active traps:
```shell
trap - {{SIGHUP}} {{SIGINT}}
```
{% endraw %}{% raw %}
<h2 id="trash">
  <a href="/en/linux/trash.html">trash</a> <a href="#trash"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A CLI for managing your trashcan / recycling bin.
> More information: <https://github.com/andreafrancia/trash-cli>.

#### Delete a file (send to trash):
```shell
trash {{path/to/file}}
```
#### List files in trash:
```shell
trash-list
```
#### Restore file from trash:
```shell
trash-restore
```
#### Empty trash:
```shell
trash-empty
```
#### Empty trash, keeping files trashed less than {{10}} days ago:
```shell
trash-empty {{10}}
```
#### Remove all files named 'foo' from the trash:
```shell
trash-rm foo
```
#### Remove all files with a given original location:
```shell
trash-rm {{/absolute/path/to/file_or_directory}}
```
{% endraw %}{% raw %}
<h2 id="tree">
  <a href="/en/linux/tree.html">tree</a> <a href="#tree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show the contents of the current directory as a tree.
> More information: <http://mama.indstate.edu/users/ice/tree/>.

#### Print files and directories up to 'num' levels of depth (where 1 means the current directory):
```shell
tree -L {{num}}
```
#### Print directories only:
```shell
tree -d
```
#### Print hidden files too with colorization on:
```shell
tree -a -C
```
#### Print the tree without indentation lines, showing the full path instead (use `-N` to not escape non-printable characters):
```shell
tree -i -f
```
#### Print the size of each file and the cumulative size of each directory, in human-readable format:
```shell
tree -s -h --du
```
#### Print files within the tree hierarchy, using a wildcard (glob) pattern, and pruning out directories that don't contain matching files:
```shell
tree -P '{{*.txt}}' --prune
```
#### Print directories within the tree hierarchy, using the wildcard (glob) pattern, and pruning out directories that aren't ancestors of the wanted one:
```shell
tree -P {{directory_name}} --matchdirs --prune
```
#### Print the tree ignoring the given directories:
```shell
tree -I '{{directory_name1|directory_name2}}'
```
{% endraw %}{% raw %}
<h2 id="trizen">
  <a href="/en/linux/trizen.html">trizen</a> <a href="#trizen"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux utility for building packages from the Arch User Repository (AUR).

#### Synchronize and update all AUR packages:
```shell
trizen -Syua
```
#### Install a new package:
```shell
trizen -S {{package}}
```
#### Remove a package and its dependencies:
```shell
trizen -Rs {{package}}
```
#### Search the package database for a keyword:
```shell
trizen -Ss {{keyword}}
```
#### Show information about a package:
```shell
trizen -Si {{package}}
```
#### List installed packages and versions:
```shell
trizen -Qe
```
{% endraw %}{% raw %}
<h2 id="tshark">
  <a href="/en/linux/tshark.html">tshark</a> <a href="#tshark"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Packet analysis tool, CLI version of Wireshark.

#### Monitor everything on localhost:
```shell
tshark
```
#### Only capture packets matching a specific capture filter:
```shell
tshark -f '{{udp port 53}}'
```
#### Only show packets matching a specific output filter:
```shell
tshark -Y '{{http.request.method == "GET"}}'
```
#### Decode a TCP port using a specific protocol (e.g. HTTP):
```shell
tshark -d tcp.port=={{8888}},{{http}}
```
#### Specify the format of captured output:
```shell
tshark -T {{json|text|ps|…}}
```
#### Select specific fields to output:
```shell
tshark -T {{fields|ek|json|pdml}} -e {{http.request.method}} -e {{ip.src}}
```
#### Write captured packet to a file:
```shell
tshark -w {{path/to/file}}
```
#### Analyze packets from a file:
```shell
tshark -r {{filename}}.pcap
```
{% endraw %}{% raw %}
<h2 id="tune2fs">
  <a href="/en/linux/tune2fs.html">tune2fs</a> <a href="#tune2fs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Adjust parameters of an ext2, ext3 or ext4 filesystem.
> May be used on mounted filesystems.

#### Set the max number of counts before a filesystem is checked to 2:
```shell
tune2fs -c {{2}} {{/dev/sdXN}}
```
#### Set the filesystem label to MY_LABEL:
```shell
tune2fs -L {{'MY_LABEL'}} {{/dev/sdXN}}
```
#### Enable discard and user-specified extended attributes for a filesystem:
```shell
tune2fs -o {{discard,user_xattr}} {{/dev/sdXN}}
```
#### Enable journaling for a filesystem:
```shell
tune2fs -o^{{nobarrier}} {{/dev/sdXN}}
```
{% endraw %}{% raw %}
<h2 id="tuxi">
  <a href="/en/linux/tuxi.html">tuxi</a> <a href="#tuxi"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A CLI tool that scrapes Google search results and SERPs that provides instant and concise answers.
> More information: <https://github.com/Bugswriter/tuxi>.

#### Make a search using Google:
```shell
tuxi {{search_terms}}
```
#### Display the search results in [r]aw format (no pretty output, no colors):
```shell
tuxi -r {{search_terms}}
```
#### Display only search results (silences "Did you mean?", greetings and usage):
```shell
tuxi -q {{search_terms}}
```
#### Display help:
```shell
tuxi -h
```
{% endraw %}{% raw %}
<h2 id="udisksctl">
  <a href="/en/linux/udisksctl.html">udisksctl</a> <a href="#udisksctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line program used to interact with the udisksd daemon process.
> More information: <http://storaged.org/doc/udisks2-api/latest/udisksctl.1.html>.

#### Show high-level information about disk drives and block devices:
```shell
udisksctl status
```
#### Show detailed information about a device:
```shell
udisksctl info --block-device {{/dev/sdX}}
```
#### Show detailed information about a device partition:
```shell
udisksctl info --block-device {{/dev/sdXN}}
```
#### Mount a device partition and prints the mount point:
```shell
udisksctl mount --block-device {{/dev/sdXN}}
```
#### Unmount a device partition:
```shell
udisksctl unmount --block-device {{/dev/sdXN}}
```
#### Monitor the daemon for events:
```shell
udisksctl monitor
```
{% endraw %}{% raw %}
<h2 id="ufw">
  <a href="/en/linux/ufw.html">ufw</a> <a href="#ufw"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Uncomplicated Firewall.
> Frontend for iptables aiming to make configuration of a firewall easier.
> More information: <https://wiki.ubuntu.com/UncomplicatedFirewall>.

#### Enable ufw:
```shell
ufw enable
```
#### Disable ufw:
```shell
ufw disable
```
#### Show ufw rules, along with their numbers:
```shell
ufw status numbered
```
#### Allow incoming traffic on port 5432 on this host with a comment identifying the service:
```shell
ufw allow {{5432}} comment "{{Service}}"
```
#### Allow only TCP traffic from 192.168.0.4 to any address on this host, on port 22:
```shell
ufw allow proto {{tcp}} from {{192.168.0.4}} to {{any}} port {{22}}
```
#### Deny traffic on port 80 on this host:
```shell
ufw deny {{80}}
```
#### Deny all UDP traffic to port 22:
```shell
ufw deny proto {{udp}} from {{any}} to {{any}} port {{22}}
```
#### Delete a particular rule. The rule number can be retrieved from the `ufw status numbered` command:
```shell
ufw delete {{rule_number}}
```
{% endraw %}{% raw %}
<h2 id="ul">
  <a href="/en/linux/ul.html">ul</a> <a href="#ul"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Performs the underlining of a text.
> Each character in a given string must be underlined separately.

#### Display the contents of the file with underlines where applicable:
```shell
ul {{file.txt}}
```
#### Display the contents of the file with underlines made of dashes `-`:
```shell
ul -i {{file.txt}}
```
{% endraw %}{% raw %}
<h2 id="unix2dos">
  <a href="/en/linux/unix2dos.html">unix2dos</a> <a href="#unix2dos"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Change Unix-style line endings to DOS-style.
> Replaces CR with CRLF.

#### Change the line endings of a file:
```shell
unix2dos {{filename}}
```
#### Create a copy with DOS-style line endings:
```shell
unix2dos -n {{filename}} {{new_filename}}
```
{% endraw %}{% raw %}
<h2 id="unix2mac">
  <a href="/en/linux/unix2mac.html">unix2mac</a> <a href="#unix2mac"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Change Unix-style line endings to macOS-style.
> Replaces CR with LF.

#### Change the line endings of a file:
```shell
unix2mac {{filename}}
```
#### Create a copy with macOS-style line endings:
```shell
unix2mac -n {{filename}} {{new_filename}}
```
{% endraw %}{% raw %}
<h2 id="unset">
  <a href="/en/linux/unset.html">unset</a> <a href="#unset"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remove shell variables or functions.

#### Remove the variable `foo`, or if the variable doesn't exist, remove the function `foo`:
```shell
unset {{foo}}
```
#### Remove the variables foo and bar:
```shell
unset -v {{foo}} {{bar}}
```
#### Remove the function my_func:
```shell
unset -f {{my_func}}
```
{% endraw %}{% raw %}
<h2 id="unshadow">
  <a href="/en/linux/unshadow.html">unshadow</a> <a href="#unshadow"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility provided by the John the Ripper project to obtain the traditional Unix password file if the system uses shadow passwords.
> More information: <https://www.openwall.com/john/>.

#### Combine the `/etc/shadow` and `/etc/passwd` of the current system:
```shell
sudo unshadow /etc/passwd /etc/shadow
```
#### Combine two arbitrary shadow and password files:
```shell
sudo unshadow {{path/to/passwd}} {{path/to/shadow}}
```
{% endraw %}{% raw %}
<h2 id="update-alternatives">
  <a href="/en/linux/update-alternatives.html">update-alternatives</a> <a href="#update-alternatives"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A convenient tool for maintaining symbolic links to determine default commands.

#### Add a symbolic link:
```shell
sudo update-alternatives --install {{path/to/symlink}} {{command_name}} {{path/to/command_binary}} {{priority}}
```
#### Configure a symbolic link for `java`:
```shell
sudo update-alternatives --config {{java}}
```
#### Remove a symbolic link:
```shell
sudo update-alternatives --remove {{java}} {{/opt/java/jdk1.8.0_102/bin/java}}
```
#### Display information about a specified command:
```shell
update-alternatives --display {{java}}
```
#### Display all commands and their current selection:
```shell
update-alternatives --get-selections
```
{% endraw %}{% raw %}
<h2 id="update-rc.d">
  <a href="/en/linux/update-rc.d.html">update-rc.d</a> <a href="#update-rc.d"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Install and remove services which are System-V style init script links.
> Init scripts are in the `/etc/init.d/`.

#### Install a service:
```shell
update-rc.d {{mysql}} defaults
```
#### Enable a service:
```shell
update-rc.d {{mysql}} enable
```
#### Disable a service:
```shell
update-rc.d {{mysql}} disable
```
#### Forcibly remove a service:
```shell
update-rc.d -f {{mysql}} remove
```
{% endraw %}{% raw %}
<h2 id="updatedb">
  <a href="/en/linux/updatedb.html">updatedb</a> <a href="#updatedb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create or update the database used by `locate`.
> It is usually run daily by cron.

#### Refresh database content:
```shell
sudo updatedb
```
#### Display file names as soon as they are found:
```shell
sudo updatedb --verbose
```
{% endraw %}{% raw %}
<h2 id="upower">
  <a href="/en/linux/upower.html">upower</a> <a href="#upower"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> System utility to provide power and battery information and statistics.
> More information: <https://upower.freedesktop.org/docs/upower.1.html>.

#### Display power and battery information:
```shell
upower --dump
```
#### List all power devices:
```shell
upower --enumerate
```
#### Watch for and print power status changes:
```shell
upower --monitor
```
#### Watch for and print detailed power status changes:
```shell
upower --monitor-detail
```
#### Display version:
```shell
upower --version
```
{% endraw %}{% raw %}
<h2 id="uprecords">
  <a href="/en/linux/uprecords.html">uprecords</a> <a href="#uprecords"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Displays a summary of historical uptime records.

#### Display a summary of the top 10 historical uptime records:
```shell
uprecords
```
#### Display the top 25 records:
```shell
uprecords -m {{25}}
```
#### Display the downtime between reboots instead of the kernel version:
```shell
uprecords -d
```
#### Show the most recent reboots:
```shell
uprecords -B
```
#### Don't truncate information:
```shell
uprecords -w
```
{% endraw %}{% raw %}
<h2 id="urxvt">
  <a href="/en/linux/urxvt.html">urxvt</a> <a href="#urxvt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rxvt-unicode.
> A customizable terminal emulator.

#### Open a new urxvt window:
```shell
urxvt
```
#### Run in a specific directory:
```shell
urxvt -cd {{path/to/directory}}
```
#### Run a command in a new urxvt window:
```shell
urxvt -e {{command}}
```
#### Run a command and keep the window open:
```shell
urxvt --hold -e {{command}}
```
#### Run a command within the `sh` shell:
```shell
urxvt -e {{sh}} -c {{command}}
```
{% endraw %}{% raw %}
<h2 id="useradd">
  <a href="/en/linux/useradd.html">useradd</a> <a href="#useradd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create a new user.
> More information: <https://manned.org/useradd>.

#### Create new user:
```shell
useradd {{name}}
```
#### Create new user with a default home directory:
```shell
useradd --create-home {{name}}
```
#### Create new user with specified shell:
```shell
useradd --shell {{path/to/shell}} {{name}}
```
#### Create new user belonging to additional groups (mind the lack of whitespace):
```shell
useradd --groups {{group1,group2}} {{name}}
```
#### Create new system user without a home directory:
```shell
useradd --no-create-home --system {{name}}
```
{% endraw %}{% raw %}
<h2 id="userdel">
  <a href="/en/linux/userdel.html">userdel</a> <a href="#userdel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Remove a user account or remove a user from a group.
> Note: all commands must be executed as root.
> More information: <https://manned.org/userdel>.

#### Remove a user:
```shell
userdel {{name}}
```
#### Remove a user along with their home directory and mail spool:
```shell
userdel --remove {{name}}
```
#### Remove a user from a group:
```shell
userdel {{name}} {{group}}
```
#### Remove a user in other root directory:
```shell
userdel --root {{path/to/other/root}} {{name}}
```
{% endraw %}{% raw %}
<h2 id="usermod">
  <a href="/en/linux/usermod.html">usermod</a> <a href="#usermod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Modifies a user account.
> More information: <https://manned.org/usermod>.

#### Change a user's name:
```shell
usermod -l {{newname}} {{user}}
```
#### Add user to supplementary groups (mind the whitespace):
```shell
usermod -a -G {{group1,group2}} {{user}}
```
#### Create a new home directory for a user and move their files to it:
```shell
usermod -m -d {{path/to/home}} {{user}}
```
{% endraw %}{% raw %}
<h2 id="utmpdump">
  <a href="/en/linux/utmpdump.html">utmpdump</a> <a href="#utmpdump"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Dump and load btmp, utmp and wtmp accounting files.

#### Dump the `/var/log/wtmp` file to the standard output as plain text:
```shell
utmpdump {{/var/log/wtmp}}
```
#### Load a previously dumped file into `/var/log/wtmp`:
```shell
utmpdump -r {{dumpfile}} > {{/var/log/wtmp}}
```
{% endraw %}{% raw %}
<h2 id="uuid">
  <a href="/en/linux/uuid.html">uuid</a> <a href="#uuid"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate and decode Universally Unique Identifiers (UUID).
> See also `uuidgen`.
> More information: <https://manned.org/uuid>.

#### Generate a UUIDv1 (based on time and system's hardware address, if present):
```shell
uuid
```
#### Generate a UUIDv4 (based on random data):
```shell
uuid -v {{4}}
```
#### Generate multiple UUIDv4 identifiers at once:
```shell
uuid -v {{4}} -n {{number_of_uuids}}
```
#### Generate a UUIDv4 and specify the output format:
```shell
uuid -v {{4}} -F {{BIN|STR|SIV}}
```
#### Generate a UUIDv4 and write the output to a file:
```shell
uuid -v {{4}} -o {{path/to/file}}
```
#### Generate a UUIDv5 (based on the supplied object name) with a specified namespace prefix:
```shell
uuid -v {{5}} ns:{{DNS|URL|OID|X500}} {{object_name}}
```
#### Decode a given UUID:
```shell
uuid -d {{uuid}}
```
{% endraw %}{% raw %}
<h2 id="uuidd">
  <a href="/en/linux/uuidd.html">uuidd</a> <a href="#uuidd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Daemon for generating UUIDs.
> More information: <https://manned.org/uuidd>.

#### Generate a random UUID:
```shell
uuidd --random
```
#### Generate a bulk number of random UUIDs:
```shell
uuidd --random --uuids {{number_of_uuids}}
```
#### Generate a time-based UUID, based on the current time and MAC address of the system:
```shell
uuidd --time
```
{% endraw %}{% raw %}
<h2 id="uuidgen">
  <a href="/en/linux/uuidgen.html">uuidgen</a> <a href="#uuidgen"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate unique identifiers (UUIDs).
> See also `uuid`.
> More information: <https://manned.org/uuidgen>.

#### Create a random UUIDv4:
```shell
uuidgen --random
```
#### Create a UUIDv1 based on the current time:
```shell
uuidgen --time
```
#### Create a UUIDv5 of the name with a specified namespace prefix:
```shell
uuidgen --sha1 --namespace {{@dns|@url|@oid|@x500}} --name {{object_name}}
```
{% endraw %}{% raw %}
<h2 id="uvcdynctrl">
  <a href="/en/linux/uvcdynctrl.html">uvcdynctrl</a> <a href="#uvcdynctrl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A libwebcam command-line tool to manage dynamic controls in uvcvideo.

#### List all available cameras:
```shell
uvcdynctrl -l
```
#### Specify the device to use (defaults to `video0`):
```shell
uvcdynctrl -d {{device_name}}
```
#### List available controls:
```shell
uvcdynctrl -c
```
#### Set a new control value (for negative values, add -- before {{-value}}):
```shell
uvcdynctrl -s {{control_name}} {{value}}
```
#### Get the current control value:
```shell
uvcdynctrl -g {{control_name}}
```
#### Save the state of the current controls to a file:
```shell
uvcdynctrl -W {{filename}}
```
#### Load the state of the controls from a file:
```shell
uvcdynctrl -L {{filename}}
```
{% endraw %}{% raw %}
<h2 id="veracrypt">
  <a href="/en/linux/veracrypt.html">veracrypt</a> <a href="#veracrypt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Free and open source disk encryption software.
> More information: <https://www.veracrypt.fr/code/VeraCrypt/plain/doc/html/Documentation.html>.

#### Create a new volume through a text user interface and use `/dev/urandom` as a source of random data:
```shell
veracrypt --text --create --random-source={{/dev/urandom}}
```
#### Decrypt a volume interactively through a text user interface and mount it to a directory:
```shell
veracrypt --text {{path/to/volume}} {{path/to/mount_point}}
```
#### Decrypt a partition using a keyfile and mount it to a directory:
```shell
veracrypt --keyfiles={{path/to/keyfile}} {{/dev/sdXN}} {{path/to/mount_point}}
```
#### Dismount a volume on the directory it is mounted to:
```shell
veracrypt --dismount {{path/to/mounted_point}}
```
{% endraw %}{% raw %}
<h2 id="vgcreate">
  <a href="/en/linux/vgcreate.html">vgcreate</a> <a href="#vgcreate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create volume groups combining multiple mass-storage devices.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/vgcreate.8.html>.

#### Create a new volume group called vg1 using the `/dev/sda1` device:
```shell
vgcreate {{vg1}} {{/dev/sda1}}
```
#### Create a new volume group called vg1 using multiple devices:
```shell
vgcreate {{vg1}} {{/dev/sda1}} {{/dev/sdb1}} {{/dev/sdc1}}
```
{% endraw %}{% raw %}
<h2 id="vgdisplay">
  <a href="/en/linux/vgdisplay.html">vgdisplay</a> <a href="#vgdisplay"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display information about Logical Volume Manager (LVM) volume groups.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/vgdisplay.8.html>.

#### Display information about all volume groups:
```shell
sudo vgdisplay
```
#### Display information about volume group vg1:
```shell
sudo vgdisplay {{vg1}}
```
{% endraw %}{% raw %}
<h2 id="vgs">
  <a href="/en/linux/vgs.html">vgs</a> <a href="#vgs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display information about volume groups.
> See also: `lvm`.
> More information: <https://man7.org/linux/man-pages/man8/vgs.8.html>.

#### Display information about volume groups:
```shell
vgs
```
#### Display all volume groups:
```shell
vgs -a
```
#### Change default display to show more details:
```shell
vgs -v
```
#### Display only specific fields:
```shell
vgs -o {{field_name_1}},{{field_name_2}}
```
#### Append field to default display:
```shell
vgs -o +{{field_name}}
```
#### Suppress heading line:
```shell
vgs --noheadings
```
#### Use separator to separate fields:
```shell
vgs --separator =
```
{% endraw %}{% raw %}
<h2 id="viewnior">
  <a href="/en/linux/viewnior.html">viewnior</a> <a href="#viewnior"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Simple and elegant image viewer.

#### View an image:
```shell
viewnior {{path/to/image.ext}}
```
#### View in fullscreen mode:
```shell
viewnior --fullscreen {{path/to/image.ext}}
```
#### View fullscreen in slideshow mode:
```shell
viewnior --slideshow {{path/to/image.ext}}
```
{% endraw %}{% raw %}
<h2 id="vipw">
  <a href="/en/linux/vipw.html">vipw</a> <a href="#vipw"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Edit the password file.
> More information: <https://manned.org/vipw>.

#### Edit the password file:
```shell
vipw
```
#### Display the current version of `vipw`:
```shell
vipw --version
```
{% endraw %}{% raw %}
<h2 id="virt-manager">
  <a href="/en/linux/virt-manager.html">virt-manager</a> <a href="#virt-manager"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI launcher for virt-manager, a desktop user interface for managing KVM and Xen virtual machines and LXC containers.
> More information: <https://manpages.ubuntu.com/manpages/man1/virt-manager.1.html>.

#### Launch virt-manager:
```shell
virt-manager
```
#### Connect to a hypervisor:
```shell
virt-manager --connect {{hypervisor_uri}}
```
#### Don't fork virt-manager process into background on startup:
```shell
virt-manager --no-fork
```
#### Print debug output:
```shell
virt-manager --debug
```
#### Open the "New VM" wizard:
```shell
virt-manager --show-domain-creator
```
#### Show domain details window:
```shell
virt-manager --show-domain-editor {{name|id|uuid}}
```
#### Show domain performance window:
```shell
virt-manager --show-domain-performance {{name|id|uuid}}
```
#### Show connection details window:
```shell
virt-manager --show-host-summary
```
{% endraw %}{% raw %}
<h2 id="vmstat">
  <a href="/en/linux/vmstat.html">vmstat</a> <a href="#vmstat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Report information about processes, memory, paging, block IO, traps, disks and CPU activity.
> More information: <https://manned.org/vmstat>.

#### Display virtual memory statistics:
```shell
vmstat
```
#### Display reports every 2 seconds for 5 times:
```shell
vmstat {{2}} {{5}}
```
{% endraw %}{% raw %}
<h2 id="vmware-checkvm">
  <a href="/en/linux/vmware-checkvm.html">vmware-checkvm</a> <a href="#vmware-checkvm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Checks to see if the current host is a VMware VM or not.

#### Return the current VMware software version (exit status determines whether the system is a VM or not):
```shell
vmware-checkvm
```
#### Return the VMware hardware version:
```shell
vmware-checkvm -h
```
{% endraw %}{% raw %}
<h2 id="vncserver">
  <a href="/en/linux/vncserver.html">vncserver</a> <a href="#vncserver"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Launches a VNC (Virtual Network Computing) desktop.

#### Launch a VNC Server on next available display:
```shell
vncserver
```
#### Launch a VNC Server with specific screen geometry:
```shell
vncserver --geometry {{width}}x{{height}}
```
#### Kill an instance of VNC Server running on a specific display:
```shell
vncserver --kill :{{display_number}}
```
{% endraw %}{% raw %}
<h2 id="vncviewer">
  <a href="/en/linux/vncviewer.html">vncviewer</a> <a href="#vncviewer"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Launches a VNC (Virtual Network Computing) client.

#### Launch a VNC client which connects to a host on a given display:
```shell
vncviewer {{host}}:{{display_number}}
```
#### Launch in full-screen mode:
```shell
vncviewer -FullScreen {{host}}:{{display_number}}
```
#### Launch a VNC client with a specific screen geometry:
```shell
vncviewer --geometry {{width}}x{{height}} {{host}}:{{display_number}}
```
#### Launch a VNC client which connects to a host on a given port:
```shell
vncviewer {{host}}::{{port}}
```
{% endraw %}{% raw %}
<h2 id="vnstat">
  <a href="/en/linux/vnstat.html">vnstat</a> <a href="#vnstat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A console-based network traffic monitor.

#### Display traffic summary for all interfaces:
```shell
vnstat
```
#### Display traffic summary for a specific network interface:
```shell
vnstat -i {{eth0}}
```
#### Display live stats for a specific network interface:
```shell
vnstat -l -i {{eth0}}
```
#### Show traffic statistics on an hourly basis for the last 24 hours using a bar graph:
```shell
vnstat -hg
```
#### Measure and show average traffic for 30 seconds:
```shell
vnstat -tr {{30}}
```
{% endraw %}{% raw %}
<h2 id="vpnc">
  <a href="/en/linux/vpnc.html">vpnc</a> <a href="#vpnc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A VPN client for the Cisco 3000 VPN Concentrator.

#### Connect with a defined configuration file:
```shell
sudo vpnc {{config_file}}
```
#### Terminate the previously created connection:
```shell
sudo vpnc-disconnect
```
{% endraw %}{% raw %}
<h2 id="vrms">
  <a href="/en/linux/vrms.html">vrms</a> <a href="#vrms"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Report non-free packages installed on Debian-based OSes.
> More information: <https://debian.pages.debian.net/vrms/>.

#### List non-free and contrib packages (and their description):
```shell
vrms
```
#### Only output the package names:
```shell
vrms --sparse
```
{% endraw %}{% raw %}
<h2 id="w">
  <a href="/en/linux/w.html">w</a> <a href="#w"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display who is logged in and their processes.
> More information: <https://www.geeksforgeeks.org/w-command-in-linux-with-examples/>.

#### Display information about all users who are currently logged in:
```shell
w
```
#### Display information about a specific user:
```shell
w {{user}}
```
#### Display information without including the header:
```shell
w --no-header
```
#### Display information without including the login, JCPU and PCPU columns:
```shell
w --short
```
{% endraw %}{% raw %}
<h2 id="wall">
  <a href="/en/linux/wall.html">wall</a> <a href="#wall"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Write a message on the terminals of users currently logged in.

#### Send a message:
```shell
echo "{{message}}" | wall
```
#### Send a message from a file:
```shell
wall {{file}}
```
#### Send a message with timeout (default 300):
```shell
wall -t {{seconds}} {{file}}
```
{% endraw %}{% raw %}
<h2 id="watch">
  <a href="/en/linux/watch.html">watch</a> <a href="#watch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Execute a command repeatedly, and monitor the output in full-screen mode.

#### Monitor files in the current directory:
```shell
watch {{ls}}
```
#### Monitor disk space and highlight the changes:
```shell
watch -d {{df}}
```
#### Monitor "node" processes, refreshing every 3 seconds:
```shell
watch -n {{3}} "{{ps aux | grep node}}"
```
{% endraw %}{% raw %}
<h2 id="wg-quick">
  <a href="/en/linux/wg-quick.html">wg-quick</a> <a href="#wg-quick"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Quickly set up WireGuard tunnels based on config files.
> More information: <https://www.wireguard.com/quickstart/>.

#### Set up a VPN tunnel:
```shell
wg-quick up {{interface_name}}
```
#### Delete a VPN tunnel:
```shell
wg-quick down {{interface_name}}
```
{% endraw %}{% raw %}
<h2 id="wg">
  <a href="/en/linux/wg.html">wg</a> <a href="#wg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage the configuration of WireGuard interfaces.
> More information: <https://www.wireguard.com/quickstart/>.

#### Check status of currently active interfaces:
```shell
sudo wg
```
#### Print a new private key:
```shell
wg genkey
```
#### Print a new public key:
```shell
echo {{private_key}} | wg pubkey
```
#### Generate a public and private key:
```shell
wg genkey | tee {{privatekey.txt}} | wg pubkey > {{publickey.txt}}
```
{% endraw %}{% raw %}
<h2 id="whatis">
  <a href="/en/linux/whatis.html">whatis</a> <a href="#whatis"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display one-line descriptions from manual pages.

#### Display a description from a man page:
```shell
whatis {{command}}
```
#### Don't cut the description off at the end of the line:
```shell
whatis --long {{command}}
```
#### Display descriptions for all commands matching a glob:
```shell
whatis --wildcard {{net*}}
```
#### Search man page descriptions with a regular expression:
```shell
whatis --regex '{{wish[0-9]\.[0-9]}}'
```
{% endraw %}{% raw %}
<h2 id="whereis">
  <a href="/en/linux/whereis.html">whereis</a> <a href="#whereis"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Locate the binary, source, and manual page files for a command.

#### Locate binary, source and man pages for ssh:
```shell
whereis {{ssh}}
```
#### Locate binary and man pages for ls:
```shell
whereis -bm {{ls}}
```
#### Locate source of gcc and man pages for Git:
```shell
whereis -s {{gcc}} -m {{git}}
```
#### Locate binaries for gcc in `/usr/bin/` only:
```shell
whereis -b -B {{/usr/bin/}} -f {{gcc}}
```
#### Locate unusual binaries (those that have more or less than one binary on the system):
```shell
whereis -u *
```
#### Locate binaries that have unusual manual entries (binaries that have more or less than one manual installed):
```shell
whereis -u -m *
```
{% endraw %}{% raw %}
<h2 id="whiptail">
  <a href="/en/linux/whiptail.html">whiptail</a> <a href="#whiptail"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display text-based dialog boxes from shell scripts.

#### Display a simple message:
```shell
whiptail --title "{{title}}" --msgbox "{{message}}" {{height_in_chars}} {{width_in_chars}}
```
#### Display a boolean choice, returning the result through the exit code:
```shell
whiptail --title "{{title}}" --yesno "{{message}}" {{height_in_chars}} {{width_in_chars}}
```
#### Customise the text on the yes / no buttons:
```shell
whiptail --title "{{title}}" --yes-button "{{text}}" --no-button "{{text}}" --yesno "{{message}}" {{height_in_chars}} {{width_in_chars}}
```
#### Display a text input box:
```shell
{{result_variable_name}}="$(whiptail --title "{{title}}" --inputbox "{{message}}" {{height_in_chars}} {{width_in_chars}} {{default_text}} 3>&1 1>&2 2>&3)"
```
#### Display a password input box:
```shell
{{result_variable_name}}="$(whiptail --title "{{title}}" --passwordbox "{{message}}" {{height_in_chars}} {{width_in_chars}} 3>&1 1>&2 2>&3)"
```
#### Display a multiple-choice menu:
```shell
{{result_variable_name}}=$(whiptail --title "{{title}}" --menu "{{message}}" {{height_in_chars}} {{width_in_chars}} {{menu_display_height}} "{{value_1}}" "{{display_text_1}}" "{{value_n}}" "{{display_text_n}}" ..... 3>&1 1>&2 2>&3)
```
{% endraw %}{% raw %}
<h2 id="wine">
  <a href="/en/linux/wine.html">wine</a> <a href="#wine"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run Windows programs on Unix.
> More information: <https://wiki.winehq.org/>.

#### Run `ipconfig.exe` program:
```shell
wine {{ipconfig}} {{/all}}
```
#### Run `cmd.exe` in background:
```shell
wine start {{cmd}}
```
#### Run Windows-like Package Manager:
```shell
wine uninstaller
```
#### Install MSI packages:
```shell
wine msiexec /i {{package}}
```
{% endraw %}{% raw %}
<h2 id="winetricks">
  <a href="/en/linux/winetricks.html">winetricks</a> <a href="#winetricks"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage Wine virtual Windows environments.
> More information: <https://wiki.winehq.org/Winetricks>.

#### Start a graphical setup at the default Wine location:
```shell
winetricks
```
#### Specify a custom Wine directory to run Winetricks in:
```shell
WINEPREFIX={{path/to/wine_directory}} winetricks
```
#### Install a Windows DLL or component to the default Wine directory:
```shell
winetricks {{package}}
```
{% endraw %}{% raw %}
<h2 id="wipefs">
  <a href="/en/linux/wipefs.html">wipefs</a> <a href="#wipefs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Wipe filesystem, raid, or partition-table signatures from a device.

#### Display signatures for specified device:
```shell
sudo wipefs {{/dev/sdX}}
```
#### Wipe all available signatures for specified device:
```shell
sudo wipefs --all {{/dev/sdX}}
```
#### Perform dry run:
```shell
sudo wipefs --all --no-act {{/dev/sdX}}
```
#### Force wipe, even if the filesystem is mounted:
```shell
sudo wipefs --all --force {{/dev/sdX}}
```
{% endraw %}{% raw %}
<h2 id="wmctrl">
  <a href="/en/linux/wmctrl.html">wmctrl</a> <a href="#wmctrl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI for X Window Manager.

#### List all windows, managed by the window manager:
```shell
wmctrl -l
```
#### Switch to the first window whose (partial) title matches:
```shell
wmctrl -a {{window_title}}
```
#### Move a window to the current workspace, raise it and give it focus:
```shell
wmctrl -R {{window_title}}
```
#### Switch to a workspace:
```shell
wmctrl -s {{workspace_number}}
```
#### Select a window and toggle fullscreen:
```shell
wmctrl -r {{window_title}} -b toggle,fullscreen
```
#### Select a window a move it to a workspace:
```shell
wmctrl -r {{window_title}} -t {{workspace_number}}
```
{% endraw %}{% raw %}
<h2 id="wodim">
  <a href="/en/linux/wodim.html">wodim</a> <a href="#wodim"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command (aliased as `cdrecord` on some systems) for recording data to CDs or DVDs.
> Some invocations of wodim can cause destructive actions, such as erasing all the data on a disc.

#### Display optical drives available to `wodim`:
```shell
wodim --devices
```
#### Record ("burn") an audio-only disc:
```shell
wodim dev=/dev/{{optical_drive}} -audio {{track*.cdaudio}}
```
#### Burn a file to a disc, ejecting the disc once done (some recorders require this):
```shell
wodim -eject dev=/dev/{{optical_drive}} -data {{file.iso}}
```
#### Burn a file to the disc in an optical drive, potentially writing to multiple discs in succession:
```shell
wodim -tao dev=/dev/{{optical_drive}} -data {{file.iso}}
```
{% endraw %}{% raw %}
<h2 id="wol">
  <a href="/en/linux/wol.html">wol</a> <a href="#wol"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Client for sending Wake-on-LAN magic packets.
> More information: <https://sourceforge.net/projects/wake-on-lan/>.

#### Send a WoL packet to a device:
```shell
wol {{mac_address}}
```
#### Send a WoL packet to a device in another subnet based on its IP:
```shell
wol --ipaddr={{ip_address}} {{mac_address}}
```
#### Send a WoL packet to a device in another subnet based on its hostname:
```shell
wol --host={{hostname}} {{mac_address}}
```
#### Send a WoL packet to a specific port on a host:
```shell
wol --port={{port_number}} {{mac_address}}
```
#### Read hardware addresses, IP addresses/hostnames, optional ports and SecureON passwords from a file:
```shell
wol --file={{path/to/file}}
```
#### Turn on verbose output:
```shell
wol --verbose {{mac_address}}
```
{% endraw %}{% raw %}
<h2 id="wpa_cli">
  <a href="/en/linux/wpa_cli.html">wpa_cli</a> <a href="#wpa_cli"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Add and configure wlan interfaces.

#### Scan for available networks:
```shell
wpa_cli scan
```
#### Show scan results:
```shell
wpa_cli scan_results
```
#### Add a network:
```shell
wpa_cli add_network {{number}}
```
#### Set a network's SSID:
```shell
wpa_cli set_network {{number}} ssid "{{SSID}}"
```
#### Enable network:
```shell
wpa_cli enable_network {{number}}
```
#### Save config:
```shell
wpa_cli save_config
```
{% endraw %}{% raw %}
<h2 id="wpa_passphrase">
  <a href="/en/linux/wpa_passphrase.html">wpa_passphrase</a> <a href="#wpa_passphrase"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate a WPA-PSK key from an ASCII passphrase for a given SSID.

#### Compute and display the WPA-PSK key for a given SSID reading the passphrase from stdin:
```shell
wpa_passphrase {{SSID}}
```
#### Compute and display WPA-PSK key for a given SSID specifying the passphrase as an argument:
```shell
wpa_passphrase {{SSID}} {{passphrase}}
```
{% endraw %}{% raw %}
<h2 id="wtf">
  <a href="/en/linux/wtf.html">wtf</a> <a href="#wtf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show the expansions of acronyms.
> More information: <https://manpages.debian.org/bsdgames/wtf.6.en.html>.

#### Expand a given acronym:
```shell
wtf {{IMO}}
```
#### Specify a computer related search type:
```shell
wtf -t {{comp}} {{WWW}}
```
{% endraw %}{% raw %}
<h2 id="x0vncserver">
  <a href="/en/linux/x0vncserver.html">x0vncserver</a> <a href="#x0vncserver"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> TigerVNC Server for X displays.
> More information: <https://tigervnc.org/doc/x0vncserver.html>.

#### Start a VNC server using a passwordfile:
```shell
x0vncserver -display {{:0}} -passwordfile {{path/to/file}}
```
#### Start a VNC server using a specific port:
```shell
x0vncserver -display {{:0}} -rfbport {{port}}
```
{% endraw %}{% raw %}
<h2 id="x11vnc">
  <a href="/en/linux/x11vnc.html">x11vnc</a> <a href="#x11vnc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A VNC server that will enable VNC on an existing display server.
> By default, the server will automatically terminate once all clients disconnect from it.

#### Launch a VNC server that allows multiple clients to connect:
```shell
x11vnc -shared
```
#### Launch a VNC server in view-only mode, and which won't terminate once the last client disconnects:
```shell
x11vnc -forever -viewonly
```
#### Launch a VNC server on a specific display and screen (both starting at index zero):
```shell
x11vnc -display :{{display}}.{{screen}}
```
#### Launch a VNC server on the third display's default screen:
```shell
x11vnc -display :{{2}}
```
#### Launch a VNC server on the first display's second screen:
```shell
x11vnc -display :{{0}}.{{1}}
```
{% endraw %}{% raw %}
<h2 id="xar">
  <a href="/en/linux/xar.html">xar</a> <a href="#xar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage .xar archives.

#### Create a xar archive of all files in a given directory:
```shell
xar -cf {{archive.xar}} {{path/to/directory}}
```
#### List the contents of a given xar archive:
```shell
xar -tf {{archive.xar}}
```
#### Extract the contents of a given xar archive to the current directory:
```shell
xar -xf {{archive.xar}}
```
{% endraw %}{% raw %}
<h2 id="xbacklight">
  <a href="/en/linux/xbacklight.html">xbacklight</a> <a href="#xbacklight"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility to adjust backlight brightness using the RandR extension.
> More information: <https://gitlab.freedesktop.org/xorg/app/xbacklight>.

#### Get the current screen brightness as a percentage:
```shell
xbacklight
```
#### Set the screen brightness to 40%:
```shell
xbacklight -set {{40}}
```
#### Increase current brightness by 25%:
```shell
xbacklight -inc {{25}}
```
#### Decrease current brightness by 75%:
```shell
xbacklight -dec {{75}}
```
#### Increase backlight to 100%, over 60 seconds (value given in ms), using 60 steps:
```shell
xbacklight -set {{100}} -time {{60000}} -steps {{60}}
```
{% endraw %}{% raw %}
<h2 id="xbps">
  <a href="/en/linux/xbps.html">xbps</a> <a href="#xbps"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The X Binary Package System (or xbps) is the binary package system used by Void Linux.
> More information: <https://github.com/void-linux/xbps>.

#### Install packages and synchronize them with the remote repository:
```shell
xbps-install --synchronize {{package_name1}} {{package_name2}}
```
#### Search for a package in the remote repository:
```shell
xbps-query --repository -s {{package_name}}
```
#### Remove a package, leaving all of its dependencies installed:
```shell
xbps-remove {{package_name}}
```
#### Remove a package and all of its dependencies recursively that are not required by other packages:
```shell
xbps-remove --recursive {{package_name}}
```
#### Synchronize your repository databases and update your system and dependencies:
```shell
xbps-install --synchronize -u
```
#### Remove packages that were installed as dependencies and aren't currently needed:
```shell
xbps-remove --remove-orphans
```
#### Remove obsolete packages from the cache:
```shell
xbps-remove --clean-cache
```
{% endraw %}{% raw %}
<h2 id="xclip">
  <a href="/en/linux/xclip.html">xclip</a> <a href="#xclip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> X11 clipboard manipulation tool, similar to `xsel`.
> Handles the X primary and secondary selections, plus the system clipboard (`Ctrl + C`/`Ctrl + V`).

#### Copy the output from a command to the X11 primary selection area (clipboard):
```shell
echo 123 | xclip
```
#### Copy the output from a command to a given X11 selection area:
```shell
echo 123 | xclip -selection {{primary|secondary|clipboard}}
```
#### Copy the output from a command to the system clipboard, using short notation:
```shell
echo 123 | xclip -sel clip
```
#### Copy the contents of a file into the system clipboard:
```shell
xclip -sel clip {{input_file.txt}}
```
#### Copy the contents of a PNG image into the system clipboard (can be pasted in other programs correctly):
```shell
xclip -sel clip -t image/png {{input_file.png}}
```
#### Copy the user input in the console into the system clipboard:
```shell
xclip -i
```
#### Paste the contents of the X11 primary selection area to the console:
```shell
xclip -o
```
#### Paste the contents of the system clipboard to the console:
```shell
xclip -o -sel clip
```
{% endraw %}{% raw %}
<h2 id="xclock">
  <a href="/en/linux/xclock.html">xclock</a> <a href="#xclock"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display the time in analog or digital form.

#### Display an analog clock:
```shell
xclock
```
#### Display a 24-hour digital clock with the hour and minute fields only:
```shell
xclock -digital -brief
```
#### Display a digital clock using an strftime format string (see strftime(3)):
```shell
xclock -digital -strftime {{format}}
```
#### Display a 24-hour digital clock with the hour, minute and second fields that updates every second:
```shell
xclock -digital -strftime '%H:%M:%S' -update 1
```
#### Display a 12-hour digital clock with the hour and minute fields only:
```shell
xclock -digital -twelve -brief
```
{% endraw %}{% raw %}
<h2 id="xcursorgen">
  <a href="/en/linux/xcursorgen.html">xcursorgen</a> <a href="#xcursorgen"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create an X cursor file from a collection of PNG images.
> If `--prefix` is omitted, the image files must be located in the current working directory.
> More information: <https://manned.org/xcursorgen.1>.

#### Create an X cursor file using a config file:
```shell
xcursorgen {{path/to/config.cursor}} {{path/to/output_file}}
```
#### Create an X cursor file using a config file and specify the path to the image files:
```shell
xcursorgen --prefix {{path/to/image_directory/}} {{path/to/config.cursor}} {{path/to/output_file}}
```
#### Create an X cursor file using a config file and write the output to stdout:
```shell
xcursorgen {{path/to/config.cursor}}
```
{% endraw %}{% raw %}
<h2 id="xdg-mime">
  <a href="/en/linux/xdg-mime.html">xdg-mime</a> <a href="#xdg-mime"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Query and manage MIME types according to the XDG standard.
> More information: <https://portland.freedesktop.org/doc/xdg-mime.html>.

#### Display the MIME type of a file:
```shell
xdg-mime query filetype {{path/to/file}}
```
#### Display the default application for opening PNG images:
```shell
xdg-mime query default {{image/png}}
```
#### Display the default application for opening a specific file:
```shell
xdg-mime query default $(xdg-mime query filetype {{path/to/file}})
```
#### Set imv as the default application for opening PNG and JPEG images:
```shell
xdg-mime default {{imv.desktop}} {{image/png}} {{image/jpeg}}
```
{% endraw %}{% raw %}
<h2 id="xdg-open">
  <a href="/en/linux/xdg-open.html">xdg-open</a> <a href="#xdg-open"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Opens a file or URL in the user's preferred application.
> More information: <https://man.archlinux.org/man/xdg-open.1>.

#### Open the current directory in the default file explorer:
```shell
xdg-open .
```
#### Open an URL in the default browser:
```shell
xdg-open {{https://example.com}}
```
#### Open an image in the default image viewer:
```shell
xdg-open {{path/to/image}}
```
#### Open a PDF in the default PDF viewer:
```shell
xdg-open {{path/to/pdf}}
```
#### Display help:
```shell
xdg-open --help
```
{% endraw %}{% raw %}
<h2 id="xdotool">
  <a href="/en/linux/xdotool.html">xdotool</a> <a href="#xdotool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line automation for X11.

#### Retrieve the X-Windows window ID of the running Firefox window(s):
```shell
xdotool search --onlyvisible --name {{firefox}}
```
#### Click the right mouse button:
```shell
xdotool click {{3}}
```
#### Get the id of the currently active window:
```shell
xdotool getactivewindow
```
#### Focus on the window with id of 12345:
```shell
xdotool windowfocus --sync {{12345}}
```
#### Type a message, with a 500ms delay for each letter:
```shell
xdotool type --delay {{500}} "Hello world"
```
#### Press the enter key:
```shell
xdotool key {{KP_Enter}}
```
{% endraw %}{% raw %}
<h2 id="xeyes">
  <a href="/en/linux/xeyes.html">xeyes</a> <a href="#xeyes"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display eyes on the screen that follow the mouse cursor.

#### Launch xeyes on the local machine's default display:
```shell
xeyes
```
#### Launch xeyes on a remote machine's display 0, screen 0:
```shell
xeyes -display {{remote_host}}:{{0}}.{{0}}
```
{% endraw %}{% raw %}
<h2 id="xfce4-screenshooter">
  <a href="/en/linux/xfce4-screenshooter.html">xfce4-screenshooter</a> <a href="#xfce4-screenshooter"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The XFCE4 screenshot tool.
> More information: <https://docs.xfce.org/apps/xfce4-screenshooter/start>.

#### Launch the screenshooter GUI:
```shell
xfce4-screenshooter
```
#### Take a screenshot of the entire screen and launch the GUI to ask how to proceed:
```shell
xfce4-screenshooter --fullscreen
```
#### Take a screenshot of the entire screen and save it in the specified directory:
```shell
xfce4-screenshooter --fullscreen --save {{path/to/directory}}
```
#### Wait some time before taking the screenshot:
```shell
xfce4-screenshooter --delay {{seconds}}
```
#### Take a screenshot of a region of the screen (select using the mouse):
```shell
xfce4-screenshooter --region
```
#### Take a screenshot of the active window, and copy it to the clipboard:
```shell
xfce4-screenshooter --window --clipboard
```
#### Take a screenshot of the active window, and open it with a chosen program:
```shell
xfce4-screenshooter --window --open {{gimp}}
```
{% endraw %}{% raw %}
<h2 id="xfce4-terminal">
  <a href="/en/linux/xfce4-terminal.html">xfce4-terminal</a> <a href="#xfce4-terminal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The XFCE4 terminal emulator.
> More information: <https://docs.xfce.org/apps/xfce4-terminal/start>.

#### Open a new terminal window:
```shell
xfce4-terminal
```
#### Set the initial title:
```shell
xfce4-terminal --initial-title "{{initial_title}}"
```
#### Open a new tab in the current terminal window:
```shell
xfce4-terminal --tab
```
#### Execute a command in a new terminal window:
```shell
xfce4-terminal --command "{{command_with_args}}"
```
#### Keep the terminal around after the executed command finishes executing:
```shell
xfce4-terminal --command "{{command_with_args}}" --hold
```
#### Open multiple new tabs, executing a command in each:
```shell
xfce4-terminal --tab --command "{{command_a}}" --tab --command "{{command_b}}"
```
{% endraw %}{% raw %}
<h2 id="xinput">
  <a href="/en/linux/xinput.html">xinput</a> <a href="#xinput"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List available input devices, query information about a device and change input device settings.

#### List all input devices:
```shell
xinput list
```
#### Disable an input:
```shell
xinput disable {{id}}
```
#### Enable an input:
```shell
xinput enable {{id}}
```
#### Disconnect an input from its master:
```shell
xinput float {{id}}
```
#### Reattach an input as slave to a master:
```shell
xinput reattach {{id}} {{master_id}}
```
{% endraw %}{% raw %}
<h2 id="xman">
  <a href="/en/linux/xman.html">xman</a> <a href="#xman"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manual page viewer for X Window System.

#### Start xman in three-button window:
```shell
xman
```
#### Open the manual page output stored in a given file:
```shell
xman -helpfile {{filename}}
```
#### Show both manual page and directory:
```shell
xman -bothshown
```
{% endraw %}{% raw %}
<h2 id="xmount">
  <a href="/en/linux/xmount.html">xmount</a> <a href="#xmount"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Convert on-the-fly between multiple input and output hard disk image types with optional write cache support.
> Creates a virtual file system using FUSE (Filesystem in Userspace) that contains a virtual representation of the input image.
> More information: <https://manned.org/xmount>.

#### Mount a `.raw` image file into a DMG container file:
```shell
xmount --in {{raw}} {{path/to/image.dd}} --out {{dmg}} {{mountpoint}}
```
#### Mount an EWF image file with write-cache support into a VHD file to boot from:
```shell
xmount --cache {{path/to/cache.ovl}} --in {{ewf}} {{path/to/image.E??}} --out {{vhd}} {{mountpoint}}
```
#### Mount the first partition at sector 2048 into a new `.raw` image file:
```shell
xmount --offset {{2048}} --in {{raw}} {{path/to/image.dd}} --out {{raw}} {{mountpoint}}
```
{% endraw %}{% raw %}
<h2 id="xrandr">
  <a href="/en/linux/xrandr.html">xrandr</a> <a href="#xrandr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Set the size, orientation and/or reflection of the outputs for a screen.

#### Display the current state of the system (known screens, resolutions, ...):
```shell
xrandr --query
```
#### Disable disconnected outputs and enable connected ones with default settings:
```shell
xrandr --auto
```
#### Change the resolution and update frequency of DisplayPort 1 to 1920x1080, 60Hz:
```shell
xrandr --output {{DP1}} --mode {{1920x1080}} --rate {{60}}
```
#### Set the resolution of HDMI2 to 1280x1024 and put it on the right of DP1:
```shell
xrandr --output {{HDMI2}} --mode {{1280x1024}} --right-of {{DP1}}
```
#### Disable the VGA1 output:
```shell
xrandr --output {{VGA1}} --off
```
#### Set brightness for LVDS1 to 50%:
```shell
xrandr --output {{LVDS1}} --brightness {{0.5}}
```
#### See display hardware information:
```shell
xrandr -q
```
{% endraw %}{% raw %}
<h2 id="xsel">
  <a href="/en/linux/xsel.html">xsel</a> <a href="#xsel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> X11 selection and clipboard manipulation tool.

#### Use a command's output as input of the clip[b]oard (equivalent to `Ctrl + C`):
```shell
echo 123 | xsel -ib
```
#### Use the contents of a file as input of the clipboard:
```shell
cat {{file}} | xsel -ib
```
#### Output the clipboard's contents into the terminal (equivalent to `Ctrl + V`):
```shell
xsel -ob
```
#### Output the clipboard's contents into a file:
```shell
xsel -ob > {{file}}
```
#### Clear the clipboard:
```shell
xsel -cb
```
#### Output the X11 primary selection's contents into the terminal (equivalent to a mouse middle-click):
```shell
xsel -op
```
{% endraw %}{% raw %}
<h2 id="xsetwacom">
  <a href="/en/linux/xsetwacom.html">xsetwacom</a> <a href="#xsetwacom"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line tool to change settings for Wacom pen tablets at runtime.

#### List all the available wacom devices. The device name is in the first column:
```shell
xsetwacom list
```
#### Set Wacom area to specific screen. Get name of the screen with `xrandr`:
```shell
xsetwacom set "{{device_name}}" MapToOutput {{screen}}
```
#### Set mode to relative (like a mouse) or absolute (like a pen) mode:
```shell
xsetwacom set "{{device_name}}" Mode "{{Relative|Absolute}}"
```
#### Rotate the input (useful for tablet-PC when rotating screen) by 0|90|180|270 degrees from "natural" rotation:
```shell
xsetwacom set "{{device_name}}" Rotate {{none|half|cw|ccw}}
```
#### Set button to only work when the tip of the pen is touching the tablet:
```shell
xsetwacom set "{{device_name}}" TabletPCButton "on"
```
{% endraw %}{% raw %}
<h2 id="xterm">
  <a href="/en/linux/xterm.html">xterm</a> <a href="#xterm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A terminal emulator for the X Window System.

#### Open the terminal with a title of `Example`:
```shell
xterm -T {{Example}}
```
#### Open the terminal in fullscreen mode:
```shell
xterm -fullscreen
```
#### Open the terminal with a dark blue background and yellow foreground (font color):
```shell
xterm -bg {{darkblue}} -fg {{yellow}}
```
#### Open the terminal with 100 characters per line and 35 lines, in screen position x=200px, y=20px:
```shell
xterm -geometry {{100}}x{{35}}+{{200}}+{{20}}
```
#### Open the terminal using a Serif font and a font size equal to 20:
```shell
xterm -fa {{'Serif'}} -fs {{20}}
```
{% endraw %}{% raw %}
<h2 id="xtrlock">
  <a href="/en/linux/xtrlock.html">xtrlock</a> <a href="#xtrlock"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lock the X display until the user supplies their password.

#### Lock the display and show a padlock instead of the cursor:
```shell
xtrlock
```
#### Display a blank screen as well as the padlock cursor:
```shell
xtrlock -b
```
#### Fork the xtrlock process and return immediately:
```shell
xtrlock -f
```
{% endraw %}{% raw %}
<h2 id="xvfb-run">
  <a href="/en/linux/xvfb-run.html">xvfb-run</a> <a href="#xvfb-run"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run a command in a virtual X server environment.
> More information: <https://www.x.org/wiki/>.

#### Run the specified command in a virtual X server:
```shell
xvfb-run {{command}}
```
#### Try to get a free server number, if the default (99) is not available:
```shell
xvfb-run --auto-servernum {{command}}
```
#### Pass arguments to the Xvfb server:
```shell
xvfb-run --server-args "{{-screen 0 1024x768x24}}" {{command}}
```
{% endraw %}{% raw %}
<h2 id="yank">
  <a href="/en/linux/yank.html">yank</a> <a href="#yank"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Read input from stdin and display a selection interface that allows a field to be selected and copied to the clipboard.

#### Yank using the default delimiters (\f, \n, \r, \s, \t):
```shell
{{sudo dmesg}} | yank
```
#### Yank an entire line:
```shell
{{sudo dmesg}} | yank -l
```
#### Yank using a specific delimiter:
```shell
{{echo hello=world}} | yank -d {{=}}
```
#### Only yank fields matching a specific pattern:
```shell
{{ps ux}} | yank -g "{{[0-9]+}}"
```
{% endraw %}{% raw %}
<h2 id="yaourt">
  <a href="/en/linux/yaourt.html">yaourt</a> <a href="#yaourt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux utility for building packages from the Arch User Repository.

#### Synchronize and update all packages (including AUR):
```shell
yaourt -Syua
```
#### Install a new package (includes AUR):
```shell
yaourt -S {{package_name}}
```
#### Remove a package and its dependencies (includes AUR packages):
```shell
yaourt -Rs {{package_name}}
```
#### Search the package database for a keyword (including AUR):
```shell
yaourt -Ss {{package_name}}
```
#### List installed packages, versions, and repositories (AUR packages will be listed under the repository name 'local'):
```shell
yaourt -Q
```
{% endraw %}{% raw %}
<h2 id="yay">
  <a href="/en/linux/yay.html">yay</a> <a href="#yay"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Yet Another Yogurt: A utility for Arch Linux to build and install packages from the Arch User Repository.
> Also see `pacman`.
> More information: <https://github.com/Jguer/yay>.

#### Interactively search and install packages from the repos and AUR:
```shell
yay {{package_name|search_term}}
```
#### Synchronize and update all packages from the repos and AUR:
```shell
yay
```
#### Synchronize and update only AUR packages:
```shell
yay -Sua
```
#### Install a new package from the repos and AUR:
```shell
yay -S {{package_name}}
```
#### Remove an installed package and both its dependencies and configuration files:
```shell
yay -Rns {{package_name}}
```
#### Search the package database for a keyword from the repos and AUR:
```shell
yay -Ss {{keyword}}
```
#### Show statistics for installed packages and system health:
```shell
yay -Ps
```
{% endraw %}{% raw %}
<h2 id="yetris">
  <a href="/en/linux/yetris.html">yetris</a> <a href="#yetris"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Clone of the game Tetris in the terminal.
> More information: <https://github.com/alexdantas/yetris>.

#### Start a tetris game:
```shell
yetris
```
#### Navigate the piece horizontally:
```shell
{{Left|Right}} arrow key
```
#### Rotate the piece clockwise or counterclockwise:
```shell
{{x|z}}
```
#### Hold a piece (only one allowed at a time):
```shell
c
```
#### Soft drop the piece:
```shell
Down arrow key
```
#### Hard drop the piece:
```shell
Spacebar
```
#### Pause/unpause the game:
```shell
p
```
#### Quit the game:
```shell
q
```
{% endraw %}{% raw %}
<h2 id="yum">
  <a href="/en/linux/yum.html">yum</a> <a href="#yum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Package management utility for RHEL, Fedora, and CentOS (for older versions).
> More information: <https://man7.org/linux/man-pages/man8/yum.8.html>.

#### Install a new package:
```shell
yum install {{package}}
```
#### Install a new package and assume yes to all questions (also works with update, great for automated updates):
```shell
yum -y install {{package}}
```
#### Find the package that provides a particular command:
```shell
yum provides {{command}}
```
#### Remove a package:
```shell
yum remove {{package}}
```
#### Display available updates for installed packages:
```shell
yum check-update
```
#### Upgrade installed packages to newest available versions:
```shell
yum upgrade
```
{% endraw %}{% raw %}
<h2 id="zenity">
  <a href="/en/linux/zenity.html">zenity</a> <a href="#zenity"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display dialogs from the command-line/shell scripts.
> Return user-inserted values or 1 if error.

#### Display the default question dialog:
```shell
zenity --question
```
#### Display an info dialog displaying the text "Hello!":
```shell
zenity --info --text="{{Hello!}}"
```
#### Display a name/password form and output the data separated by ";":
```shell
zenity --forms --add-entry="{{Name}}" --add-password="{{Password}}" --separator="{{;}}"
```
#### Display a file selection form in which the user can only select directories:
```shell
zenity --file-selection --directory
```
#### Display a progress bar which updates its message every second and show a progress percent:
```shell
{{(echo "#1"; sleep 1; echo "50"; echo "#2"; sleep 1; echo "100")}} | zenity --progress
```
{% endraw %}{% raw %}
<h2 id="zgrep">
  <a href="/en/linux/zgrep.html">zgrep</a> <a href="#zgrep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Grep text patterns from files within compressed file (equivalent to grep -Z).

#### Grep a pattern in a compressed file (case-sensitive):
```shell
zgrep {{pattern}} {{path/to/compressed/file}}
```
#### Grep a pattern in a compressed file (case-insensitive):
```shell
zgrep -i {{pattern}} {{path/to/compressed/file}}
```
#### Output count of lines containing matched pattern in a compressed file:
```shell
zgrep -c {{pattern}} {{path/to/compressed/file}}
```
#### Display the lines which don’t have the pattern present (Invert the search function):
```shell
zgrep -v {{pattern}} {{path/to/compressed/file}}
```
#### Grep a compressed file for multiple patterns:
```shell
zgrep -e "{{pattern_1}}" -e "{{pattern_2}}" {{path/to/compressed/file}}
```
#### Use extended regular expressions (supporting `?`, `+`, `{}`, `()` and `|`):
```shell
zgrep -E {{regular_expression}} {{path/to/file}}
```
#### Print 3 lines of [C]ontext around, [B]efore, or [A]fter each match:
```shell
zgrep -{{C|B|A}} {{3}} {{pattern}} {{path/to/compressed/file}}
```
{% endraw %}{% raw %}
<h2 id="zile">
  <a href="/en/linux/zile.html">zile</a> <a href="#zile"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Zile is a lightweight clone of the Emacs text editor.
> More information: <https://www.gnu.org/software/zile/>.

#### Start a buffer for temporary notes, which won't be saved:
```shell
zile
```
#### Open a file:
```shell
zile {{path/to/file}}
```
#### Save a file:
```shell
Ctrl + X, Ctrl + S
```
#### Quit:
```shell
Ctrl + X, Ctrl + C
```
#### Open a file at a specified line number:
```shell
zile +{{line_number}} {{path/to/file}}
```
#### Undo changes:
```shell
Ctrl + X, U
```
{% endraw %}{% raw %}
<h2 id="zramctl">
  <a href="/en/linux/zramctl.html">zramctl</a> <a href="#zramctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Setup and control zram devices.
> Use `mkfs` or `mkswap` to format zram devices to partitions.

#### Check if zram is enabled:
```shell
lsmod | grep -i zram
```
#### Enable zram with a dynamic number of devices (use `zramctl` to configure devices further):
```shell
sudo modprobe zram
```
#### Enable zram with exactly 2 devices:
```shell
sudo modprobe zram num_devices={{2}}
```
#### Find and initialise the next free zram device to a 2GB virtual drive using LZ4 compression:
```shell
sudo zramctl --find --size {{2GB}} --algorithm {{lz4}}
```
#### List currently initialised devices:
```shell
zramctl
```
{% endraw %}{% raw %}
<h2 id="zypper">
  <a href="/en/linux/zypper.html">zypper</a> <a href="#zypper"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> SUSE & openSUSE package management utility.

#### Synchronize list of packages and versions available:
```shell
zypper refresh
```
#### Install a new package:
```shell
zypper install {{package}}
```
#### Remove a package:
```shell
zypper remove {{package}}
```
#### Upgrade installed packages to newest available versions:
```shell
zypper update
```
#### Search package via keyword:
```shell
zypper search {{keyword}}
```
{% endraw %}