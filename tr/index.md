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
> Debian ve Ubuntu paket yönetim aracı.
> Paket aramak için `apt-cache` komutunu kullanın.
> Daha fazla bilgi için: <https://manpages.debian.org/latest/apt/apt-get.8.html>.

#### Kullanılabilir paket ve versiyon listesini güncelleyin (diğer `apt-get` komutlarını çalıştırmadan önce kullanmanız önerilir):
```shell
apt-get update
```
#### Bir paket yükleyin veya son sürüme güncelleyin:
```shell
apt-get install {{paket}}
```
#### Bir paketi silin:
```shell
apt-get remove {{paket}}
```
#### Bir paketi ve konfigürasyon dosyalarını silin:
```shell
apt-get purge {{paket}}
```
#### Yüklü paketlerin hepsini son sürümlerine yükseltin:
```shell
apt-get upgrade
```
#### Yerel depoyu temizleyin - kullanılmayan gereksiz paket dosyalarını (.deb) silin:
```shell
apt-get autoclean
```
#### Artık gerekmeyen paketleri silin:
```shell
apt-get autoremove
```
#### Yüklenmiş paketleri yükseltin (`upgrade` gibi), ancak gereksiz paketleri silin ve yeni bağımlılıkları memnun edecek ek paketler kurun:
```shell
apt-get dist-upgrade
```
{% endraw %}{% raw %}
<h2 id="aptitude">
  <a href="/tr/linux/aptitude.html">aptitude</a> <a href="#aptitude"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Debian ve Ubuntu paket yönetim aracı.
> Daha fazla bilgi için: <https://manpages.debian.org/latest/aptitude/aptitude.8.html>.

#### Kullanılabilir paket ve sürüm listesini senkronize et. Bu, herhangi bir aptitude komutunu uygulamadan önce çalıştırılmalıdır:
```shell
aptitude update
```
#### Yeni bir paket ve onun bağımlılıklarını kur:
```shell
aptitude install {{paket}}
```
#### Paket ara:
```shell
aptitude search {{paket}}
```
#### İndirilmiş bir paket ara: (`?installed` bir aptitude arama ifadesidir):
```shell
aptitude search '?installed({{paket}})'
```
#### Bir paket ve onun bağımlılıklarını kaldır:
```shell
aptitude remove {{paket}}
```
#### Yüklü paketleri son kullanılabilir sürümlerine yükselt:
```shell
aptitude upgrade
```
#### Yüklü paketleri yükle (`aptitude upgrade` gibi), gereksizleri sil ve yeni bağımlılıkları karşılamak üzere ek paketler kur:
```shell
aptitude full-upgrade
```
#### Bir paketin otomatik yükseltilmesini engellemek için onu beklemede tut:
```shell
aptitude hold '?installed({{paket}})'
```
{% endraw %}{% raw %}
<h2 id="pacman-mirrors">
  <a href="/tr/linux/pacman-mirrors.html">pacman-mirrors</a> <a href="#pacman-mirrors"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manjaro Linux için pacman aynalistesi oluşturucu.
> pacman-mirrors'ın çalıştırıldığı her vakit, E`sudo pacman -Syyu` komutu ile veritabanının senkronize edilmesi ve sistemin güncellenmesi gerekir.
> Daha fazla bilgi için: <https://wiki.manjaro.org/index.php?title=Pacman-mirrors>.

#### Varsayılan ayarlar ile bir aynalistesi oluştur:
```shell
sudo pacman-mirrors --fasttrack
```
#### Mevcut aynaların durumunu göster:
```shell
pacman-mirrors --status
```
#### Mevcut dalı göster:
```shell
pacman-mirrors --get-branch
```
#### Farklı bir dala geç:
```shell
sudo pacman-mirrors --api --set-branch {{stabil|instabil|test_ediliyor}}
```
#### Sadece IP adresinin bulunduğu ülkenin aynalarını kullanarak bir aynalistesi oluştur:
```shell
sudo pacman-mirrors --geoip
```
{% endraw %}{% raw %}
<h2 id="pacman---query">
  <a href="/tr/linux/pacman-query.html">pacman --query</a> <a href="#pacman---query"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux paket yönetim aracı.
> Daha fazla bilgi için: <https://man.archlinux.org/man/pacman.8>.

#### Yüklenmiş paket ve sürümleri sırala:
```shell
pacman --query
```
#### Sadece özellikle indirilmiş paket ve sürümleri sırala:
```shell
pacman --query --explicit
```
#### Hangi paketin belirtilen dosyaya sahip olduğunu bul:
```shell
pacman --query --owns {{dosya_ismi}}
```
#### İndirilmiş bir pakete dair bilgiyi görüntüle:
```shell
pacman --query --info {{paket_ismi}}
```
#### Bir paketin içerdiği dosyaları sırala:
```shell
pacman --query --list {{paket_ismi}}
```
#### Yetim (başka bir pakete bağlılık olarak indirilmiş ancak herhangi bir paket tarafından gerektirilmeyen) paketleri sırala:
```shell
pacman --query --unrequired --deps --quiet
```
#### Mevcut depolarda bulunmayan, indirilmiş paketleri sırala:
```shell
pacman --query --foreign
```
#### Miadı dolmuş paketleri sırala:
```shell
pacman --query --upgrades
```
{% endraw %}{% raw %}
<h2 id="pacman---remove">
  <a href="/tr/linux/pacman-remove.html">pacman --remove</a> <a href="#pacman---remove"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux paket yönetim aracı.
> Daha fazla bilgi için: <https://man.archlinux.org/man/pacman.8>.

#### Bu alt komut için yardım göster:
```shell
pacman --remove --help
```
#### Bir paket ve bağlılıklarını sil:
```shell
sudo pacman --remove --recursive {{paket_ismi}}
```
#### Bir paketi ve onun hem bağlılıklarını, hem de konfigürasyon dosyalarını sil:
```shell
sudo pacman --remove --recursive --nosave {{paket_ismi}}
```
#### Bir paketi telkin olmaksızın sil:
```shell
sudo pacman --remove --noconfirm {{paket_ismi}}
```
#### Yetim (başka bir pakete bağlılık olarak indirilmiş ancak herhangi bir paket tarafından gerektirilmeyen) paketleri sil:
```shell
sudo pacman --remove --recursive --nosave $(pacman --query --unrequired --deps --quiet)
```
#### Bir paketi ve ona bağlı olan tüm öbür paketleri sil:
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
> Arch Linux paket yönetim aracı.
> Daha fazla bilgi için: <https://man.archlinux.org/man/pacman.8>.

