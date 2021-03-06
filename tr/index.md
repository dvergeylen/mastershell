---
layout: default
title: "TR"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#common">Common</a>
  * <a href="#7z">7z</a>
  * <a href="#base32">base32</a>
  * <a href="#base64">base64</a>
  * <a href="#chroot">chroot</a>
  * <a href="#cmake">cmake</a>
  * <a href="#command">command</a>
  * <a href="#dirname">dirname</a>
  * <a href="#dirs">dirs</a>
  * <a href="#dirsearch">dirsearch</a>
  * <a href="#docker">docker</a>
  * <a href="#docker-build">docker build</a>
  * <a href="#docker-compose">docker compose</a>
  * <a href="#docker-exec">docker exec</a>
  * <a href="#docker-images">docker images</a>
  * <a href="#docker-inspect">docker inspect</a>
  * <a href="#docker-logs">docker logs</a>
  * <a href="#docker-network">docker network</a>
  * <a href="#docker-ps">docker ps</a>
  * <a href="#docker-rmi">docker rmi</a>
  * <a href="#docker-run">docker run</a>
  * <a href="#docker-save">docker save</a>
  * <a href="#docker-secret">docker secret</a>
  * <a href="#docker-service">docker service</a>
  * <a href="#docker-start">docker start</a>
  * <a href="#docker-stats">docker stats</a>
  * <a href="#docker-swarm">docker swarm</a>
  * <a href="#docker-system">docker system</a>
  * <a href="#docker-machine">docker-machine</a>
  * <a href="#man">man</a>
  * <a href="#minetest">minetest</a>
  * <a href="#minetestserver">minetestserver</a>
  * <a href="#tldr">tldr</a>
  * <a href="#tldr-lint">tldr-lint</a>
  * <a href="#tldrl">tldrl</a>

* <a href="#linux">Linux</a>
  * <a href="#apt-get">apt-get</a>
  * <a href="#aptitude">aptitude</a>
  * <a href="#pacman">pacman</a>
  * <a href="#pacman---query">pacman --query</a>
  * <a href="#pacman---remove">pacman --remove</a>
  * <a href="#pacman---sync">pacman --sync</a>
  * <a href="#pacman-mirrors">pacman-mirrors</a>
  * <a href="#pulseaudio">pulseaudio</a>
  * <a href="#tree">tree</a>
  * <a href="#xeyes">xeyes</a>
  * <a href="#xfce4-screenshooter">xfce4-screenshooter</a>
  * <a href="#xfce4-terminal">xfce4-terminal</a>
  * <a href="#xterm">xterm</a>


# Linux
{% raw %}
<h2 id="apt-get">
  <a href="/tr/linux/apt-get.html">apt-get</a> <a href="#apt-get"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Debian ve Ubuntu paket y??netim arac??.
> Paket aramak i??in `apt-cache` komutunu kullan??n.
> Daha fazla bilgi i??in: <https://manpages.debian.org/latest/apt/apt-get.8.html>.

#### Kullan??labilir paket ve versiyon listesini g??ncelleyin (di??er `apt-get` komutlar??n?? ??al????t??rmadan ??nce kullanman??z ??nerilir):
```shell
apt-get update
```
#### Bir paket y??kleyin veya son s??r??me g??ncelleyin:
```shell
apt-get install {{paket}}
```
#### Bir paketi silin:
```shell
apt-get remove {{paket}}
```
#### Bir paketi ve konfig??rasyon dosyalar??n?? silin:
```shell
apt-get purge {{paket}}
```
#### Y??kl?? paketlerin hepsini son s??r??mlerine y??kseltin:
```shell
apt-get upgrade
```
#### Yerel depoyu temizleyin - kullan??lmayan gereksiz paket dosyalar??n?? (.deb) silin:
```shell
apt-get autoclean
```
#### Art??k gerekmeyen paketleri silin:
```shell
apt-get autoremove
```
#### Y??klenmi?? paketleri y??kseltin (`upgrade` gibi), ancak gereksiz paketleri silin ve yeni ba????ml??l??klar?? memnun edecek ek paketler kurun:
```shell
apt-get dist-upgrade
```
{% endraw %}{% raw %}
<h2 id="aptitude">
  <a href="/tr/linux/aptitude.html">aptitude</a> <a href="#aptitude"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Debian ve Ubuntu paket y??netim arac??.
> Daha fazla bilgi i??in: <https://manpages.debian.org/latest/aptitude/aptitude.8.html>.

#### Kullan??labilir paket ve s??r??m listesini senkronize et. Bu, herhangi bir aptitude komutunu uygulamadan ??nce ??al????t??r??lmal??d??r:
```shell
aptitude update
```
#### Yeni bir paket ve onun ba????ml??l??klar??n?? kur:
```shell
aptitude install {{paket}}
```
#### Paket ara:
```shell
aptitude search {{paket}}
```
#### ??ndirilmi?? bir paket ara: (`?installed` bir aptitude arama ifadesidir):
```shell
aptitude search '?installed({{paket}})'
```
#### Bir paket ve onun ba????ml??l??klar??n?? kald??r:
```shell
aptitude remove {{paket}}
```
#### Y??kl?? paketleri son kullan??labilir s??r??mlerine y??kselt:
```shell
aptitude upgrade
```
#### Y??kl?? paketleri y??kle (`aptitude upgrade` gibi), gereksizleri sil ve yeni ba????ml??l??klar?? kar????lamak ??zere ek paketler kur:
```shell
aptitude full-upgrade
```
#### Bir paketin otomatik y??kseltilmesini engellemek i??in onu beklemede tut:
```shell
aptitude hold '?installed({{paket}})'
```
{% endraw %}{% raw %}
<h2 id="pacman-mirrors">
  <a href="/tr/linux/pacman-mirrors.html">pacman-mirrors</a> <a href="#pacman-mirrors"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manjaro Linux i??in pacman aynalistesi olu??turucu.
> pacman-mirrors'??n ??al????t??r??ld?????? her vakit, E`sudo pacman -Syyu` komutu ile veritaban??n??n senkronize edilmesi ve sistemin g??ncellenmesi gerekir.
> Daha fazla bilgi i??in: <https://wiki.manjaro.org/index.php?title=Pacman-mirrors>.

#### Varsay??lan ayarlar ile bir aynalistesi olu??tur:
```shell
sudo pacman-mirrors --fasttrack
```
#### Mevcut aynalar??n durumunu g??ster:
```shell
pacman-mirrors --status
```
#### Mevcut dal?? g??ster:
```shell
pacman-mirrors --get-branch
```
#### Farkl?? bir dala ge??:
```shell
sudo pacman-mirrors --api --set-branch {{stabil|instabil|test_ediliyor}}
```
#### Sadece IP adresinin bulundu??u ??lkenin aynalar??n?? kullanarak bir aynalistesi olu??tur:
```shell
sudo pacman-mirrors --geoip
```
{% endraw %}{% raw %}
<h2 id="pacman---query">
  <a href="/tr/linux/pacman-query.html">pacman --query</a> <a href="#pacman---query"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux paket y??netim arac??.
> Daha fazla bilgi i??in: <https://man.archlinux.org/man/pacman.8>.

