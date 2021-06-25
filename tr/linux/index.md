---
layout: default
title: "linux"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
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
{% endraw %}