#### Yeni bir paket indir::
```shell
sudo pacman --sync {{paket_ismi}}
```
#### Tüm paketleri senkronize et ve güncelle (bahsi geçen paketleri güncellemeden indirmek için `--downloadonly` eki gereklidir)
```shell
sudo pacman --sync --refresh --sysupgrade
```
#### Tüm paketleri güncelle ve telkin olmaksızın yeni bir tane indir:
```shell
sudo pacman --sync --refresh --sysupgrade --noconfirm {{paket_ismi}}
```
#### Paket veritabanını girilen ifade ile arat:
```shell
pacman --sync --search "{{arama_şablonu}}"
```
#### Bir paket hakkında bilgi görüntüle:
```shell
pacman --sync --info {{paket_ismi}}
```
#### Bir paket güncellemesi sırasında çakışan dosyaların üstüne yaz:
```shell
sudo pacman --sync --refresh --sysupgrade --overwrite {{örnek_dosya}}
```
#### Tüm paketleri senkronize et ve güncelle, ancak belli bir paketi yoksay:
```shell
sudo pacman --sync --refresh --sysupgrade --ignore {{paket_ismi}}
```
#### Kullanılmayan paket ve kullanılmamış depoları çerezlerden sil (tüm paketlerin çerezlerini temizlemek için `--clean` eki iki kez kullanılmalıdır):
```shell
sudo pacman --sync --clean
```
{% endraw %}{% raw %}
<h2 id="pacman">
  <a href="/tr/linux/pacman.html">pacman</a> <a href="#pacman"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux paket yönetim aracı.
> Daha fazla bilgi için: <https://man.archlinux.org/man/pacman.8>.

#### Tüm paketleri senkronize et ve güncelle:
```shell
pacman -Syu
```
#### Yeni bir paket indir:
```shell
pacman -S {{paket_ismi}}
```
#### Bir paket ve bağlılıklarını sil:
```shell
pacman -Rs {{paket_ismi}}
```
#### Paket veritabanını girilen ifade ile arat:
```shell
pacman -Ss "{{arama_şablonu}}"
```
#### İndirilmiş paket ve sürümleri sırala:
```shell
pacman -Q
```
#### Sadece özellikle belirtilen paket ve sürümleri sırala:
```shell
pacman -Qe
```
#### Hangi paketin belirtilen dosyaya sahip olduğunu bul:
```shell
pacman -Qo {{dosya_ismi}}
```
#### Paket çerezlerini boş alan açmak için temizle:
```shell
pacman -Scc
```
{% endraw %}{% raw %}
<h2 id="pulseaudio">
  <a href="/tr/linux/pulseaudio.html">pulseaudio</a> <a href="#pulseaudio"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ses sistem arkaplan uygulaması ve yöneticisi.
> Daha fazla bilgi için: <https://www.freedesktop.org/wiki/Software/PulseAudio/>.

#### Pulseaudio'nun çalışıp çalışmadığını kontrol et (sıfır olmayan çıktı, çalışmadığı anlamına gelir):
```shell
pulseaudio --check
```
#### Pulseaudio'yu arkaplanda çalıştır:
```shell
pulseaudio --start
```
#### Arkaplanda çalışan tüm pulseaudio uygulamalarını öldür:
```shell
pulseaudio --kill
```
#### Müsait modülleri sırala:
```shell
pulseaudio --dump-modules
```
#### Belirtilen argümanlarla bir modülü mevcut çalışan arkaplan uygulamasına yükle:
```shell
pulseaudio --load="{{modül_ismi}} {{argümanlar}}"
```
{% endraw %}{% raw %}
<h2 id="tree">
  <a href="/tr/linux/tree.html">tree</a> <a href="#tree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mevcut dizinin içeriğini ağaç biçiminde göster.
> Daha fazla bilgi için: <http://mama.indstate.edu/users/ice/tree/>.

#### Dosya ve dizinleri `num` değeri kadar derinlikte göster (1 olması durumunda mevcut dizin gösterilir):
```shell
tree -L {{num}}
```
#### Yalnızca dizinleri göster:
```shell
tree -d
```
#### Renklendirme açık olacak şekilde gizli dosyaları dahi göster:
```shell
tree -a -C
```
#### Ağacın satırlarını girintiler yerine tüm yolu belirterek göster:
```shell
tree -i -f
```
#### Tüm dosyaların ve dizinlerin eklenerek artan boyutlarını, insanların okuyabileceği bir biçimde göster:
```shell
tree -s -h --du
```
#### Ağaç hiyerarşisi içindeki dosyaları bir wildcard (glob) kalıbı kullanarak ve aranan özellikteki dosyalara sahip olmayan dizinleri yoksayarak göster:
```shell
tree -P '{{*.txt}}' --prune
```
#### Ağaç hiyerarşisi içindeki dizinleri bir wildcard (glob) kalıbı kullanarak ve istenen dizine atalığı olmayan dizinleri yoksayarak göster:
```shell
tree -P {{dizin_ismi}} --matchdirs --prune
```
#### Ağacı belirtilen dizinleri yoksayarak göster:
```shell
tree -I '{{dizin_ismi1|dizin_ismi2}}'
```
{% endraw %}{% raw %}
<h2 id="xeyes">
  <a href="/tr/linux/xeyes.html">xeyes</a> <a href="#xeyes"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ekranda fare imlecini takip eden bir çift göz göster.

#### Xeyes'ı yerel makinenin varsayılan ekranında başlat:
```shell
xeyes
```
#### Xeyes'ı uzak bir makinenin 0. görüntü ve 0. ekran koordinatlarında başlat:
```shell
xeyes -display {{uzak_makine}}:{{0}}.{{0}}
```
{% endraw %}{% raw %}
<h2 id="xfce4-screenshooter">
  <a href="/tr/linux/xfce4-screenshooter.html">xfce4-screenshooter</a> <a href="#xfce4-screenshooter"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> XFCE4 ekran görüntüsü aracı.
> Daha fazla bilgi için: <https://docs.xfce.org/apps/xfce4-screenshooter/start>.