#### Y??klenmi?? paket ve s??r??mleri s??rala:
```shell
pacman --query
```
#### Sadece ??zellikle indirilmi?? paket ve s??r??mleri s??rala:
```shell
pacman --query --explicit
```
#### Hangi paketin belirtilen dosyaya sahip oldu??unu bul:
```shell
pacman --query --owns {{dosya_ismi}}
```
#### ??ndirilmi?? bir pakete dair bilgiyi g??r??nt??le:
```shell
pacman --query --info {{paket_ismi}}
```
#### Bir paketin i??erdi??i dosyalar?? s??rala:
```shell
pacman --query --list {{paket_ismi}}
```
#### Yetim (ba??ka bir pakete ba??l??l??k olarak indirilmi?? ancak herhangi bir paket taraf??ndan gerektirilmeyen) paketleri s??rala:
```shell
pacman --query --unrequired --deps --quiet
```
#### Mevcut depolarda bulunmayan, indirilmi?? paketleri s??rala:
```shell
pacman --query --foreign
```
#### Miad?? dolmu?? paketleri s??rala:
```shell
pacman --query --upgrades
```
{% endraw %}{% raw %}
<h2 id="pacman---remove">
  <a href="/tr/linux/pacman-remove.html">pacman --remove</a> <a href="#pacman---remove"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux paket y??netim arac??.
> Daha fazla bilgi i??in: <https://man.archlinux.org/man/pacman.8>.

#### Bu alt komut i??in yard??m g??ster:
```shell
pacman --remove --help
```
#### Bir paket ve ba??l??l??klar??n?? sil:
```shell
sudo pacman --remove --recursive {{paket_ismi}}
```
#### Bir paketi ve onun hem ba??l??l??klar??n??, hem de konfig??rasyon dosyalar??n?? sil:
```shell
sudo pacman --remove --recursive --nosave {{paket_ismi}}
```
#### Bir paketi telkin olmaks??z??n sil:
```shell
sudo pacman --remove --noconfirm {{paket_ismi}}
```
#### Yetim (ba??ka bir pakete ba??l??l??k olarak indirilmi?? ancak herhangi bir paket taraf??ndan gerektirilmeyen) paketleri sil:
```shell
sudo pacman --remove --recursive --nosave $(pacman --query --unrequired --deps --quiet)
```
#### Bir paketi ve ona ba??l?? olan t??m ??b??r paketleri sil:
```shell
sudo pacman --remove --cascade {{paket_ismi}}
```
#### (Bir paketin silinme durumunda) Etkilenecek paketleri (silmeden) listele:
```shell
pacman --remove --print {{paket_ismi}}
```
{% endraw %}{% raw %}
<h2 id="pacman---sync">
  <a href="/tr/linux/pacman-sync.html">pacman --sync</a> <a href="#pacman---sync"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux paket y??netim arac??.
> Daha fazla bilgi i??in: <https://man.archlinux.org/man/pacman.8>.

#### Yeni bir paket indir::
```shell
sudo pacman --sync {{paket_ismi}}
```
#### T??m paketleri senkronize et ve g??ncelle (bahsi ge??en paketleri g??ncellemeden indirmek i??in `--downloadonly` eki gereklidir)
```shell
sudo pacman --sync --refresh --sysupgrade
```
#### T??m paketleri g??ncelle ve telkin olmaks??z??n yeni bir tane indir:
```shell
sudo pacman --sync --refresh --sysupgrade --noconfirm {{paket_ismi}}
```
#### Paket veritaban??n?? girilen ifade ile arat:
```shell
pacman --sync --search "{{arama_??ablonu}}"
```
#### Bir paket hakk??nda bilgi g??r??nt??le:
```shell
pacman --sync --info {{paket_ismi}}
```
#### Bir paket g??ncellemesi s??ras??nda ??ak????an dosyalar??n ??st??ne yaz:
```shell
sudo pacman --sync --refresh --sysupgrade --overwrite {{??rnek_dosya}}
```
#### T??m paketleri senkronize et ve g??ncelle, ancak belli bir paketi yoksay:
```shell
sudo pacman --sync --refresh --sysupgrade --ignore {{paket_ismi}}
```
#### Kullan??lmayan paket ve kullan??lmam???? depolar?? ??erezlerden sil (t??m paketlerin ??erezlerini temizlemek i??in `--clean` eki iki kez kullan??lmal??d??r):
```shell
sudo pacman --sync --clean
```
{% endraw %}{% raw %}
<h2 id="pacman">
  <a href="/tr/linux/pacman.html">pacman</a> <a href="#pacman"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux paket y??netim arac??.
> Daha fazla bilgi i??in: <https://man.archlinux.org/man/pacman.8>.

#### T??m paketleri senkronize et ve g??ncelle:
```shell
pacman -Syu
```
#### Yeni bir paket indir:
```shell
pacman -S {{paket_ismi}}
```
#### Bir paket ve ba??l??l??klar??n?? sil:
```shell
pacman -Rs {{paket_ismi}}
```
#### Paket veritaban??n?? girilen ifade ile arat:
```shell
pacman -Ss "{{arama_??ablonu}}"
```
#### ??ndirilmi?? paket ve s??r??mleri s??rala:
```shell
pacman -Q
```
#### Sadece ??zellikle belirtilen paket ve s??r??mleri s??rala:
```shell
pacman -Qe
```
#### Hangi paketin belirtilen dosyaya sahip oldu??unu bul:
```shell
pacman -Qo {{dosya_ismi}}
```
#### Paket ??erezlerini bo?? alan a??mak i??in temizle:
```shell
pacman -Scc
```
{% endraw %}{% raw %}
<h2 id="pulseaudio">
  <a href="/tr/linux/pulseaudio.html">pulseaudio</a> <a href="#pulseaudio"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ses sistem arkaplan uygulamas?? ve y??neticisi.
> Daha fazla bilgi i??in: <https://www.freedesktop.org/wiki/Software/PulseAudio/>.

#### Pulseaudio'nun ??al??????p ??al????mad??????n?? kontrol et (s??f??r olmayan ????kt??, ??al????mad?????? anlam??na gelir):
```shell
pulseaudio --check
```
#### Pulseaudio'yu arkaplanda ??al????t??r:
```shell
pulseaudio --start
```
#### Arkaplanda ??al????an t??m pulseaudio uygulamalar??n?? ??ld??r:
```shell
pulseaudio --kill
```
#### M??sait mod??lleri s??rala:
```shell
pulseaudio --dump-modules
```
#### Belirtilen arg??manlarla bir mod??l?? mevcut ??al????an arkaplan uygulamas??na y??kle:
```shell
pulseaudio --load="{{mod??l_ismi}} {{arg??manlar}}"
```
{% endraw %}{% raw %}
<h2 id="tree">
  <a href="/tr/linux/tree.html">tree</a> <a href="#tree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mevcut dizinin i??eri??ini a??a?? bi??iminde g??ster.
> Daha fazla bilgi i??in: <http://mama.indstate.edu/users/ice/tree/>.

#### Dosya ve dizinleri `num` de??eri kadar derinlikte g??ster (1 olmas?? durumunda mevcut dizin g??sterilir):
```shell
tree -L {{num}}
```
#### Yaln??zca dizinleri g??ster:
```shell
tree -d
```
#### Renklendirme a????k olacak ??ekilde gizli dosyalar?? dahi g??ster:
```shell
tree -a -C
```
#### A??ac??n sat??rlar??n?? girintiler yerine t??m yolu belirterek g??ster:
```shell
tree -i -f
```
#### T??m dosyalar??n ve dizinlerin eklenerek artan boyutlar??n??, insanlar??n okuyabilece??i bir bi??imde g??ster:
```shell
tree -s -h --du
```
#### A??a?? hiyerar??isi i??indeki dosyalar?? bir wildcard (glob) kal??b?? kullanarak ve aranan ??zellikteki dosyalara sahip olmayan dizinleri yoksayarak g??ster:
```shell
tree -P '{{*.txt}}' --prune
```
#### A??a?? hiyerar??isi i??indeki dizinleri bir wildcard (glob) kal??b?? kullanarak ve istenen dizine atal?????? olmayan dizinleri yoksayarak g??ster:
```shell
tree -P {{dizin_ismi}} --matchdirs --prune
```
#### A??ac?? belirtilen dizinleri yoksayarak g??ster:
```shell
tree -I '{{dizin_ismi1|dizin_ismi2}}'
```
{% endraw %}{% raw %}
<h2 id="xeyes">
  <a href="/tr/linux/xeyes.html">xeyes</a> <a href="#xeyes"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ekranda fare imlecini takip eden bir ??ift g??z g??ster.

#### Xeyes'?? yerel makinenin varsay??lan ekran??nda ba??lat:
```shell
xeyes
```
#### Xeyes'?? uzak bir makinenin 0. g??r??nt?? ve 0. ekran koordinatlar??nda ba??lat:
```shell
xeyes -display {{uzak_makine}}:{{0}}.{{0}}
```
{% endraw %}{% raw %}
<h2 id="xfce4-screenshooter">
  <a href="/tr/linux/xfce4-screenshooter.html">xfce4-screenshooter</a> <a href="#xfce4-screenshooter"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> XFCE4 ekran g??r??nt??s?? arac??.
> Daha fazla bilgi i??in: <https://docs.xfce.org/apps/xfce4-screenshooter/start>.

#### Ekran g??r??nt??s?? alma grafik aray??z??n?? ba??lat:
```shell
xfce4-screenshooter
```
#### T??m ekran??n ekran g??r??nt??s??n?? al ve nas??l devam edilece??ini belirlemek ad??na grafik aray??z??n?? ba??lat:
```shell
xfce4-screenshooter --fullscreen
```
#### T??m ekran??n ekran g??r??nt??s??n?? al ve g??r??nt??y?? belirtilen dizine kaydet:
```shell
xfce4-screenshooter --fullscreen --save {{??rnek/dizin}}
```
#### Ekran g??r??nt??s??n?? ??ekmeden ??nce belli bir s??re bekle:
```shell
xfce4-screenshooter --delay {{saniye_miktar??}}
```
#### Ekran??n (fare ile se??ilecek) belli bir b??l??m??n??n g??r??nt??s??n?? al:
```shell
xfce4-screenshooter --region
```
#### ??zerinde bulunulan pencerenin g??r??nt??s??n?? al ve panoya kopyala:
```shell
xfce4-screenshooter --window --clipboard
```
#### ??zerinde bulunulan pencerenin g??r??nt??s??n?? qal ve se??ilen bir program ile a??:
```shell
xfce4-screenshooter --window --open {{gimp}}
```
{% endraw %}{% raw %}
<h2 id="xfce4-terminal">
  <a href="/tr/linux/xfce4-terminal.html">xfce4-terminal</a> <a href="#xfce4-terminal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> XFCE4 terminal ??yk??n??c??s??.
> Daha fazla bilgi i??in: <https://docs.xfce.org/apps/xfce4-terminal/start>.

#### Yeni bir terminal penceresi a??:
```shell
xfce4-terminal
```
#### Ba??lang???? ba??l?????? belirle:
```shell
xfce4-terminal --initial-title "{{ba??lang????_ba??l??????}}"
```
#### Mevcut terminal penceresinde yeni bir sekme a??:
```shell
xfce4-terminal --tab
```
#### Yeni bir terminal penceresini belirlenen bir komutu ??al????t??rarak a??:
```shell
xfce4-terminal --command "{{arg??manl??_komut}}"
```
#### ??al????t??r??lan komutun ??al????may?? kesme durumunda dahi terminali kapama:
```shell
xfce4-terminal --command "{{arg??manl??_komut}}" --hold
```
#### Her birinde farkl?? komut ??al????acak bir??ok yeni sekme a??:
```shell
xfce4-terminal --tab --command "{{komut_a}}" --tab --command "{{komut_b}}"
```
{% endraw %}{% raw %}
<h2 id="xterm">
  <a href="/tr/linux/xterm.html">xterm</a> <a href="#xterm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> X Ekran Sistemi i??in terminal ??yk??n??c??s??.

#### `??rnek` ba??l??????na sahip bir terminal a??:
```shell
xterm -T {{??rnek}}
```
#### Terminali tam ekran modunda a??:
```shell
xterm -fullscreen
```
#### Terminali lacivert arkaplan ve sar?? ??n plan (font rengi) ile a??:
```shell
xterm -bg {{darkblue}} -fg {{yellow}}
```
#### Terminali sat??r ba????na 100 karakter ve s??tun ba????na 35 sat??r s????acak ??ekilde, x=200px y=20px koordinatlar??nda a??:
```shell
xterm -geometry {{100}}x{{35}}+{{200}}+{{20}}
```
#### Terminali bir Serif fontu ve 20'ye e??it olan bir font b??y??kl?????? ile a??:
```shell
xterm -fa "{{Serif}}" -fs {{20}}
```
{% endraw %}# Common
{% raw %}
<h2 id="7z">
  <a href="/tr/common/7z.html">7z</a> <a href="#7z"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Y??ksek s??k????t??rma oran??na sahip dosya s??k????t??r??c??s??.
> Daha fazla bilgi: <https://www.7-zip.org/>.

#### Dosya veya dizin ar??ivle:
```shell
7z a {{sikistirilmis_dosya.7z}} {{yoldan/dosya_veya_dizine}}
```
#### Varolan bir ar??ivi ????z??mle (headerlar dahil):
```shell
7z a {{sifrelenmi??_dosya.7z}} -p{{parola}} -mhe=on {{sikistirilmis_dosya.7z}}
```
#### Varolan 7z dosyas??n?? orijinal dizin yap??s??yla d????a aktar:
```shell
7z x {{sikistirilmis_dosya.7z}}
```
#### Ar??ivi kullan??c?? taraf??ndan belirtilmi?? ????k???? noktas??na aktar:
```shell
7z x {{sikistirilmis_dosya.7z}} -o{{yoldan/????kt??ya}}
```
#### Ar??ivi stdout'a aktar:
```shell
7z x {{sikistirilmis_dosya.7z}} -so
```
#### Spesifik bir ar??ivleme t??r??yle ar??ivle:
```shell
7z a -t{{zip|gzip|bzip2|tar}} {{sikistirilmis_dosya.7z}} {{yoldan/dosya_veya_dizine}}
```
#### Kullan??labilir ar??iv t??rlerini s??rala:
```shell
7z i
```
#### Ar??iv dosyas??n??n i??eri??ini listele:
```shell
7z l {{sikistirilmis_dosya.7z}}
```
{% endraw %}{% raw %}
<h2 id="base32">
  <a href="/tr/common/base32.html">base32</a> <a href="#base32"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bir dosya veya standart veriyi Base32 format??nda ??ifrele veya yal??n veri ????kt??s?? olarak de??ifre et.