#### Ekran görüntüsü alma grafik arayüzünü başlat:
```shell
xfce4-screenshooter
```
#### Tüm ekranın ekran görüntüsünü al ve nasıl devam edileceğini belirlemek adına grafik arayüzünü başlat:
```shell
xfce4-screenshooter --fullscreen
```
#### Tüm ekranın ekran görüntüsünü al ve görüntüyü belirtilen dizine kaydet:
```shell
xfce4-screenshooter --fullscreen --save {{örnek/dizin}}
```
#### Ekran görüntüsünü çekmeden önce belli bir süre bekle:
```shell
xfce4-screenshooter --delay {{saniye_miktarı}}
```
#### Ekranın (fare ile seçilecek) belli bir bölümünün görüntüsünü al:
```shell
xfce4-screenshooter --region
```
#### Üzerinde bulunulan pencerenin görüntüsünü al ve panoya kopyala:
```shell
xfce4-screenshooter --window --clipboard
```
#### Üzerinde bulunulan pencerenin görüntüsünü qal ve seçilen bir program ile aç:
```shell
xfce4-screenshooter --window --open {{gimp}}
```
{% endraw %}{% raw %}
<h2 id="xfce4-terminal">
  <a href="/tr/linux/xfce4-terminal.html">xfce4-terminal</a> <a href="#xfce4-terminal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> XFCE4 terminal öykünücüsü.
> Daha fazla bilgi için: <https://docs.xfce.org/apps/xfce4-terminal/start>.

#### Yeni bir terminal penceresi aç:
```shell
xfce4-terminal
```
#### Başlangıç başlığı belirle:
```shell
xfce4-terminal --initial-title "{{başlangıç_başlığı}}"
```
#### Mevcut terminal penceresinde yeni bir sekme aç:
```shell
xfce4-terminal --tab
```
#### Yeni bir terminal penceresini belirlenen bir komutu çalıştırarak aç:
```shell
xfce4-terminal --command "{{argümanlı_komut}}"
```
#### Çalıştırılan komutun çalışmayı kesme durumunda dahi terminali kapama:
```shell
xfce4-terminal --command "{{argümanlı_komut}}" --hold
```
#### Her birinde farklı komut çalışacak birçok yeni sekme aç:
```shell
xfce4-terminal --tab --command "{{komut_a}}" --tab --command "{{komut_b}}"
```
{% endraw %}{% raw %}
<h2 id="xterm">
  <a href="/tr/linux/xterm.html">xterm</a> <a href="#xterm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> X Ekran Sistemi için terminal öykünücüsü.

#### `Örnek` başlığına sahip bir terminal aç:
```shell
xterm -T {{Örnek}}
```
#### Terminali tam ekran modunda aç:
```shell
xterm -fullscreen
```
#### Terminali lacivert arkaplan ve sarı ön plan (font rengi) ile aç:
```shell
xterm -bg {{darkblue}} -fg {{yellow}}
```
#### Terminali satır başına 100 karakter ve sütun başına 35 satır sığacak şekilde, x=200px y=20px koordinatlarında aç:
```shell
xterm -geometry {{100}}x{{35}}+{{200}}+{{20}}
```
#### Terminali bir Serif fontu ve 20'ye eşit olan bir font büyüklüğü ile aç:
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
> Yüksek sıkıştırma oranına sahip dosya sıkıştırıcısı.
> Daha fazla bilgi: <https://www.7-zip.org/>.

#### Dosya veya dizin arşivle:
```shell
7z a {{sikistirilmis_dosya.7z}} {{yoldan/dosya_veya_dizine}}
```
#### Varolan bir arşivi çözümle (headerlar dahil):
```shell
7z a {{sifrelenmiş_dosya.7z}} -p{{parola}} -mhe=on {{sikistirilmis_dosya.7z}}
```
#### Varolan 7z dosyasını orijinal dizin yapısıyla dışa aktar:
```shell
7z x {{sikistirilmis_dosya.7z}}
```
#### Arşivi kullanıcı tarafından belirtilmiş çıkış noktasına aktar:
```shell
7z x {{sikistirilmis_dosya.7z}} -o{{yoldan/çıktıya}}
```
#### Arşivi stdout'a aktar:
```shell
7z x {{sikistirilmis_dosya.7z}} -so
```
#### Spesifik bir arşivleme türüyle arşivle:
```shell
7z a -t{{zip|gzip|bzip2|tar}} {{sikistirilmis_dosya.7z}} {{yoldan/dosya_veya_dizine}}
```
#### Kullanılabilir arşiv türlerini sırala:
```shell
7z i
```
#### Arşiv dosyasının içeriğini listele:
```shell
7z l {{sikistirilmis_dosya.7z}}
```
{% endraw %}{% raw %}
<h2 id="base32">
  <a href="/tr/common/base32.html">base32</a> <a href="#base32"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bir dosya veya standart veriyi Base32 formatında şifrele veya yalın veri çıktısı olarak deşifre et.
> Daha fazla bilgi için: <https://www.gnu.org/software/coreutils/base32>.

#### Bir dosyayı şifrele:
```shell
base32 {{dosyaismi}}
```
#### Bir dosyayı deşifre et:
```shell
base32 --decode {{dosyaismi}}
```
#### stdin'den şifrele:
```shell
{{herhangibirkomut}} | base32
```
#### stdin'den deşifre et:
```shell
{{herhangibirkomut}} | base32 --decode
```
{% endraw %}{% raw %}
<h2 id="base64">
  <a href="/tr/common/base64.html">base64</a> <a href="#base64"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bir dosya veya standart veriyi Base64 formatında şifrele veya yalın veri çıktısı olarak deşifre et.
> Daha fazla bilgi için: <https://www.gnu.org/software/coreutils/base64>.

#### Bir dosyayı şifrele:
```shell
base64 {{dosyaismi}}
```
#### Bir dosyayı deşifre et:
```shell
base64 --decode {{dosyaismi}}
```
#### stdin'den şifrele:
```shell
{{herhangibirkomut}} | base64
```
#### stdin'den deşifre et:
```shell
{{herhangibirkomut}} | base64 --decode
```
{% endraw %}{% raw %}
<h2 id="chroot">
  <a href="/tr/common/chroot.html">chroot</a> <a href="#chroot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Komut veya etkileşimli komut satırını özel kök diziniyle çalıştırır.