> Daha fazla bilgi i??in: <https://www.gnu.org/software/coreutils/base32>.

#### Bir dosyay?? ??ifrele:
```shell
base32 {{dosyaismi}}
```
#### Bir dosyay?? de??ifre et:
```shell
base32 --decode {{dosyaismi}}
```
#### stdin'den ??ifrele:
```shell
{{herhangibirkomut}} | base32
```
#### stdin'den de??ifre et:
```shell
{{herhangibirkomut}} | base32 --decode
```
{% endraw %}{% raw %}
<h2 id="base64">
  <a href="/tr/common/base64.html">base64</a> <a href="#base64"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bir dosya veya standart veriyi Base64 format??nda ??ifrele veya yal??n veri ????kt??s?? olarak de??ifre et.
> Daha fazla bilgi i??in: <https://www.gnu.org/software/coreutils/base64>.

#### Bir dosyay?? ??ifrele:
```shell
base64 {{dosyaismi}}
```
#### Bir dosyay?? de??ifre et:
```shell
base64 --decode {{dosyaismi}}
```
#### stdin'den ??ifrele:
```shell
{{herhangibirkomut}} | base64
```
#### stdin'den de??ifre et:
```shell
{{herhangibirkomut}} | base64 --decode
```
{% endraw %}{% raw %}
<h2 id="chroot">
  <a href="/tr/common/chroot.html">chroot</a> <a href="#chroot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Komut veya etkile??imli komut sat??r??n?? ??zel k??k diziniyle ??al????t??r??r.
> Daha fazla bilgi i??in: <https://www.gnu.org/software/coreutils/chroot>.

#### Komutu yeni k??k dizini olarak ??al????t??r:
```shell
chroot {{yeni/kok/yolu}} {{komut}}
```
#### Kullan??lacak kullan??c?? ve grubu (ID veya isim) belirle:
```shell
chroot --userspec={{kullanici:grup}}
```
{% endraw %}{% raw %}
<h2 id="cmake">
  <a href="/tr/common/cmake.html">cmake</a> <a href="#cmake"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ??ok platformlu yap??m sistem olu??turucusu.
> Hedeflenen sisteme g??re Makefile, Visual Studio projeleri ve benzerlerini olu??turur.
> Daha fazla bilgi i??in: <https://cmake.org/cmake/help/latest/manual/cmake.1.html>.

#### Bir Makefile olu??tur ve onu ayn?? dizindeki bir projeyi derlemek i??in kullan:
```shell
cmake && make
```
#### Bir Makefile olu??tur ve onu farkl?? bir "yapim" dizinindeki projeyi derlemek i??in kullan (kaynak-d?????? yap??m):
```shell
cmake -H. -B {{build}} && make -C {{yapim}}
```
{% endraw %}{% raw %}
<h2 id="command">
  <a href="/tr/common/command.html">command</a> <a href="#command"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command, kabu??u bir program?? herhangi bir fonksiyon ve g??m??l?? ??zelli??e ve alias'a tak??lmadan ??al????t??rmaya zorlar.
> Daha fazla bilgi i??in: <https://manned.org/command>.

#### `ls` program??n?? ayn?? isimde bir alias olsa dahi ??al????t??r:
```shell
command {{ls}}
```
#### Alias'a atanan ??zel komutu veya ??al????t??r??labilir dosyan??n yolunu g??ster:
```shell
command -v {{komut_ismi}}
```
{% endraw %}{% raw %}
<h2 id="dirname">
  <a href="/tr/common/dirname.html">dirname</a> <a href="#dirname"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Belirtilen dosya veya yolun ana dizinini hesaplar.
> Daha fazla bilgi i??in: <https://www.gnu.org/software/coreutils/dirname>.

#### Belirtilen yolun ana dizinini hesapla:
```shell
dirname {{dosya_veya_dizine/giden/yol}}
```
#### Birden ??ok yolun ana dizinini hesapla:
```shell
dirname {{dosya_veya_dizine/giden/yol_1}} {{dosya_veya_dizine/giden/yol_2}}
```
#### Komut ????kt??s??n?? yeni sat??r yerine NUL karakteri ile s??n??rland??rma (`xargs` yaz??l??m?? ile kullan??rken i??e yarar):
```shell
dirname --zero {{dosya_veya_dizine/giden/yol_1}} {{dosya_veya_dizine/giden/yol_2}}
```
{% endraw %}{% raw %}
<h2 id="dirs">
  <a href="/tr/common/dirs.html">dirs</a> <a href="#dirs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Dizin y??????n?? g??r??nt??ler veya ??zerinde oynama yapar.
> Dizin y??????n??, `pushd` ve `popd` komutlar??yla ??zerinde oynama yap??labilen, son ziyaret edilen dizinleri g??steren bir listedir.
> Daha fazla bilgi i??in: <https://www.gnu.org/software/bash/manual/bash.html#Directory-Stack-Builtins>.

#### Dizin y??????n??n?? her madde aras??nda bo??luk olacak ??ekilde g??r??nt??le:
```shell
dirs
```
#### Dizin y??????n??n?? her sat??r ba???? tek madde olacak ??ekilde g??r??nt??le:
```shell
dirs -p
```
#### Dizin y??????n??nda 0'dan ba??lamak ??zere yaln??zca nth giri??ini g??ster:
```shell
dirs +{{N}}
```
#### Dizin y??????n??n?? temizle:
```shell
dirs -c
```
{% endraw %}{% raw %}
<h2 id="dirsearch">
  <a href="/tr/common/dirsearch.html">dirsearch</a> <a href="#dirsearch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A?? yolu taray??c??.
> Daha fazla bilgi i??in: <https://github.com/maurosoria/dirsearch>.

#### Bir a?? sunucusunu yayg??n eklentiler i??eren yayg??n yollar i??in taray??n:
```shell
dirsearch --url {{url}} --extensions-list
```
#### A?? sunucular??n?? i??eren bir listeyi `.php` eklentili yayg??n yollar i??in taray??n:
```shell
dirsearch --url-list {{??rnek/url-listesi.txt}} --extensions {{php}}
```
#### Bir a?? sunucusunu yayg??n eklentiler i??eren belirtilen yollar i??in taray??n:
```shell
dirsearch --url {{url}} --extensions-list --wordlist {{path/to/url-yol-listesi.txt}}
```
#### Bir a?? sunucusunu ??erez kullanarak taray??n:
```shell
dirsearch --url {{url}} --extensions {{php}} --cookie {{cookie}}
```
#### Bir a?? sunucusunu `HEAD` HTTP metodunu kullanarak taray??n:
```shell
dirsearch --url {{url}} --extensions {{php}} --http-method {{HEAD}}
```
#### Bir a?? sunucusunu taray??n ve sonu??lar?? bir `.json` dosyas??na kaydedin:
```shell
dirsearch --url {{url}} --extensions {{php}} --json-report {{??rnek/rapor_dosyas??.json}}
```
{% endraw %}{% raw %}
<h2 id="docker-build">
  <a href="/tr/common/docker-build.html">docker build</a> <a href="#docker-build"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bir Dockerfile'dan imge yarat??n.
> Daha fazla bilgi i??in: <https://docs.docker.com/engine/reference/commandline/build/>.

#### Mevcut dizindeki Dockerfile'dan bir docker imgesi olu??turun:
```shell
docker build .
```
#### Belirtilen URL'deki Dockerfile'dan bir docker imgesi olu??turun:
```shell
docker build {{ornekadres.com/ornek-dizin/ornek-docker-projesi}}
```
#### Bir docker imgesi olu??turun ve etiketleyin:
```shell
docker build --tag {{isim:etiket}} .
```
#### ??mge olu??tururken ??erez kullan??m??n?? etkisizle??tirin:
```shell
docker build --no-cache --tag {{isim:etiket}} .
```
#### Belirtilen Dockerfile ile bir docker imgesi olu??turun:
```shell
docker build --file {{Dockerfile}} .
```
#### Ki??iselle??tirilmi?? yap??m-zaman de??erleriyle olu??turun:
```shell
docker build --build-arg {{HTTP_PROXY=http://10.20.30.2:1234}} --build-arg {{FTP_PROXY=http://40.50.60.5:4567}} .
```
{% endraw %}{% raw %}
<h2 id="docker-compose">
  <a href="/tr/common/docker-compose.html">docker compose</a> <a href="#docker-compose"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ??oklu konteynerli docker uygulamalar??n?? ??al????t??r??n ve y??netin.
> Daha fazla bilgi i??in: <https://docs.docker.com/compose/reference/overview/>.

#### T??m konteynerleri listele:
```shell
docker-compose ps
```
#### Mevcut dizinde bir `docker-compose.yml` dosyas?? ??al????t??rarak arkaplandaki t??m konteynerleri ??al????t??r??n ve ba??lat??n:
```shell
docker-compose up -d
```
#### T??m konteynerleri ??al????t??r??n ve gerekiyorsa yeniden olu??turun:
```shell
docker-compose up --build
```
#### T??m konteynerleri alternatif bir beste dosyas??yla ba??lat??n:
```shell
docker-compose --file {{yoldan/dosyaya}} up
```
#### ??al????an t??m konteynerleri durdurun:
```shell
docker-compose stop
```
#### T??m konteynerleri, a??lar??, imgeleri ve alanlar?? durdurun ve silin:
```shell
docker-compose down --rmi all --volumes
```
#### T??m konteynerler i??in loglar?? takip edin:
```shell
docker-compose logs --follow
```
#### Belirtilmi?? bir konteyner i??in loglar?? takip edin:
```shell
docker-compose logs --follow {{konteyner_ismi}}
```
{% endraw %}{% raw %}
<h2 id="docker-exec">
  <a href="/tr/common/docker-exec.html">docker exec</a> <a href="#docker-exec"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Halihaz??rda ??al????an bir Docker konteyneri ??st??nde komut ??al????t??r.
> Daha fazla bilgi i??in: <https://docs.docker.com/engine/reference/komutline/exec/>.

#### Halihaz??rda ??al????an bir konteynerin ??st??nde interaktif bir kabuk oturumunu ??al????t??r:
```shell
docker exec --interactive --tty {{konteyner_ismi}} {{/bin/bash}}
```
#### Halihaz??rda ??al????an bir konteynerin ??st??ne arkaplanda ??al????mak ??zere (ayr??lm????) bir komut ??al????t??r:
```shell
docker exec --detach {{konteyner_ismi}} {{komut}}
```
#### Belirtilen bir komutu ??st??nde ??al????t??rmak ad??na ??al????an dizini se??:
```shell
docker exec --interactive -tty --workdir {{??rnek/dizin}} {{konteyner_ismi}} {{komut}}
```
#### Varolan konteyner ??st??nde arkaplanda ??al????mak ??zere bir komut ??al????t??r ancak stdin'i a????k tut:
```shell
docker exec --interactive --detach {{konteyner_ismi}} {{komut}}
```
#### ??al????makta olan bir bash oturumu i??inde bir ??evre de??i??keni belirle:
```shell
docker exec --interactive --tty --env {{de??i??ken_ismi}}={{value}} {{konteyner_ismi}} {{/bin/bash}}
```
#### Belirtilmi?? bir kullan??c?? olarak komut ??al????t??r:
```shell
docker exec --user {{kullan??c??}} {{konteyner_ismi}} {{komut}}
```
{% endraw %}{% raw %}
<h2 id="docker-images">
  <a href="/tr/common/docker-images.html">docker images</a> <a href="#docker-images"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Docker imgelerini y??net.
> Daha fazla bilgi i??in: <https://docs.docker.com/engine/reference/commandline/images/>.

#### T??m Docker imgelerini listele:
```shell
docker images
```
#### Orta d??zeyler de dahil olmak ??zere t??m Docker imgelerini s??rala:
```shell
docker images --all
```
#### ????kt??y?? sessiz modda (yaln??zca say??sal ID'ler olarak) s??rala:
```shell
docker images --quiet
```
#### Herhangi bir konteyner taraf??ndan kullan??lmayan t??m Docker imgelerini s??rala:
```shell
docker images --filter dangling=true
```
#### ??sminde belirtilen dizeleri ta????yan imgeleri s??rala:
```shell
docker images "{{*isim*}}"
```
{% endraw %}{% raw %}
<h2 id="docker-inspect">
  <a href="/tr/common/docker-inspect.html">docker inspect</a> <a href="#docker-inspect"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Docker objelerinde bulunan d??????k seviye bilgiyi g??sterir.
> Daha fazla bilgi i??in: <https://docs.docker.com/engine/reference/commandline/inspect/>.

#### Yard??m i??eri??ini g??ster:
```shell
docker inspect
```
#### Bir konteyner, imge veya hacim ile ilgili bilgiyi ismini veya ID'sini girerek g??r??nt??le:
```shell
docker inspect {{konteyner|imge|ID}}
```
#### Bir konteynerin IP adresini g??r??nt??le:
```shell
docker inspect --format='{{range .NetworkSettings.Networks}}{{.IPAddress}}{{end}}' {{konteyner}}
```
#### Konteynerin log dosyas??n??n yolunu g??r??nt??le:
```shell
docker inspect --format='{{.LogPath}}' {{konteyner}}
```
#### Konteynerin imge ismini g??r??nt??le:
```shell
docker inspect --format='{{.Config.Image}}' {{konteyner}}
```
#### Konfig??rasyon bilgisini JSON olarak g??r??nt??le:
```shell
docker inspect --format='{{json .Config}}' {{konteyner}}
```
#### T??m port limanlay??c??lar?? g??r??nt??le:
```shell
docker inspect --format='{{range $p, $conf := .NetworkSettings.Ports}} {{$p}} -> {{(index $conf 0).HostPort}} {{end}}' {{konteyner}}
```
{% endraw %}{% raw %}
<h2 id="docker-logs">
  <a href="/tr/common/docker-logs.html">docker logs</a> <a href="#docker-logs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Konteyner kayd??n?? yazd??r??r.