> Daha fazla bilgi için: <https://www.gnu.org/software/coreutils/chroot>.

#### Komutu yeni kök dizini olarak çalıştır:
```shell
chroot {{yeni/kok/yolu}} {{komut}}
```
#### Kullanılacak kullanıcı ve grubu (ID veya isim) belirle:
```shell
chroot --userspec={{kullanici:grup}}
```
{% endraw %}{% raw %}
<h2 id="cmake">
  <a href="/tr/common/cmake.html">cmake</a> <a href="#cmake"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Çok platformlu yapım sistem oluşturucusu.
> Hedeflenen sisteme göre Makefile, Visual Studio projeleri ve benzerlerini oluşturur.
> Daha fazla bilgi için: <https://cmake.org/cmake/help/latest/manual/cmake.1.html>.

#### Bir Makefile oluştur ve onu aynı dizindeki bir projeyi derlemek için kullan:
```shell
cmake && make
```
#### Bir Makefile oluştur ve onu farklı bir "yapim" dizinindeki projeyi derlemek için kullan (kaynak-dışı yapım):
```shell
cmake -H. -B {{build}} && make -C {{yapim}}
```
{% endraw %}{% raw %}
<h2 id="command">
  <a href="/tr/common/command.html">command</a> <a href="#command"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command, kabuğu bir programı herhangi bir fonksiyon ve gömülü özelliğe ve alias'a takılmadan çalıştırmaya zorlar.
> Daha fazla bilgi için: <https://manned.org/command>.

#### `ls` programını aynı isimde bir alias olsa dahi çalıştır:
```shell
command {{ls}}
```
#### Alias'a atanan özel komutu veya çalıştırılabilir dosyanın yolunu göster:
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
> Daha fazla bilgi için: <https://www.gnu.org/software/coreutils/dirname>.

#### Belirtilen yolun ana dizinini hesapla:
```shell
dirname {{dosya_veya_dizine/giden/yol}}
```
#### Birden çok yolun ana dizinini hesapla:
```shell
dirname {{dosya_veya_dizine/giden/yol_1}} {{dosya_veya_dizine/giden/yol_2}}
```
#### Komut çıktısını yeni satır yerine NUL karakteri ile sınırlandırma (`xargs` yazılımı ile kullanırken işe yarar):
```shell
dirname --zero {{dosya_veya_dizine/giden/yol_1}} {{dosya_veya_dizine/giden/yol_2}}
```
{% endraw %}{% raw %}
<h2 id="dirs">
  <a href="/tr/common/dirs.html">dirs</a> <a href="#dirs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Dizin yığını görüntüler veya üzerinde oynama yapar.
> Dizin yığını, `pushd` ve `popd` komutlarıyla üzerinde oynama yapılabilen, son ziyaret edilen dizinleri gösteren bir listedir.
> Daha fazla bilgi için: <https://www.gnu.org/software/bash/manual/bash.html#Directory-Stack-Builtins>.

#### Dizin yığınını her madde arasında boşluk olacak şekilde görüntüle:
```shell
dirs
```
#### Dizin yığınını her satır başı tek madde olacak şekilde görüntüle:
```shell
dirs -p
```
#### Dizin yığınında 0'dan başlamak üzere yalnızca nth girişini göster:
```shell
dirs +{{N}}
```
#### Dizin yığınını temizle:
```shell
dirs -c
```
{% endraw %}{% raw %}
<h2 id="dirsearch">
  <a href="/tr/common/dirsearch.html">dirsearch</a> <a href="#dirsearch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Ağ yolu tarayıcı.
> Daha fazla bilgi için: <https://github.com/maurosoria/dirsearch>.

#### Bir ağ sunucusunu yaygın eklentiler içeren yaygın yollar için tarayın:
```shell
dirsearch --url {{url}} --extensions-list
```
#### Ağ sunucularını içeren bir listeyi `.php` eklentili yaygın yollar için tarayın:
```shell
dirsearch --url-list {{örnek/url-listesi.txt}} --extensions {{php}}
```
#### Bir ağ sunucusunu yaygın eklentiler içeren belirtilen yollar için tarayın:
```shell
dirsearch --url {{url}} --extensions-list --wordlist {{path/to/url-yol-listesi.txt}}
```
#### Bir ağ sunucusunu çerez kullanarak tarayın:
```shell
dirsearch --url {{url}} --extensions {{php}} --cookie {{cookie}}
```
#### Bir ağ sunucusunu `HEAD` HTTP metodunu kullanarak tarayın:
```shell
dirsearch --url {{url}} --extensions {{php}} --http-method {{HEAD}}
```
#### Bir ağ sunucusunu tarayın ve sonuçları bir `.json` dosyasına kaydedin:
```shell
dirsearch --url {{url}} --extensions {{php}} --json-report {{örnek/rapor_dosyası.json}}
```
{% endraw %}{% raw %}
<h2 id="docker-build">
  <a href="/tr/common/docker-build.html">docker build</a> <a href="#docker-build"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bir Dockerfile'dan imge yaratın.
> Daha fazla bilgi için: <https://docs.docker.com/engine/reference/commandline/build/>.

#### Mevcut dizindeki Dockerfile'dan bir docker imgesi oluşturun:
```shell
docker build .
```
#### Belirtilen URL'deki Dockerfile'dan bir docker imgesi oluşturun:
```shell
docker build {{ornekadres.com/ornek-dizin/ornek-docker-projesi}}
```
#### Bir docker imgesi oluşturun ve etiketleyin:
```shell
docker build --tag {{isim:etiket}} .
```
#### İmge oluştururken çerez kullanımını etkisizleştirin:
```shell
docker build --no-cache --tag {{isim:etiket}} .
```
#### Belirtilen Dockerfile ile bir docker imgesi oluşturun:
```shell
docker build --file {{Dockerfile}} .
```
#### Kişiselleştirilmiş yapım-zaman değerleriyle oluşturun:
```shell
docker build --build-arg {{HTTP_PROXY=http://10.20.30.2:1234}} --build-arg {{FTP_PROXY=http://40.50.60.5:4567}} .
```
{% endraw %}{% raw %}
<h2 id="docker-compose">
  <a href="/tr/common/docker-compose.html">docker compose</a> <a href="#docker-compose"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Çoklu konteynerli docker uygulamalarını çalıştırın ve yönetin.