> Daha fazla bilgi i??in: <https://docs.docker.com/engine/reference/commandline/logs>.

#### Bir konteyner i??indeki kay??tlar?? yazd??r:
```shell
docker logs {{konteyner_ismi}}
```
#### Kay??tlar?? yazd??r ve izle:
```shell
docker logs -f {{konteyner_ismi}}
```
#### Son 5 kayd?? yazd??r:
```shell
docker logs {{konteyner_ismi}} --tail {{5}}
```
#### Kay??tlar?? yazd??r ve zaman damgalar?? ile ili??tir:
```shell
docker logs -t {{konteyner_ismi}}
```
#### Belli bir konteyner ??al????ma zaman??ndaki (i.e. 23m, 10s, 2013-01-02T13:23:37) kay??tlar?? yazd??r:
```shell
docker logs {{konteyner_ismi}} --until {{zaman}}
```
{% endraw %}{% raw %}
<h2 id="docker-machine">
  <a href="/tr/common/docker-machine.html">docker-machine</a> <a href="#docker-machine"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Docker ??al????t??ran makineler olu??tur ve onlar?? y??net.
> Daha fazla bilgi i??in: <https://docs.docker.com/machine/reference/>.

#### Halihaz??rda ??al????an docker makinelerini s??rala:
```shell
docker-machine ls
```
#### Belirli bir isim ile docker makinesi olu??tur:
```shell
docker-machine create {{isim}}
```
#### Bir makinenin durumunu ????ren:
```shell
docker-machine status {{isim}}
```
#### Bir makineyi ba??lat:
```shell
docker-machine start {{isim}}
```
#### Bir makineyi durdur:
```shell
docker-machine stop {{isim}}
```
#### Bir makine hakk??ndaki bilgileri incele:
```shell
docker-machine inspect {{isim}}
```
{% endraw %}{% raw %}
<h2 id="docker-network">
  <a href="/tr/common/docker-network.html">docker network</a> <a href="#docker-network"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Docker a??lar?? olu??tur ve y??net.
> Daha fazla bilgi i??in: <https://docs.docker.com/engine/reference/commandline/network/>.

#### docker daemon'daki t??m m??sait ve d??zenlenmi?? a??lar?? s??rala:
```shell
docker network ls
```
#### Kullan??c?? taraf??ndan belirtilmi?? bir a?? olu??tur:
```shell
docker network create --driver {{driver_name}} {{a??_ismi}}
```
#### Bo??luk ile ayr??lm???? bir a?? listesinin detayl?? bilgisini g??r??nt??le:
```shell
docker network inspect {{a??_ismi}}
```
#### Bir konteyneri isim veya ID kullanarak bir a??a ba??la:
```shell
docker network connect {{a??_ismi}} {{konteyner_ismi|ID}}
```
#### Bir konteyneri bir a??dan ????kar:
```shell
docker network disconnect {{a??_ismi}} {{konteyner_ismi|ID}}
```
#### T??m kullan??lmayan (hi??bir konteyner taraf??ndan belirtilmeyen) a??lar?? sil:
```shell
docker network prune
```
#### Kullan??lmayan a??lar??n bo??luk ile ayr??lm???? bir listesini sil:
```shell
docker network rm {{a??_ismi}}
```
{% endraw %}{% raw %}
<h2 id="docker-ps">
  <a href="/tr/common/docker-ps.html">docker ps</a> <a href="#docker-ps"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Docker konteynerlerini s??rala.
> Daha fazla bilgi i??in: <https://docs.docker.com/engine/reference/commandline/ps/>.

#### Halihaz??rda ??al????an docker konteynerlerini listele:
```shell
docker ps
```
#### T??m (durmu?? veya ??al????an) docker konteynerlerini listele:
```shell
docker ps --all
```
#### En son olu??turulan (durmu?? veya ??al????an) konteynerleri listele:
```shell
docker ps --latest
```
#### ??simlerinde belirtilen dizeleri i??eren konteynerleri filtrele:
```shell
docker ps --filter="name={{isim}}"
```
#### Belirtilen imge ile akrabal??k ta????yan konteynerleri filtrele:
```shell
docker ps --filter "ancestor={{imge}}:{{tag}}"
```
#### Konteynerleri ????k???? durum koduna g??re filtrele:
```shell
docker ps --all --filter="exited={{kod}}"
```
#### Konteynerleri mevcut durumlar??na (olu??turulma, ??al????ma, silinme, durma, ????kma ve ??lme) g??re s??rala:
```shell
docker ps --filter="status={{mevcut_durum}}"
```
#### Belirtilmi?? bir hacmi g??men veya belirtilmi?? bir yola g??m??lm???? hacmi i??eren konteynerleri filtrele:
```shell
docker ps --filter="volume={{??rnek/dizin}}" --format "table {{.ID}}\t{{.Image}}\t{{.Names}}\t{{.Mounts}}"
```
{% endraw %}{% raw %}
<h2 id="docker-rmi">
  <a href="/tr/common/docker-rmi.html">docker rmi</a> <a href="#docker-rmi"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bir veya daha fazla Docker imgesini sil.
> Daha fazla bilgi i??in: <https://docs.docker.com/engine/reference/commandline/rmi/>.

#### Yard??m g??ster:
```shell
docker rmi
```
#### Bir veya daha fazla imgeyi isimlerini belirterek sil:
```shell
docker rmi {{imge1 imge2 ...}}
```
#### Bir imgeyi zorla sil:
```shell
docker rmi --force {{imge}}
```
#### Bir imgeyi etiketlenmemi?? ana yollar??n?? silmeden sil:
```shell
docker rmi --no-prune {{imge}}
```
{% endraw %}{% raw %}
<h2 id="docker-run">
  <a href="/tr/common/docker-run.html">docker run</a> <a href="#docker-run"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Yeni bir Docker konteynerinde bir komut ??al????t??r.
> Daha fazla bilgi: <https://docs.docker.com/engine/reference/commandline/run/>.

#### Yeni bir konteynerde, etiketlenmi?? bir imgeden komut ??al????t??r.:
```shell
docker run {{imge:etiket}} {{komut}}
```
#### Yeni bir konteynerde arkaplanda ??al????acak ??ekilde komut ??al????t??r ve ID'sini g??ster:
```shell
docker run -d {{imge}} {{komut}}
```
#### ??nteraktif mod ve pseudo-TTY'deki bir a????k-kapal?? konteynerde komut ??al????t??r:
```shell
docker run --rm -it {{imge}} {{komut}}
```
#### Yeni bir konteynerde ge??ebilmi?? ??evresel de??i??kenler ile komut ??al????t??r:
```shell
docker run -e '{{de??i??ken}}={{de??er}}' -e {{de??i??ken}} {{imge}} {{komut}}
```
#### Yeni bir konteynerde ba??lama tak??l?? hacimlerle komut ??al????t??r:
```shell
docker run -v {{??rnek/host}}:{{??rnek/konteyner}} {{imge}} {{komut}}
```
#### Yay??nlanm???? portlar?? i??eren yeni bir konteynerde komut ??al????t??r:
```shell
docker run -p {{host_portu}}:{{konteyner_portu}} {{imge}} {{komut}}
```
{% endraw %}{% raw %}
<h2 id="docker-save">
  <a href="/tr/common/docker-save.html">docker save</a> <a href="#docker-save"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bir veya daha fazla docker imgesini ar??ivlemek i??in d????a aktar.
> Daha fazla bilgi i??in: <https://docs.docker.com/engine/reference/commandline/save/>.

#### Bir imgeyi, stdout'u tar ar??ivine y??nlendirerek kaydet:
```shell
docker save {{imge}}:{{etiket}} > {??rnek/dosya.tar}}
```
#### Bir imgeyi, bir tar ar??ivine kaydet:
```shell
docker save --output {{??rnek/dosya.tar}} {{imge}}:{{etiket}}
```
#### Bir imgenin t??m etiketlerini kaydet:
```shell
docker save --output {{??rnek/dosya.tar}} {{imge_ismi}}
```
#### Bir imgenin belirli etiketlerini kaydetmek i??in elle se??:
```shell
docker save --output {{??rnek/dosya.tar}} {{imge_ismi:etiket1 imge_ismi:etiket2 ...}}
```
{% endraw %}{% raw %}
<h2 id="docker-secret">
  <a href="/tr/common/docker-secret.html">docker secret</a> <a href="#docker-secret"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Docker swarm s??rlar??n?? y??net.
> Daha fazla bilgi i??in: <https://docs.docker.com/engine/reference/commandline/secret/>.

#### stdin'den yeni bir s??r yarat:
```shell
{{komut}} | docker secret create {{s??r_ismi}} -
```
#### Bir dosyadan yeni s??r olu??turun:
```shell
docker secret create {{s??r_ismi}} {{??rnek/dosya}}
```
#### T??m s??rlar?? s??rala:
```shell
docker secret ls
```
#### Bir veya daha fazla s??rra dair detayl?? bilgiyi insan dostu bir formatta g??ster:
```shell
docker secret inspect --pretty {{s??r_ismi1 s??r_ismi2 ...}}
```
#### Bir veya daha fazla s??rr?? sil:
```shell
docker secret rm {{s??r_ismi1 s??r_ismi2 ...}}
```
{% endraw %}{% raw %}
<h2 id="docker-service">
  <a href="/tr/common/docker-service.html">docker service</a> <a href="#docker-service"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bir docker daemon'unun ??zerindeki servisleri y??net.
> Daha fazla bilgi i??in: <https://docs.docker.com/engine/reference/commandline/service/>.

#### Bir docker daeomon'unun ??zerindeki servisleri listele:
```shell
docker service ls
```
#### Yeni bir servis yarat:
```shell
docker service create --name {{servis_ismi}} {{imge}}:{{etiket}}
```
#### Bo??luk ile ayr??lm???? bir servis listesinin detayl?? bilgisini g??r??nt??le:
```shell
docker service inspect {{servis_ismi|ID}}
```
#### Bo??luk ile ayr??lm???? bir servis listesinin g??revlerini s??rala:
```shell
docker service ps {{servis_ismi|ID}}
```
#### Bo??luk ile ayr??lm???? bir servis listesi i??in belirli bir replika miktar??na y??ksel:
```shell
docker service scale {{servis_ismi}}={{replika_miktar??}}
```
#### Bo??luk ile ayr??lm???? bir servis listesini sil:
```shell
docker service rm {{servis_ismi|ID}}
```
{% endraw %}{% raw %}
<h2 id="docker-start">
  <a href="/tr/common/docker-start.html">docker start</a> <a href="#docker-start"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bir veya daha fazla durmu?? konteyneri ba??lar.
> Daha fazla bilgi i??in: <https://docs.docker.com/engine/reference/commandline/start/>.

#### Yard??m g??ster:
```shell
docker start
```
#### Bir docker konteynerini ba??lat:
```shell
docker start {{konteyner}}
```
#### Bir konteyneri, ona stdout ile stderr'i ekleyerek ve sinyaller g??ndererek ba??lat:
```shell
docker start --attach {{konteyner}}
```
#### Bir veya daha fazla bo??lukla ayr??larak belirtilmi?? konteynerleri ba??lar:
```shell
docker start {{konteyner(ler)}}
```
{% endraw %}{% raw %}
<h2 id="docker-stats">
  <a href="/tr/common/docker-stats.html">docker stats</a> <a href="#docker-stats"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Konteynerler i??in kaynak kullan??m istatistiklerinin canl?? yay??n??n?? g??r??nt??le.
> Daha fazla bilgi i??in: <https://docs.docker.com/engine/reference/commandline/stats/>.

#### ??al????an t??m konteynerlerin aynak kullan??m istatistiklerinin canl?? yay??n??n?? g??r??nt??le:
```shell
docker stats
```
#### Bo??luk ile ayr??lm???? bir listedeki konteynerlerin canl?? yay??n??n?? g??r??nt??le:
```shell
docker stats {{container_ismi}}
```
#### Konteyner'in CPU kullan??m y??zdesini g??stermek i??in s??tun format??n?? de??i??tir:
```shell
docker stats --format "{{.Name}}:\t{{.CPUPerc}}"
```
#### T??m (??al????an veya durmu??) konteynerler i??in istatistikleri g??r??nt??le:
```shell
docker stats --all
```
#### ??statistikleri canl?? yay??nlamay?? durdur ve yaln??zca mevcut durumdaki istatistikleri g??r??nt??le:
```shell
docker stats --no-stream
```
{% endraw %}{% raw %}
<h2 id="docker-swarm">
  <a href="/tr/common/docker-swarm.html">docker swarm</a> <a href="#docker-swarm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bir konteyner orkestrasyon arac??.
> Daha fazla bilgi i??in: <https://docs.docker.com/engine/swarm/>.

#### Bir batakl??k dizisi olu??tur:
```shell
docker swarm init
```
#### Bir y??netici veya i????iye tak??lmak i??in token g??ster:
```shell
docker swarm join-token {{i????i|y??netici}}
```
#### Diziye yeni bir d??????m ekle:
```shell
docker swarm join --token {{token}} {{manager_node_url:2377}}
```
#### Bir i????iyi batakl??ktan sil (i????i d??????m??n??n i??inde ??al????t??r):
```shell
docker swarm leave
```
#### Mevcut CA sertifikas??n?? PEM format??nda g??r??nt??le:
```shell
docker swarm ca
```
#### Mevcut CA sertifikas??n?? d??nd??r ve yeni sertifikay?? g??r??nt??le:
```shell
docker swarm ca --rotate
```
#### D??????m sertifikalar?? i??in ge??erli periyodu de??i??tir:
```shell
docker swarm update --cert-expiry {{saat}}h{{dakika}}m{{saniye}}s
```
{% endraw %}{% raw %}
<h2 id="docker-system">
  <a href="/tr/common/docker-system.html">docker system</a> <a href="#docker-system"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Docker verilerini y??net ve sistem bilgisi g??r??nt??le.
> More information: <https://docs.docker.com/engine/reference/commandline/system/>.