> Daha fazla bilgi için: <https://docs.docker.com/compose/reference/overview/>.

#### Tüm konteynerleri listele:
```shell
docker-compose ps
```
#### Mevcut dizinde bir `docker-compose.yml` dosyası çalıştırarak arkaplandaki tüm konteynerleri çalıştırın ve başlatın:
```shell
docker-compose up -d
```
#### Tüm konteynerleri çalıştırın ve gerekiyorsa yeniden oluşturun:
```shell
docker-compose up --build
```
#### Tüm konteynerleri alternatif bir beste dosyasıyla başlatın:
```shell
docker-compose --file {{yoldan/dosyaya}} up
```
#### Çalışan tüm konteynerleri durdurun:
```shell
docker-compose stop
```
#### Tüm konteynerleri, ağları, imgeleri ve alanları durdurun ve silin:
```shell
docker-compose down --rmi all --volumes
```
#### Tüm konteynerler için logları takip edin:
```shell
docker-compose logs --follow
```
#### Belirtilmiş bir konteyner için logları takip edin:
```shell
docker-compose logs --follow {{konteyner_ismi}}
```
{% endraw %}{% raw %}
<h2 id="docker-exec">
  <a href="/tr/common/docker-exec.html">docker exec</a> <a href="#docker-exec"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Halihazırda çalışan bir Docker konteyneri üstünde komut çalıştır.
> Daha fazla bilgi için: <https://docs.docker.com/engine/reference/komutline/exec/>.

#### Halihazırda çalışan bir konteynerin üstünde interaktif bir kabuk oturumunu çalıştır:
```shell
docker exec --interactive --tty {{konteyner_ismi}} {{/bin/bash}}
```
#### Halihazırda çalışan bir konteynerin üstüne arkaplanda çalışmak üzere (ayrılmış) bir komut çalıştır:
```shell
docker exec --detach {{konteyner_ismi}} {{komut}}
```
#### Belirtilen bir komutu üstünde çalıştırmak adına çalışan dizini seç:
```shell
docker exec --interactive -tty --workdir {{örnek/dizin}} {{konteyner_ismi}} {{komut}}
```
#### Varolan konteyner üstünde arkaplanda çalışmak üzere bir komut çalıştır ancak stdin'i açık tut:
```shell
docker exec --interactive --detach {{konteyner_ismi}} {{komut}}
```
#### Çalışmakta olan bir bash oturumu içinde bir çevre değişkeni belirle:
```shell
docker exec --interactive --tty --env {{değişken_ismi}}={{value}} {{konteyner_ismi}} {{/bin/bash}}
```
#### Belirtilmiş bir kullanıcı olarak komut çalıştır:
```shell
docker exec --user {{kullanıcı}} {{konteyner_ismi}} {{komut}}
```
{% endraw %}{% raw %}
<h2 id="docker-images">
  <a href="/tr/common/docker-images.html">docker images</a> <a href="#docker-images"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Docker imgelerini yönet.
> Daha fazla bilgi için: <https://docs.docker.com/engine/reference/commandline/images/>.

#### Tüm Docker imgelerini listele:
```shell
docker images
```
#### Orta düzeyler de dahil olmak üzere tüm Docker imgelerini sırala:
```shell
docker images --all
```
#### Çıktıyı sessiz modda (yalnızca sayısal ID'ler olarak) sırala:
```shell
docker images --quiet
```
#### Herhangi bir konteyner tarafından kullanılmayan tüm Docker imgelerini sırala:
```shell
docker images --filter dangling=true
```
#### İsminde belirtilen dizeleri taşıyan imgeleri sırala:
```shell
docker images "{{*isim*}}"
```
{% endraw %}{% raw %}
<h2 id="docker-inspect">
  <a href="/tr/common/docker-inspect.html">docker inspect</a> <a href="#docker-inspect"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Docker objelerinde bulunan düşük seviye bilgiyi gösterir.
> Daha fazla bilgi için: <https://docs.docker.com/engine/reference/commandline/inspect/>.

#### Yardım içeriğini göster:
```shell
docker inspect
```
#### Bir konteyner, imge veya hacim ile ilgili bilgiyi ismini veya ID'sini girerek görüntüle:
```shell
docker inspect {{konteyner|imge|ID}}
```
#### Bir konteynerin IP adresini görüntüle:
```shell
docker inspect --format='{{range .NetworkSettings.Networks}}{{.IPAddress}}{{end}}' {{konteyner}}
```
#### Konteynerin log dosyasının yolunu görüntüle:
```shell
docker inspect --format='{{.LogPath}}' {{konteyner}}
```
#### Konteynerin imge ismini görüntüle:
```shell
docker inspect --format='{{.Config.Image}}' {{konteyner}}
```
#### Konfigürasyon bilgisini JSON olarak görüntüle:
```shell
docker inspect --format='{{json .Config}}' {{konteyner}}
```
#### Tüm port limanlayıcıları görüntüle:
```shell
docker inspect --format='{{range $p, $conf := .NetworkSettings.Ports}} {{$p}} -> {{(index $conf 0).HostPort}} {{end}}' {{konteyner}}
```
{% endraw %}{% raw %}
<h2 id="docker-logs">
  <a href="/tr/common/docker-logs.html">docker logs</a> <a href="#docker-logs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Konteyner kaydını yazdırır.
> Daha fazla bilgi için: <https://docs.docker.com/engine/reference/commandline/logs>.

#### Bir konteyner içindeki kayıtları yazdır:
```shell
docker logs {{konteyner_ismi}}
```
#### Kayıtları yazdır ve izle:
```shell
docker logs -f {{konteyner_ismi}}
```
#### Son 5 kaydı yazdır:
```shell
docker logs {{konteyner_ismi}} --tail {{5}}
```
#### Kayıtları yazdır ve zaman damgaları ile iliştir:
```shell
docker logs -t {{konteyner_ismi}}
```
#### Belli bir konteyner çalışma zamanındaki (i.e. 23m, 10s, 2013-01-02T13:23:37) kayıtları yazdır:
```shell
docker logs {{konteyner_ismi}} --until {{zaman}}
```
{% endraw %}{% raw %}
<h2 id="docker-machine">
  <a href="/tr/common/docker-machine.html">docker-machine</a> <a href="#docker-machine"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Docker çalıştıran makineler oluştur ve onları yönet.