#### Yard??m g??ster:
```shell
docker system
```
#### Docker disk kullan??m??n?? g??ster:
```shell
docker system df
```
#### Disk kullan??m?? ??zerine detayl?? bilgi g??ster:
```shell
docker system df --verbose
```
#### Kullan??lmayan veriyi sil:
```shell
docker system prune
```
#### Kullan??lmayan ve ge??mi??te birden ??ok kez olu??turulan veriyi sil:
```shell
docker system prune --filter="until={{saat}}h{{dakika}}m"
```
#### Docker deamon'dan tam-zamanl?? eylemleri g??r??nt??le:
```shell
docker system events
```
#### Ge??erli JSON sat??rlar?? olarak yay??nlanan konteynerleden tam-zamanl?? eylemleri g??ster:
```shell
docker system events --filter 'type=container' --format '{{json .}}'
```
#### Sistem bilgisi g??ster:
```shell
docker system info
```
{% endraw %}{% raw %}
<h2 id="docker">
  <a href="/tr/common/docker.html">docker</a> <a href="#docker"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Docker konteyner ve imgelerini y??netir.
> Daha fazla bilgi i??in: <https://docs.docker.com/engine/reference/commandline/cli/>.

#### ??uan ??al????an docker konteynerlerini listele:
```shell
docker ps
```
#### T??m (??al????an veya duran) docker konteynerlerini listele:
```shell
docker ps -a
```
#### Bir imgeden ??zel bir isimle konteyner ba??lat:
```shell
docker run --name {{konteyner_ismi}} {{imge}}
```
#### Varolan bir konteyneri ba??lat veya durdur:
```shell
docker {{baslat|durdur}} {{konteyner_ismi}}
```
#### Bir docker kayd??ndan imge ??ek:
```shell
docker pull {{imge}}
```
#### Halihaz??rda ??al????an bir konteyner i??inde komut istemcisi a??:
```shell
docker exec -it {{konteyner_ismi}} {{sh}}
```
#### Durmu?? bir konteyneri sil:
```shell
docker rm {{konteyner_ismi}}
```
#### Bir konteynerin kayd??n?? ??ek ve takip et:
```shell
docker logs -f {{konteyner_ismi}}
```
{% endraw %}{% raw %}
<h2 id="man">
  <a href="/tr/common/man.html">man</a> <a href="#man"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> K??lavuz sayfalar??n?? bi??imlendir ve g??ster.
> Daha fazla bilgi i??in: <https://www.man7.org/linux/man-pages/man1/man.1.html>.

#### Bir komut i??in man sayfas??n?? g??r??nt??le:
```shell
man {{komut}}
```
#### Sayfan??n 7. b??l??m??ndeki bir komut i??in man sayfas??n?? g??r??nt??le:
```shell
man {{komut}}.{{7}}
```
#### Mansayfalar?? i??in arat??lan yolu g??ster:
```shell
man --path
```
#### Mansayfas??n?? g??stermek yerine mansayfas??n??n konumunu g??ster:
```shell
man -w {{komut}}
```
#### Belirtilen ifadeyi i??eren mansayfalar??n?? ara:
```shell
man -k "{{aranan_ifade}}"
```
{% endraw %}{% raw %}
<h2 id="minetest">
  <a href="/tr/common/minetest.html">minetest</a> <a href="#minetest"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ??ok oyunculu s??n??rs??z d??nyal?? bloklu sandbox oyun motoru.
> Ayr??ca `minetestserver` sayfas??na bak??lmas?? ??nerilir.
> Daha fazla bilgi i??in: <https://wiki.minetest.net/Minetest>.

#### Minetest'i kullan??c?? modunda ba??lat:
```shell
minetest
```
#### Minetest'i belirtilen d??nyay?? host edecek ??ekilde sunucu modunda ba??lat:
```shell
minetest --server --world {{isim}}
```
#### Belirtilmi?? bir dosyaya ge??mi??i yaz:
```shell
minetest --logfile {{??rnek/dosya}}
```
#### Hatalar?? yaln??zca konsola yaz:
```shell
minetest --quiet
```
{% endraw %}{% raw %}
<h2 id="minetestserver">
  <a href="/tr/common/minetestserver.html">minetestserver</a> <a href="#minetestserver"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ??ok oyunculu s??n??rs??z d??nyal?? bloklu sanbox sunucusu.
> Ayr??ca `minetest` sayfas??na bak??lmas?? ??nerilir.
> Daha fazla bilgi i??in: <https://wiki.minetest.net/Setting_up_a_server>.

#### Sunucuyu ba??lar:
```shell
minetestserver
```
#### M??sait d??nyalar?? s??rala:
```shell
minetestserver --world list
```
#### Y??klenecek d??nya ismini belirt:
```shell
minetestserver --world {{dunya_ismi}}
```
#### M??sait oyun ID'lerini s??rala:
```shell
minetestserver --gameid list
```
#### Kullan??lacak oyunu belirt:
```shell
minetestserver --gameid {{oyun_id'si}}
```
#### Belirtilmi?? bir port'u dinle:
```shell
minetestserver --port {{34567}}
```
#### Ba??ka bir veritaban?? yaz??l??m??na g???? et:
```shell
minetestserver --migrate {{sqlite3|leveldb|redis}}
```
#### Sunucuyu ba??latt??ktan sonra interaktif bir terminal a??:
```shell
minetestserver --terminal
```
{% endraw %}{% raw %}
<h2 id="tldr-lint">
  <a href="/tr/common/tldr-lint.html">tldr-lint</a> <a href="#tldr-lint"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> `tldr` sayfalar??n?? g??zden ge??ir ve bi??imlendir.
> Daha fazla bilgi i??in: <https://github.com/tldr-pages/tldr-lint>.

#### T??m sayfalar?? g??zden ge??ir:
```shell
tldr-lint {{sayfa_dizini}}
```
#### Belirtilmi?? bir sayfay?? stdout'a bi??imlendir:
```shell
tldr-lint --format {{page.md}}
```
#### Bir konumdaki t??m sayfalar?? bi??imlendir:
```shell
tldr-lint --format --in-place {{sayfa_dizini}}
```
{% endraw %}{% raw %}
<h2 id="tldr">
  <a href="/tr/common/tldr.html">tldr</a> <a href="#tldr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Komut sat??r?? ara??lar?? i??in tldr-pages projesinden basit yard??m sayfalar?? g??r??nt??ler.
> Daha fazla bilgi i??in: <https://tldr.sh>.

#### Bir komutun tipik kullan??m??n?? g??ster (ipucu: buray?? g??r??nt??lemek i??in kulland??????n??z komutun ayn??s??!):
```shell
tldr {{komut}}
```
#### Linux i??in tar tldr sayfas??n?? g??ster:
```shell
tldr -p {{linux}} {{tar}}
```
#### Bir Git alt komutu i??in yard??m al:
```shell
tldr {{git-checkout}}
```
#### (E??er al??c?? ??nbellek olu??umunu destekliyorsa) Yerel paketleri g??ncelle:
```shell
tldr -u
```
{% endraw %}{% raw %}
<h2 id="tldrl">
  <a href="/tr/common/tldrl.html">tldrl</a> <a href="#tldrl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> `tldr-lint` komutunun ayn??s??.

#### Orijinal komut i??in yard??m sayfas??n?? g??ster:
```shell
tldr tldr-lint
```
{% endraw %}