> Daha fazla bilgi için: <https://docs.docker.com/machine/reference/>.

#### Halihazırda çalışan docker makinelerini sırala:
```shell
docker-machine ls
```
#### Belirli bir isim ile docker makinesi oluştur:
```shell
docker-machine create {{isim}}
```
#### Bir makinenin durumunu öğren:
```shell
docker-machine status {{isim}}
```
#### Bir makineyi başlat:
```shell
docker-machine start {{isim}}
```
#### Bir makineyi durdur:
```shell
docker-machine stop {{isim}}
```
#### Bir makine hakkındaki bilgileri incele:
```shell
docker-machine inspect {{isim}}
```
{% endraw %}{% raw %}
<h2 id="docker-network">
  <a href="/tr/common/docker-network.html">docker network</a> <a href="#docker-network"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Docker ağları oluştur ve yönet.
> Daha fazla bilgi için: <https://docs.docker.com/engine/reference/commandline/network/>.

#### docker daemon'daki tüm müsait ve düzenlenmiş ağları sırala:
```shell
docker network ls
```
#### Kullanıcı tarafından belirtilmiş bir ağ oluştur:
```shell
docker network create --driver {{driver_name}} {{ağ_ismi}}
```
#### Boşluk ile ayrılmış bir ağ listesinin detaylı bilgisini görüntüle:
```shell
docker network inspect {{ağ_ismi}}
```
#### Bir konteyneri isim veya ID kullanarak bir ağa bağla:
```shell
docker network connect {{ağ_ismi}} {{konteyner_ismi|ID}}
```
#### Bir konteyneri bir ağdan çıkar:
```shell
docker network disconnect {{ağ_ismi}} {{konteyner_ismi|ID}}
```
#### Tüm kullanılmayan (hiçbir konteyner tarafından belirtilmeyen) ağları sil:
```shell
docker network prune
```
#### Kullanılmayan ağların boşluk ile ayrılmış bir listesini sil:
```shell
docker network rm {{ağ_ismi}}
```
{% endraw %}{% raw %}
<h2 id="docker-ps">
  <a href="/tr/common/docker-ps.html">docker ps</a> <a href="#docker-ps"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Docker konteynerlerini sırala.
> Daha fazla bilgi için: <https://docs.docker.com/engine/reference/commandline/ps/>.

#### Halihazırda çalışan docker konteynerlerini listele:
```shell
docker ps
```
#### Tüm (durmuş veya çalışan) docker konteynerlerini listele:
```shell
docker ps --all
```
#### En son oluşturulan (durmuş veya çalışan) konteynerleri listele:
```shell
docker ps --latest
```
#### İsimlerinde belirtilen dizeleri içeren konteynerleri filtrele:
```shell
docker ps --filter="name={{isim}}"
```
#### Belirtilen imge ile akrabalık taşıyan konteynerleri filtrele:
```shell
docker ps --filter "ancestor={{imge}}:{{tag}}"
```
#### Konteynerleri çıkış durum koduna göre filtrele:
```shell
docker ps --all --filter="exited={{kod}}"
```
#### Konteynerleri mevcut durumlarına (oluşturulma, çalışma, silinme, durma, çıkma ve ölme) göre sırala:
```shell
docker ps --filter="status={{mevcut_durum}}"
```
#### Belirtilmiş bir hacmi gömen veya belirtilmiş bir yola gömülmüş hacmi içeren konteynerleri filtrele:
```shell
docker ps --filter="volume={{örnek/dizin}}" --format "table {{.ID}}\t{{.Image}}\t{{.Names}}\t{{.Mounts}}"
```
{% endraw %}{% raw %}
<h2 id="docker-rmi">
  <a href="/tr/common/docker-rmi.html">docker rmi</a> <a href="#docker-rmi"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bir veya daha fazla Docker imgesini sil.
> Daha fazla bilgi için: <https://docs.docker.com/engine/reference/commandline/rmi/>.

#### Yardım göster:
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
#### Bir imgeyi etiketlenmemiş ana yollarını silmeden sil:
```shell
docker rmi --no-prune {{imge}}
```
{% endraw %}{% raw %}
<h2 id="docker-run">
  <a href="/tr/common/docker-run.html">docker run</a> <a href="#docker-run"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Yeni bir Docker konteynerinde bir komut çalıştır.
> Daha fazla bilgi: <https://docs.docker.com/engine/reference/commandline/run/>.

#### Yeni bir konteynerde, etiketlenmiş bir imgeden komut çalıştır.:
```shell
docker run {{imge:etiket}} {{komut}}
```
#### Yeni bir konteynerde arkaplanda çalışacak şekilde komut çalıştır ve ID'sini göster:
```shell
docker run -d {{imge}} {{komut}}
```
#### İnteraktif mod ve pseudo-TTY'deki bir açık-kapalı konteynerde komut çalıştır:
```shell
docker run --rm -it {{imge}} {{komut}}
```
#### Yeni bir konteynerde geçebilmiş çevresel değişkenler ile komut çalıştır:
```shell
docker run -e '{{değişken}}={{değer}}' -e {{değişken}} {{imge}} {{komut}}
```
#### Yeni bir konteynerde bağlama takılı hacimlerle komut çalıştır:
```shell
docker run -v {{örnek/host}}:{{örnek/konteyner}} {{imge}} {{komut}}
```
#### Yayınlanmış portları içeren yeni bir konteynerde komut çalıştır:
```shell
docker run -p {{host_portu}}:{{konteyner_portu}} {{imge}} {{komut}}
```
{% endraw %}{% raw %}
<h2 id="docker-save">
  <a href="/tr/common/docker-save.html">docker save</a> <a href="#docker-save"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bir veya daha fazla docker imgesini arşivlemek için dışa aktar.
> Daha fazla bilgi için: <https://docs.docker.com/engine/reference/commandline/save/>.

#### Bir imgeyi, stdout'u tar arşivine yönlendirerek kaydet:
```shell
docker save {{imge}}:{{etiket}} > {örnek/dosya.tar}}
```
#### Bir imgeyi, bir tar arşivine kaydet:
```shell
docker save --output {{örnek/dosya.tar}} {{imge}}:{{etiket}}
```
#### Bir imgenin tüm etiketlerini kaydet:
```shell
docker save --output {{örnek/dosya.tar}} {{imge_ismi}}
```
#### Bir imgenin belirli etiketlerini kaydetmek için elle seç:
```shell
docker save --output {{örnek/dosya.tar}} {{imge_ismi:etiket1 imge_ismi:etiket2 ...}}
```
{% endraw %}{% raw %}
<h2 id="docker-secret">
  <a href="/tr/common/docker-secret.html">docker secret</a> <a href="#docker-secret"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Docker swarm sırlarını yönet.
> Daha fazla bilgi için: <https://docs.docker.com/engine/reference/commandline/secret/>.

#### stdin'den yeni bir sır yarat:
```shell
{{komut}} | docker secret create {{sır_ismi}} -
```
#### Bir dosyadan yeni sır oluşturun:
```shell
docker secret create {{sır_ismi}} {{örnek/dosya}}
```
#### Tüm sırları sırala:
```shell
docker secret ls
```
#### Bir veya daha fazla sırra dair detaylı bilgiyi insan dostu bir formatta göster:
```shell
docker secret inspect --pretty {{sır_ismi1 sır_ismi2 ...}}
```
#### Bir veya daha fazla sırrı sil:
```shell
docker secret rm {{sır_ismi1 sır_ismi2 ...}}
```
{% endraw %}{% raw %}
<h2 id="docker-service">
  <a href="/tr/common/docker-service.html">docker service</a> <a href="#docker-service"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bir docker daemon'unun üzerindeki servisleri yönet.
> Daha fazla bilgi için: <https://docs.docker.com/engine/reference/commandline/service/>.

#### Bir docker daeomon'unun üzerindeki servisleri listele:
```shell
docker service ls
```
#### Yeni bir servis yarat:
```shell
docker service create --name {{servis_ismi}} {{imge}}:{{etiket}}
```
#### Boşluk ile ayrılmış bir servis listesinin detaylı bilgisini görüntüle:
```shell
docker service inspect {{servis_ismi|ID}}
```
#### Boşluk ile ayrılmış bir servis listesinin görevlerini sırala:
```shell
docker service ps {{servis_ismi|ID}}
```
#### Boşluk ile ayrılmış bir servis listesi için belirli bir replika miktarına yüksel:
```shell
docker service scale {{servis_ismi}}={{replika_miktarı}}
```
#### Boşluk ile ayrılmış bir servis listesini sil:
```shell
docker service rm {{servis_ismi|ID}}
```
{% endraw %}{% raw %}
<h2 id="docker-start">
  <a href="/tr/common/docker-start.html">docker start</a> <a href="#docker-start"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bir veya daha fazla durmuş konteyneri başlar.
> Daha fazla bilgi için: <https://docs.docker.com/engine/reference/commandline/start/>.

#### Yardım göster:
```shell
docker start
```
#### Bir docker konteynerini başlat:
```shell
docker start {{konteyner}}
```
#### Bir konteyneri, ona stdout ile stderr'i ekleyerek ve sinyaller göndererek başlat:
```shell
docker start --attach {{konteyner}}
```
#### Bir veya daha fazla boşlukla ayrılarak belirtilmiş konteynerleri başlar:
```shell
docker start {{konteyner(ler)}}
```
{% endraw %}{% raw %}
<h2 id="docker-stats">
  <a href="/tr/common/docker-stats.html">docker stats</a> <a href="#docker-stats"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Konteynerler için kaynak kullanım istatistiklerinin canlı yayınını görüntüle.
> Daha fazla bilgi için: <https://docs.docker.com/engine/reference/commandline/stats/>.

#### Çalışan tüm konteynerlerin aynak kullanım istatistiklerinin canlı yayınını görüntüle:
```shell
docker stats
```
#### Boşluk ile ayrılmış bir listedeki konteynerlerin canlı yayınını görüntüle:
```shell
docker stats {{container_ismi}}
```
#### Konteyner'in CPU kullanım yüzdesini göstermek için sütun formatını değiştir:
```shell
docker stats --format "{{.Name}}:\t{{.CPUPerc}}"
```
#### Tüm (çalışan veya durmuş) konteynerler için istatistikleri görüntüle:
```shell
docker stats --all
```
#### İstatistikleri canlı yayınlamayı durdur ve yalnızca mevcut durumdaki istatistikleri görüntüle:
```shell
docker stats --no-stream
```
{% endraw %}{% raw %}
<h2 id="docker-swarm">
  <a href="/tr/common/docker-swarm.html">docker swarm</a> <a href="#docker-swarm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bir konteyner orkestrasyon aracı.
> Daha fazla bilgi için: <https://docs.docker.com/engine/swarm/>.

#### Bir bataklık dizisi oluştur:
```shell
docker swarm init
```
#### Bir yönetici veya işçiye takılmak için token göster:
```shell
docker swarm join-token {{işçi|yönetici}}
```
#### Diziye yeni bir düğüm ekle:
```shell
docker swarm join --token {{token}} {{manager_node_url:2377}}
```
#### Bir işçiyi bataklıktan sil (işçi düğümünün içinde çalıştır):
```shell
docker swarm leave
```
#### Mevcut CA sertifikasını PEM formatında görüntüle:
```shell
docker swarm ca
```
#### Mevcut CA sertifikasını döndür ve yeni sertifikayı görüntüle:
```shell
docker swarm ca --rotate
```
#### Düğüm sertifikaları için geçerli periyodu değiştir:
```shell
docker swarm update --cert-expiry {{saat}}h{{dakika}}m{{saniye}}s
```
{% endraw %}{% raw %}
<h2 id="docker-system">
  <a href="/tr/common/docker-system.html">docker system</a> <a href="#docker-system"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Docker verilerini yönet ve sistem bilgisi görüntüle.
> More information: <https://docs.docker.com/engine/reference/commandline/system/>.

#### Yardım göster:
```shell
docker system
```
#### Docker disk kullanımını göster:
```shell
docker system df
```
#### Disk kullanımı üzerine detaylı bilgi göster:
```shell
docker system df --verbose
```
#### Kullanılmayan veriyi sil:
```shell
docker system prune
```
#### Kullanılmayan ve geçmişte birden çok kez oluşturulan veriyi sil:
```shell
docker system prune --filter="until={{saat}}h{{dakika}}m"
```
#### Docker deamon'dan tam-zamanlı eylemleri görüntüle:
```shell
docker system events
```
#### Geçerli JSON satırları olarak yayınlanan konteynerleden tam-zamanlı eylemleri göster:
```shell
docker system events --filter 'type=container' --format '{{json .}}'
```
#### Sistem bilgisi göster:
```shell
docker system info
```
{% endraw %}{% raw %}
<h2 id="docker">
  <a href="/tr/common/docker.html">docker</a> <a href="#docker"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Docker konteyner ve imgelerini yönetir.
> Daha fazla bilgi için: <https://docs.docker.com/engine/reference/commandline/cli/>.

#### Şuan çalışan docker konteynerlerini listele:
```shell
docker ps
```
#### Tüm (çalışan veya duran) docker konteynerlerini listele:
```shell
docker ps -a
```
#### Bir imgeden özel bir isimle konteyner başlat:
```shell
docker run --name {{konteyner_ismi}} {{imge}}
```
#### Varolan bir konteyneri başlat veya durdur:
```shell
docker {{baslat|durdur}} {{konteyner_ismi}}
```
#### Bir docker kaydından imge çek:
```shell
docker pull {{imge}}
```
#### Halihazırda çalışan bir konteyner içinde komut istemcisi aç:
```shell
docker exec -it {{konteyner_ismi}} {{sh}}
```
#### Durmuş bir konteyneri sil:
```shell
docker rm {{konteyner_ismi}}
```
#### Bir konteynerin kaydını çek ve takip et:
```shell
docker logs -f {{konteyner_ismi}}
```
{% endraw %}{% raw %}
<h2 id="man">
  <a href="/tr/common/man.html">man</a> <a href="#man"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Kılavuz sayfalarını biçimlendir ve göster.
> Daha fazla bilgi için: <https://www.man7.org/linux/man-pages/man1/man.1.html>.

#### Bir komut için man sayfasını görüntüle:
```shell
man {{komut}}
```
#### Sayfanın 7. bölümündeki bir komut için man sayfasını görüntüle:
```shell
man {{komut}}.{{7}}
```
#### Mansayfaları için aratılan yolu göster:
```shell
man --path
```
#### Mansayfasını göstermek yerine mansayfasının konumunu göster:
```shell
man -w {{komut}}
```
#### Belirtilen ifadeyi içeren mansayfalarını ara:
```shell
man -k "{{aranan_ifade}}"
```
{% endraw %}{% raw %}
<h2 id="minetest">
  <a href="/tr/common/minetest.html">minetest</a> <a href="#minetest"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Çok oyunculu sınırsız dünyalı bloklu sandbox oyun motoru.
> Ayrıca `minetestserver` sayfasına bakılması önerilir.
> Daha fazla bilgi için: <https://wiki.minetest.net/Minetest>.

#### Minetest'i kullanıcı modunda başlat:
```shell
minetest
```
#### Minetest'i belirtilen dünyayı host edecek şekilde sunucu modunda başlat:
```shell
minetest --server --world {{isim}}
```
#### Belirtilmiş bir dosyaya geçmişi yaz:
```shell
minetest --logfile {{örnek/dosya}}
```
#### Hataları yalnızca konsola yaz:
```shell
minetest --quiet
```
{% endraw %}{% raw %}
<h2 id="minetestserver">
  <a href="/tr/common/minetestserver.html">minetestserver</a> <a href="#minetestserver"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Çok oyunculu sınırsız dünyalı bloklu sanbox sunucusu.
> Ayrıca `minetest` sayfasına bakılması önerilir.
> Daha fazla bilgi için: <https://wiki.minetest.net/Setting_up_a_server>.

#### Sunucuyu başlar:
```shell
minetestserver
```
#### Müsait dünyaları sırala:
```shell
minetestserver --world list
```
#### Yüklenecek dünya ismini belirt:
```shell
minetestserver --world {{dunya_ismi}}
```
#### Müsait oyun ID'lerini sırala:
```shell
minetestserver --gameid list
```
#### Kullanılacak oyunu belirt:
```shell
minetestserver --gameid {{oyun_id'si}}
```
#### Belirtilmiş bir port'u dinle:
```shell
minetestserver --port {{34567}}
```
#### Başka bir veritabanı yazılımına göç et:
```shell
minetestserver --migrate {{sqlite3|leveldb|redis}}
```
#### Sunucuyu başlattıktan sonra interaktif bir terminal aç:
```shell
minetestserver --terminal
```
{% endraw %}{% raw %}
<h2 id="tldr-lint">
  <a href="/tr/common/tldr-lint.html">tldr-lint</a> <a href="#tldr-lint"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> `tldr` sayfalarını gözden geçir ve biçimlendir.
> Daha fazla bilgi için: <https://github.com/tldr-pages/tldr-lint>.

#### Tüm sayfaları gözden geçir:
```shell
tldr-lint {{sayfa_dizini}}
```
#### Belirtilmiş bir sayfayı stdout'a biçimlendir:
```shell
tldr-lint --format {{page.md}}
```
#### Bir konumdaki tüm sayfaları biçimlendir:
```shell
tldr-lint --format --in-place {{sayfa_dizini}}
```
{% endraw %}{% raw %}
<h2 id="tldr">
  <a href="/tr/common/tldr.html">tldr</a> <a href="#tldr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Komut satırı araçları için tldr-pages projesinden basit yardım sayfaları görüntüler.
> Daha fazla bilgi için: <https://tldr.sh>.

#### Bir komutun tipik kullanımını göster (ipucu: burayı görüntülemek için kullandığınız komutun aynısı!):
```shell
tldr {{komut}}
```
#### Linux için tar tldr sayfasını göster:
```shell
tldr -p {{linux}} {{tar}}
```
#### Bir Git alt komutu için yardım al:
```shell
tldr {{git-checkout}}
```
#### (Eğer alıcı önbellek oluşumunu destekliyorsa) Yerel paketleri güncelle:
```shell
tldr -u
```
{% endraw %}{% raw %}
<h2 id="tldrl">
  <a href="/tr/common/tldrl.html">tldrl</a> <a href="#tldrl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> `tldr-lint` komutunun aynısı.

#### Orijinal komut için yardım sayfasını göster:
```shell
tldr tldr-lint
```
{% endraw %}