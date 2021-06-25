---
layout: default
title: "common"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#2to3">2to3</a>
* <a href="#7z">7z</a>
* <a href="#7za">7za</a>
* <a href="#7zr">7zr</a>
* <a href="#aapt">aapt</a>
* <a href="#adb">adb</a>
* <a href="#adb-install">adb install</a>
* <a href="#adb-reverse">adb reverse</a>
* <a href="#adb-shell">adb shell</a>
* <a href="#alacritty">alacritty</a>
* <a href="#alias">alias</a>
* <a href="#apktool">apktool</a>
* <a href="#asar">asar</a>
* <a href="#cat">cat</a>
* <a href="#cd">cd</a>
* <a href="#cp">cp</a>
* <a href="#curl">curl</a>
* <a href="#deno">deno</a>
* <a href="#docker">docker</a>
* <a href="#git">git</a>
* <a href="#git-add">git add</a>
* <a href="#git-branch">git branch</a>
* <a href="#git-checkout">git checkout</a>
* <a href="#git-clone">git clone</a>
* <a href="#git-commit">git commit</a>
* <a href="#git-remote">git remote</a>
* <a href="#git-status">git status</a>
* <a href="#hugo">hugo</a>
* <a href="#java">java</a>
* <a href="#laravel">laravel</a>
* <a href="#laravel-zero">laravel-zero</a>
* <a href="#ls">ls</a>
* <a href="#mkdir">mkdir</a>
* <a href="#mongod">mongod</a>
* <a href="#mv">mv</a>
* <a href="#node">node</a>
* <a href="#npm">npm</a>
* <a href="#nvim">nvim</a>
* <a href="#nvm">nvm</a>
* <a href="#pip">pip</a>
* <a href="#pip3">pip3</a>
* <a href="#pwd">pwd</a>
* <a href="#python">python</a>
* <a href="#rm">rm</a>
* <a href="#scrcpy">scrcpy</a>
* <a href="#touch">touch</a>
* <a href="#vue">vue</a>
* <a href="#vue-build">vue build</a>
* <a href="#vue-init">vue init</a>
* <a href="#vue-serve">vue serve</a>
* <a href="#yarn">yarn</a>

{% raw %}
<h2 id="2to3">
  <a href="/id/common/2to3.html">2to3</a> <a href="#2to3"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mengkonversikan kode Python 2 menuju file Python 3 secara otomatis.
> Informasi lebih lanjut: <https://docs.python.org/3/library/2to3.html>.

#### Menampilkan apa saja yang akan diubah tanpa mengubahnya secara langsung (dry-run):
```shell
2to3 {{jalan/menuju/file.py}}
```
#### Mengkonversikan sebuah file Python 2 menuju file Python 3:
```shell
2to3 --write {{jalan/menuju/file.py}}
```
#### Mengkonversikan fitur bahasa pemrograman Python 2 tertentu menuju Python 3:
```shell
2to3 --write {{jalan/menuju/file.py}} --fix={{raw_input}} --fix={{print}}
```
#### Mengkonversikan seluruh fitur Python 2 menjadi Python 3, kecuali fitur-fitur tertentu:
```shell
2to3 --write {{jalan/menuju/file.py}} --nofix={{has_key}} --nofix={{isinstance}}
```
#### Menampilkan daftar fitur-fitur bahasa pemrograman yang dapat dikonversikan dari Python 2 menuju Python 3:
```shell
2to3 --list-fixes
```
#### Mengkonversikan seluruh file Python 2 menuju Python 3 di dalam sebuah direktori:
```shell
2to3 --output-dir={{jalan/menuju/direktori_python3}} --write-unchanged-files --nobackups {{jalan/menuju/direktori_python2}}
```
#### Menjalankan program ini dengan lebih dari satu thread:
```shell
2to3 --processes={{4}} --output-dir={{jalan/menuju/direktori_python3}} --write --nobackups --no-diff {{jalan/menuju/direktori_python2}}
```
{% endraw %}{% raw %}
<h2 id="7z">
  <a href="/id/common/7z.html">7z</a> <a href="#7z"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pengarsip file dengan rasio kompresi yang tinggi.
> Informasi lebih lanjut: <https://www.7-zip.org>.

#### Meng[a]rsipkan sebuah file atau direktori:
```shell
7z a {{jalan/menuju/arsip.7z}} {{jalan/menuju/file_atau_direktori}}
```
#### Mengenkripsi sebuah file arsip (termasuk nama-nama file yang terkandung di dalamnya):
```shell
7z a {{jalan/menuju/arsip_terenkripsi.7z}} -p{{kata sandi}} -mhe=on {{jalan/menuju/arsip.7z}}
```
#### Mengekstrak sebuah file arsip dengan mempertahankan struktur direktori asli:
```shell
7z x {{jalan/menuju/arsip.7z}}
```
#### Mengekstrak sebuah file arsip ke dalam direktori yang ditentukan:
```shell
7z x {{jalan/menuju/arsip.7z}} -o{{jalan/menuju/direktori}}
```
#### Mengekstrak sebuah file arsip menuju stdout:
```shell
7z x {{jalan/menuju/arsip.7z}} -so
```
#### Meng[a]rsipkan file atau direktori menggunakan format file arsip tertentu:
```shell
7z a -t{{7z|zip|gzip|bzip2|lzip}} {{jalan/menuju/arsip.7z}} {{jalan/menuju/file_atau_direktori}}
```
#### Me[l]ihat daftar isi dari sebuah file arsip:
```shell
7z l {{path/to/archive.7z}}
```
#### Mengetahui daftar format file arsip yang didukung:
```shell
7z i
```
{% endraw %}{% raw %}
<h2 id="7za">
  <a href="/id/common/7za.html">7za</a> <a href="#7za"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pengarsip file dengan rasio kompresi yang tinggi.
> Serupa dengan `7z` namun mendukung lebih sedikit format file arsip dan dapat digunakan lintas sistem operasi.
> Informasi lebih lanjut: <https://www.7-zip.org>.

#### Meng[a]rsipkan sebuah file atau direktori:
```shell
7za a {{jalan/menuju/arsip.7z}} {{jalan/menuju/file_atau_direktori}}
```
#### Mengenkripsi sebuah file arsip (termasuk nama-nama file yang terkandung di dalamnya):
```shell
7za a {{jalan/menuju/arsip_terenkripsi.7z}} -p{{kata sandi}} -mhe=on {{jalan/menuju/arsip.7z}}
```
#### Mengekstrak sebuah file arsip dengan mempertahankan struktur direktori asli:
```shell
7za x {{jalan/menuju/arsip.7z}}
```
#### Mengekstrak sebuah file arsip ke dalam direktori yang ditentukan:
```shell
7za x {{jalan/menuju/arsip.7z}} -o{{jalan/menuju/direktori}}
```
#### Mengekstrak sebuah file arsip menuju stdout:
```shell
7za x {{jalan/menuju/arsip.7z}} -so
```
#### Meng[a]rsipkan file atau direktori menggunakan format file arsip tertentu:
```shell
7za a -t{{7z|zip|gzip|bzip2|lzip}} {{jalan/menuju/arsip.7z}} {{jalan/menuju/file_atau_direktori}}
```
#### Me[l]ihat daftar isi dari sebuah file arsip:
```shell
7za l {{path/to/archive.7z}}
```
#### Mengetahui daftar format file arsip yang didukung:
```shell
7za i
```
{% endraw %}{% raw %}
<h2 id="7zr">
  <a href="/id/common/7zr.html">7zr</a> <a href="#7zr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pengarsip file dengan rasio kompresi yang tinggi.
> Serupa dengan `7z` namun mendukung format file arsip `.7z` saja.
> Informasi lebih lanjut: <https://www.7-zip.org>.

#### Meng[a]rsipkan sebuah file atau direktori:
```shell
7zr a {{jalan/menuju/arsip.7z}} {{jalan/menuju/file_atau_direktori}}
```
#### Mengenkripsi sebuah file arsip (termasuk nama-nama file yang terkandung di dalamnya):
```shell
7zr a {{jalan/menuju/arsip_terenkripsi.7z}} -p{{kata sandi}} -mhe=on {{jalan/menuju/arsip.7z}}
```
#### Mengekstrak sebuah file arsip dengan mempertahankan struktur direktori asli:
```shell
7zr x {{jalan/menuju/arsip.7z}}
```
#### Mengekstrak sebuah file arsip ke dalam direktori yang ditentukan:
```shell
7zr x {{jalan/menuju/arsip.7z}} -o{{jalan/menuju/direktori}}
```
#### Mengekstrak sebuah file arsip menuju stdout:
```shell
7zr x {{jalan/menuju/arsip.7z}} -so
```
#### Me[l]ihat daftar isi dari sebuah file arsip:
```shell
7zr l {{path/to/archive.7z}}
```
#### Mengetahui daftar format file arsip yang didukung:
```shell
7zr i
```
{% endraw %}{% raw %}
<h2 id="aapt">
  <a href="/id/common/aapt.html">aapt</a> <a href="#aapt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Alat Pemaketan Android Asset.
> Menyusun dan memaketkan resource aplikasi Android.

#### Daftar berkas-berkas yang termuat dalam arsip APK:
```shell
aapt list {{alamat/ke/aplikasi.apk}}
```
#### Menampilkan metadata aplikasi (versi, izin, dsb.):
```shell
aapt dump badging {{alamat/ke/aplikasi.apk}}
```
#### Membuat arsip APK baru dengan berkas dari direktory yang ditentukan:
```shell
aapt package -F {{alamat/ke/aplikasi.apk}} {{alamat/ke/direktori}}
```
{% endraw %}{% raw %}
<h2 id="adb-install">
  <a href="/id/common/adb-install.html">adb install</a> <a href="#adb-install"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge Install: Menginstal paket ke emulator Android atau perangkat Android terhubung.
> Informasi lebih lanjut: <https://developer.android.com/studio/command-line/adb>.

#### Menginstal aplikasi Android ke emulator/perangkat:
```shell
adb install {{alamat/ke/berkas.apk}}
```
#### Menginstal ulang aplikasi yang sudah ada, menjaga datanya:
```shell
adb install -r {{alamat/ke/berkas.apk}}
```
#### Memberikan semua izin yang terdaftar di manifest aplikasi:
```shell
adb install -g {{alamat/ke/berkas.apk}}
```
#### Memperbarui langsung paket terinstal dengan hanya memperbarui bagian dari APK yang berubah:
```shell
Adb install --fastdeploy {{alamat/ke/berkas.apk}}
```
{% endraw %}{% raw %}
<h2 id="adb-reverse">
  <a href="/id/common/adb-reverse.html">adb reverse</a> <a href="#adb-reverse"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge Reverse: membalik koneksi socket dari emulator Android atau perangkat Android terhubung.
> Informasi lebih lanjut: <https://developer.android.com/studio/command-line/adb>.

#### Daftar semua koneksi socket terbalik dari emulator dan perangkat:
```shell
adb reverse --list
```
#### Membalik port TCP dari emulator/perangkat ke localhost:
```shell
adb reverse tcp:{{port_jarak_jauh}} tcp:{{port_lokal}}
```
#### Melepas koneksi socket terbalik dari emulator/perangkat:
```shell
adb reverse --remove tcp:{{port_jarak_jauh}}
```
#### Melepas semua koneksi socket terbalik dari semua emulator dan perangkat:
```shell
adb reverse --remove-all
```
{% endraw %}{% raw %}
<h2 id="adb-shell">
  <a href="/id/common/adb-shell.html">adb shell</a> <a href="#adb-shell"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge Shell: Menjalankan perintah shell jarak jauh pada emulator Android atau perangkat Android terhubung.
> Informasi lebih lanjut: <https://developer.android.com/studio/command-line/adb>.

#### Memulai shell interaktif jarak jauh di emulator/perangkat:
```shell
adb shell
```
#### Mendapatkan semua properti dari emulator/perangkat:
```shell
adb shell getprop
```
#### Mengembalikan semua izin runtime ke default:
```shell
adb shell pm reset-permissions
```
#### Mencabut izin berbahaya dari sebuah aplikasi:
```shell
adb shell pm revoke {{paket}} {{izin}}
```
#### Memicu sebuah peristiwa penting:
```shell
adb shell input keyevent {{keycode}}
```
#### Mengosongkan data aplikasi pada emulator/perangkat:
```shell
adb shell pm clear {{paket}}
```
#### Memulai aktivitas pada emulator/perangkat:
```shell
adb shell am start -n {{paket}}/{{aktivitas}}
```
#### Memulai aktivitas beranda pada emulator/perangkat:
```shell
adb shell am start -W -c android.intent.category.HOME -a android.intent.action.MAIN
```
{% endraw %}{% raw %}
<h2 id="adb">
  <a href="/id/common/adb.html">adb</a> <a href="#adb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Android Debug Bridge: berkomunikasi dengan emulator Android atau perangkat Android terhubung.
> Informasi lebih lanjut: <https://developer.android.com/studio/command-line/adb>.

#### Cek apakah proses server adb telah dimulai dan memulainya:
```shell
adb start-server
```
#### Menghentikan proses server adb:
```shell
adb kill-server
```
#### Memulai shell jarak jauh pada emulator/perangkat tujuan:
```shell
adb shell
```
#### Menginstal aplikasi Android ke emulator/perangkat tujuan:
```shell
adb install -r {{alamat/ke/berkas.apk}}
```
#### Menyalin berkas/direktori dari perangkat tujuan:
```shell
adb pull {{alamat/ke/berkas_atau_direktori_perangkat}} {{alamat/ke/direktori_lokal_tujuan}}
```
#### Menyalin berkas/direktori ke perangkat tujuan:
```shell
adb push {{alamat/ke/berkas_atau_direktori_lokal}} {{alamat/ke/direktori_perangkat_tujuan}}
```
#### Mendapatkan daftar perangkat yang terhubung:
```shell
adb devices
```
{% endraw %}{% raw %}
<h2 id="alacritty">
  <a href="/id/common/alacritty.html">alacritty</a> <a href="#alacritty"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lintas platform, terakselerasi GPU terminal emulator.
> Informasi lebih lanjut: <https://github.com/alacritty/alacritty>.

#### Membuka jendela Alacritty baru:
```shell
alacritty
```
#### Menjalankan Alacritty pada direktori tertentu:
```shell
alacritty --working-directory {{alamat/ke/direktori}}
```
#### Menjalankan perintah di jendela Alacritty baru:
```shell
alacritty -e {{perintah}}
```
#### Menentukan berkas konfigurasi alternatif (nilai default `$XDG_CONFIG_HOME/alacritty/alacritty.yml`):
```shell
alacritty --config-file {{alamat/ke/konfigurasi.yml}}
```
#### Menjalankan dengan mengaktifkan pemuatan ulang konfigurasi secara langsung/otomatis (dapat juga diaktifkan secara default di `alacritty.yml`):
```shell
alacritty --live-config-reload --config-file {{alamat/ke/konfigurasi.yml}}
```
{% endraw %}{% raw %}
<h2 id="alias">
  <a href="/id/common/alias.html">alias</a> <a href="#alias"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Membuat alias -- kata-kata yang digantikan oleh utasan perintah (command).
> Alias menjadi kadaluarsa sampai sesi shell saat ini berakhir, kecuali jika didefinisikan di file konfigurasi shell, misalnya `~/.bashrc`.
> Informasi lebih lanjut: <https://tldp.org/LDP/abs/html/aliases.html>.

#### Menampilkan daftar semua alias:
```shell
alias
```
#### Membuat alias generik:
```shell
alias {{kata}}="{{perintah}}"
```
#### Melihat perintah yang dirujuk oleh alias yang diberikan:
```shell
alias {{kata}}
```
#### Menghapus alias dari sebuah perintah:
```shell
unalias {{kata}}
```
#### Mengubah `rm` menjadi perintah interaktif:
```shell
alias {{rm}}="{{rm -i}}"
```
#### Membuat `la` menjadi pintasan untuk `ls -a`:
```shell
alias {{la}}="{{ls -a}}"
```
{% endraw %}{% raw %}
<h2 id="apktool">
  <a href="/id/common/apktool.html">apktool</a> <a href="#apktool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Me-reverse engineer berkas APK.
> Informasi lebih lanjut: <https://ibotpeaches.github.io/Apktool/>.

#### Dekode berkas APK:
```shell
apktool d {{berkas.apk}}
```
#### Men-build folder menjadi berkas APK:
```shell
apktool b {{alamat/ke/direktori}}
```
#### Menginstal dan menyimpan frameworks:
```shell
apktool if {{framework.apk}}
```
{% endraw %}{% raw %}
<h2 id="asar">
  <a href="/id/common/asar.html">asar</a> <a href="#asar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pengarsip berkas untuk platform Electron.
> Informasi lebih lanjut: <https://github.com/electron/asar>.

#### Arsipkan sebuah berkas atau direktori:
```shell
asar pack {{alamat/ke/berkas_atau_direktori}} {{arsip.asar}}
```
#### Mengekstrak sebuah arsip:
```shell
asar extract {{arsip.asar}}
```
#### Mengekstrak berkas tertentu dari sebuah arsip:
```shell
asar extract-file {{arsip.asar}} {berkas}}
```
#### Mendapatkan daftar konten dari berkas arsip:
```shell
asar list {{arsip.asar}}
```
{% endraw %}{% raw %}
<h2 id="cat">
  <a href="/id/common/cat.html">cat</a> <a href="#cat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mencetak dan menggabungkan berkas.
> Informasi lebih lanjut: <https://www.gnu.org/software/coreutils/cat>.

#### Mencetak konten berkas ke keluaran standar:
```shell
cat {{berkas}}
```
#### Menggabungkan konten beberapa berkas ke berkas tujuan:
```shell
cat {{berkas1}} {{berkasw}} > {{berkas_tujuan}}
```
#### Menambahkan konten beberapa berkas ke berkas tujuan:
```shell
cat {{berkas1}} {{berkas2}} >> {{berkas_tujuan}}
```
#### Memberi nomor pada semua baris keluaran:
```shell
cat -n {{berkas}}
```
#### Menampilkan karakter yang tidak dapat dicetak dan spasi (dengan awalan `M-`jika non-ASCII):
```shell
cat -v -t -e {{berkas}}
```
{% endraw %}{% raw %}
<h2 id="cd">
  <a href="/id/common/cd.html">cd</a> <a href="#cd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mengganti direktori yang dikunjungi saat ini.
> Informasi lebih lanjut: <https://man.archlinux.org/man/cd.n>.

#### Menuju ke direktori yang telah ditentukan:
```shell
cd {{lokasi/ke/direktori}}
```
#### Menuju ke direktori pangkal/home milik pengguna:
```shell
cd
```
#### Menuju ke induk direktori dari direktori saat ini:
```shell
cd ..
```
#### Menuju direktori yang telah dikunjungi sebelumnya:
```shell
cd -
```
{% endraw %}{% raw %}
<h2 id="cp">
  <a href="/id/common/cp.html">cp</a> <a href="#cp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Membuat salinan file dan direktori.
> Informasi lebih lanjut: <https://www.gnu.org/software/coreutils/cp>.

#### Membuat salinan file ke lokasi lain:
```shell
cp {{jalan/menuju/file_sumber.ext}} {{jalan/menuju/file_tujuan.ext}}
```
#### Menyalin file ke direktori lain, dengan nama yang sama:
```shell
cp {{jalan/menuju/file_sumber.ext}} {{jalan/menuju/direktori_tujuan}}
```
#### Menyalin sebuah direktori secara beserta isinya ke lokasi lain (jika tujuan sudah ada, direktori tersebut disalin ke dalamnya):
```shell
cp -R {{jalan/menuju/direktori_sumber}} {{jalan/menuju/direktori_tujuan}}
```
#### Menyalin sebuah direktori secara beserta isinya, dalam mode `verbose` (menampilkan file-file ketika disalin):
```shell
cp -vR {{jalan/menuju/direktori_sumber}} {{jalan/menuju/direktori_tujuan}}
```
#### Menyalin file-file teks ke lokasi lain, dalam mode interaktif (menampilkan pertanyaan sebelum menimpa):
```shell
cp -i {{*.txt}} {{jalan/menuju/direktori_tujuan}}
```
#### Melepaskan tautan simbolis sebelum menyalin:
```shell
cp -L {{tautan}} {{jalan/menuju/direktori_tujuan}}
```
{% endraw %}{% raw %}
<h2 id="curl">
  <a href="/id/common/curl.html">curl</a> <a href="#curl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mentransfer data dari atau ke server.
> Mendukung sebagian besar protokol, termasuk HTTP, FTP, dan POP3.
> Informasi lebih lanjut: <https://curl.se>.

#### Unduh konten URL ke file:
```shell
curl {{http://contoh.com}} --output {{namafile}}
```
#### Unduh file, simpan hasilnya dengan nama file yang ditentukan oleh URL:
```shell
curl --remote-name {{http://contoh.com/namafile}}
```
#### Unduh file, mengikuti pengalihan lokasi, dan secara otomatis melanjutkan transfer file sebelumnya:
```shell
curl --remote-name --location --continue-at - {{http://contoh.com/filename}}
```
#### Mengirim data form yang telah di encode (permintaan POST atau tipe data `application/x-www-form-urlencoded`). Gunakan `--data @file_name` atau `--data @'-'` untuk membaca dari STDIN:
```shell
curl --data {{'name=bob'}} {{http://contoh.com/form}}
```
#### Mengirim sebuah permintaan dengan header tambahan, menggunakan metode HTTP kustom:
```shell
curl --header {{'X-My-Header: 123'}} --request {{PUT}} {{http://contoh.com}}
```
#### Mengirim data dalam format JSON, Menentukan jenis konten yang sesuai header:
```shell
curl --data {{'{"name":"bob"}'}} --header {{'Content-Type: application/json'}} {{http://contoh.com/users/1234}}
```
#### Memberikan nama pengguna dan kata sandi untuk otentikasi server:
```shell
curl --user myusername:mypassword {{http://contoh.com}}
```
#### Memberikan sertifikat klien dan kunci untuk sumber daya, melewati validasi sertifikat:
```shell
curl --cert {{client.pem}} --key {{key.pem}} --insecure {{https://contoh.com}}
```
{% endraw %}{% raw %}
<h2 id="deno">
  <a href="/id/common/deno.html">deno</a> <a href="#deno"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Runtime aman untuk JavaScript dan TypeScript.
> Informasi lebih lanjut: <https://deno.land/>.

#### Menjalankan berkas JavaScript atau TypeScript:
```shell
deno run {{alamat/ke/berkas.ts}}
```
#### Menjalankan REPL (shell interaktif):
```shell
deno
```
#### Menjalankan berkas dengan memperbolehkan akses jaringan:
```shell
deno run --allow-net {{alamat/ke/berkas.ts}}
```
#### Menjalankan berkas dari URL:
```shell
deno run {{https://deno.land/std/examples/welcome.ts}}
```
#### Memasang skrip yang dapat dieksekusi dari URL:
```shell
deno install {{https://deno.land/std/examples/colors.ts}}
```
{% endraw %}{% raw %}
<h2 id="docker">
  <a href="/id/common/docker.html">docker</a> <a href="#docker"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mengatur kontainer Docker dan image.
> Informasi lebih lanjut: <https://docs.docker.com/engine/reference/commandline/cli/>.

#### Menampilkan semua daftar kontainer docker yang sedang berjalan:
```shell
docker ps
```
#### Menampilkan semua daftar kontainer docker (yang sedang berjalan dan berhenti):
```shell
docker ps -a
```
#### Memulai sebuah kontainer dari image, dengan nama kustom:
```shell
docker run --name {{nama_kontainer}} {{image}}
```
#### Memulai atau menghentikan kontainer yang tersedia:
```shell
docker {{start|stop}} {{nama_kontainer}}
```
#### Menarik image dari registri docker:
```shell
docker pull {{image}}
```
#### Membuka shell didalam sebuah kontainer yang sedang berjalan:
```shell
docker exec -it {{nama_kontainer}} {{sh}}
```
#### Menghapus kontainer yang sedang berhenti:
```shell
docker rm {{nama_kontainer}}
```
#### Mengambil dan mengikuti semua log dari sebuah kontainer:
```shell
docker logs -f {{nama_kontainer}}
```
{% endraw %}{% raw %}
<h2 id="git-add">
  <a href="/id/common/git-add.html">git add</a> <a href="#git-add"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Menambahkan file yang diubah ke indeks.
> Informasi lebih lanjut: <https://git-scm.com/docs/git-add>.

#### Tambahkan file ke indeks:
```shell
git add {{alamat/ke/file}}
```
#### Tambahkan semua file (yang terlacak dan tidak terlacak):
```shell
git add -A
```
#### Hanya tambahkan file yang sudah terlacak:
```shell
git add -u
```
#### Tambahkan juga file yang diabaikan:
```shell
git add -f
```
#### Menambahkan file ke status stage secara interaktif:
```shell
git add -p
```
#### Menambahkan file tertentu ke status stage secara interaktif:
```shell
git add -p {{alamat/ke/file}}
```
#### Stage file secara interaktif:
```shell
git add -i
```
{% endraw %}{% raw %}
<h2 id="git-branch">
  <a href="/id/common/git-branch.html">git branch</a> <a href="#git-branch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Perintah Git utama untuk bekerja dengan cabang (*branch*).
> Informasi lebih lanjut: <https://git-scm.com/docs/git-branch>.

#### Menampilkan daftar cabang lokal. Cabang saat ini ditandai oleh `*`:
```shell
git branch
```
#### Menampilkan daftar semua cabang (lokal dan remote):
```shell
git branch -a
```
#### Tunjukkan nama cabang saat ini:
```shell
git branch --show-current
```
#### Buat cabang baru berdasarkan komit saat ini:
```shell
git branch {{nama_cabang}}
```
#### Buat cabang baru berdasarkan komit tertentu:
```shell
git branch {{nama_cabang}} {{hash_komit}}
```
#### Ganti nama cabang (harus bukan cabang saat ini untuk melakukannya):
```shell
git branch -m {{nama_cabang_lama}} {{nama_cabang_baru}}
```
#### Hapus cabang lokal (harus bukan cabang saat ini untuk melakukannya):
```shell
git branch -d {{nama_cabang}}
```
#### Hapus cabang remote:
```shell
git push {{nama_remote}} --delete {{nama_cabang_remote}}
```
{% endraw %}{% raw %}
<h2 id="git-checkout">
  <a href="/id/common/git-checkout.html">git checkout</a> <a href="#git-checkout"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Checkout cabang atau alamat ke direktori kerja.
> Informasi lebih lanjut: <https://git-scm.com/docs/git-checkout>.

#### Membuat dan beralih ke cabang baru:
```shell
git checkout -b {{nama_cabang}}
```
#### Membuat dan beralih ke cabang baru berdasarkan referensi tertentu (misal cabang, remote, cabang remote, dan tag):
```shell
git checkout -b {{nama_cabang}} {{referense}}
```
#### Beralih ke cabang lokal yang ada:
```shell
git checkout {{nama_cabang}}
```
#### Beralih ke cabang yang sebelumnya di checkout:
```shell
git checkout -
```
#### Beralih ke cabang remote yang ada:
```shell
git checkout --track {{nama_remote}}/{{nama_cabang}}
```
#### Menyingkirkan semua perubahan yang tidak masuk status stage pada direktori saat ini (lihat `git reset` untuk perintah yang lebih mirip undo):
```shell
git checkout .
```
#### Menyingkirkan perubahan yang tidak masuk status stage pada berkas:
```shell
git checkout {{nama_berkas}}
```
#### Mengganti berkas pada direktori saat ini dengan versi pada cabang lain:
```shell
git checkout {{nama_cabang}} -- {{nama_berkas}}
```
{% endraw %}{% raw %}
<h2 id="git-clone">
  <a href="/id/common/git-clone.html">git clone</a> <a href="#git-clone"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mengkloning repositori yang ada.
> Informasi lebih lanjut: <https://git-scm.com/docs/git-clone>.

#### Mengkloning repositori yang ada:
```shell
git clone {{lokasi_repositori_remote}}
```
#### Mengkloning reposiori yang ada dan submodulenya:
```shell
git clone --recursive {{lokasi_repositori_remote}}
```
#### Mengkloning repositori lokal:
```shell
git clone -l {{alamat/ke/repository/lokal}}
```
#### Mengkloning dengan senyap:
```shell
git clone -q {{lokasi_repositori_remote}}
```
#### Mengkloning repositori yang sudah ada dengan hanya mengambil 10 komit paling baru pada branch default (berguna untuk menghemat waktu):
```shell
git clone --depth {{10}} {{lokasi_repositori_remote}}
```
{% endraw %}{% raw %}
<h2 id="git-commit">
  <a href="/id/common/git-commit.html">git commit</a> <a href="#git-commit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Komit file ke dalam sebuah repositori.
> Informasi lebih lanjut: <https://git-scm.com/docs/git-commit>.

#### Komit file bertahap ke repositori dengan sebuah pesan:
```shell
git commit -m "{{pesan}}"
```
#### Otomatis merubah semua file yang dimodifikasi menjadi ke status stage dan menambahkan sebuah pesan:
```shell
git commit -a -m "{{pesan}}"
```
#### Ganti komit terakhir dengan perubahan yang ada di status stage saat ini:
```shell
git commit --amend
```
#### Komit file tertentu (yang sudah di status stage):
```shell
git commit {{alamat/ke/file/saya1}} {{alamat/ke/file/saya2}}
```
{% endraw %}{% raw %}
<h2 id="git-remote">
  <a href="/id/common/git-remote.html">git remote</a> <a href="#git-remote"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mengelola kumpulan repositori yang dilacak/diikuti ("remotes").
> Informasi lebih lanjut: <https://git-scm.com/docs/git-remote>.

#### Menampilkan daftar remote, namanya dan URL:
```shell
git remote -v
```
#### Menampilkan informasi tentang remote:
```shell
git remote show {{nama_remote}}
```
#### Menambahkan remote:
```shell
git remote add {{nama_remote}} {{url_remote}}
```
#### Mengubah URL dari remote (gunakan `--add` untuk tetap menyimpan URL lama):
```shell
git remote set-url {{nama_remote}} {{url_baru}}
```
#### Menghapus remote:
```shell
git remote remove {{nama_remote}}
```
#### Mengubah nama remote:
```shell
git remote rename {{nama_lama}} {{nama_baru}}
```
{% endraw %}{% raw %}
<h2 id="git-status">
  <a href="/id/common/git-status.html">git status</a> <a href="#git-status"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Menampilkan perubahan pada file dalam repositori Git.
> Menmapilkan daftar perubahan , menambahkan dan menghapus file dibandingkan dengan komit yang saat ini di check-out.
> Informasi lebih lanjut: <https://git-scm.com/docs/git-status>.

#### Tampilkan file yang diubah yang belum ditambahkan untuk komit:
```shell
git status
```
#### Berikan keluaran dalam format [s]hort (pendek):
```shell
git status -s
```
#### Jangan tampilkan file yang tidak terlacak di output:
```shell
git status --untracked-files=no
```
#### Tampilkan keluaran dalam format [s]hort (pendek) bersama dengan [b] info cabangnya:
```shell
git status -sb
```
{% endraw %}{% raw %}
<h2 id="git">
  <a href="/id/common/git.html">git</a> <a href="#git"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sistem kontrol versi terdistribusi.
> Informasi lebih lanjut: <https://git-scm.com/>.

#### Memeriksa versi Git:
```shell
git --version
```
#### Menunjukkan bantuan umum:
```shell
git --help
```
#### Menampilkan bantuan pada sub perintah Git (seperti `commit`,` log`, dll.):
```shell
git help {{subcommand}}
```
#### Menjalankan subperintah Git:
```shell
git {{subcommand}}
```
#### Menjalankan subperintah Git di jalur root repositori kustom:
```shell
git -C {{alamat/ke/repositori}} {{subcommand}}
```
#### Menjalankan subperintah Git dengan set konfigurasi yang diberikan:
```shell
git -c '{{config.key}}={{value}}' {{subcommand}}
```
{% endraw %}{% raw %}
<h2 id="hugo">
  <a href="/id/common/hugo.html">hugo</a> <a href="#hugo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Penghasil website statis berbasis template. Menggunakan modul, komponen dan tema.
> Informasi lebih lanjut: <https://gohugo.io>.

#### Membuat website Hugo baru:
```shell
hugo new site {{alamat/ke/website}}
```
#### Membuat tema Hugo baru (tema juga dapat diunduh dari https://themes.gohugo.io/):
```shell
hugo new theme {{nama_tema}}
```
#### Membuat halaman baru:
```shell
hugo new {{nama_bagian}}/{{nama_berkas}}
```
#### Menbuild website ke direktori `./public`:
```shell
hugo
```
#### Menbuild website termasuk halaman yang ditandai sebagai "draft":
```shell
hugo --buildDrafts
```
#### Menbuild website ke direktori yang ditentukan:
```shell
hugo --destination {{alamat/tujuan}}
```
#### Menbuild website, memulai webserver untuk menyajikannya, dan secara otomatis memuat ulang jika ada halaman yang berubah:
```shell
hugo server
```
{% endraw %}{% raw %}
<h2 id="java">
  <a href="/id/common/java.html">java</a> <a href="#java"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Peluncur Aplikasi Java.
> Informasi lebih lanjut: <https://java.com>.

#### Menjalankan berkas java `.class` yang mengandung method main dengan hanya menggunakan nama class:
```shell
java {{nama_class}}
```
#### Menjalankan program `.jar`:
```shell
java -jar {{nama_berkas.jar}}
```
#### Menjalankan program `.jar` dengan menunggu debugger terhubung ke port 5005:
```shell
java -agentlib:jdwp=transport=dt_socket,server=y,suspend=y,address=*:5005 -jar {{nama_berkas.jar}}
```
#### Menampilkan versi JDK, JRE dan HotSpot:
```shell
java -version
```
#### Menampilkan informasi penggunaan untuk perintah java:
```shell
java -help
```
{% endraw %}{% raw %}
<h2 id="laravel-zero">
  <a href="/id/common/laravel-zero.html">laravel-zero</a> <a href="#laravel-zero"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pemasang Laravel Zero framework berbasis command-line.
> Informasi lebih lanjut: <https://laravel-zero.com>.

#### Buat aplikasi Laravel Zero baru:
```shell
laravel-zero new {{nama}}
```
#### Perbarui pemasang ke versi terkini:
```shell
laravel-zero self-update
```
#### Lis perintah yang tersedia:
```shell
laravel-zero list
```
{% endraw %}{% raw %}
<h2 id="laravel">
  <a href="/id/common/laravel.html">laravel</a> <a href="#laravel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pemasang Laravel framework berbasis command-line.
> Informasi lebih lanjut: <https://laravel.com>.

#### Buat aplikasi Laravel baru:
```shell
laravel new {{nama}}
```
#### Gunakan versi pengembangan terkini:
```shell
laravel new {{nama}} --dev
```
#### Overwrite if the directory already exists:
```shell
laravel new {{nama}} --force
```
#### Pasang struktur Laravel Jetstream:
```shell
laravel new {{nama}} --jet
```
#### Pasang struktur Laravel Jetstream dengan susunan tertentu:
```shell
laravel new {{nama}} --jet --stack {{livewire|inertia}}
```
#### Pasang struktur Laravel Jetstream dengan dukungan tim:
```shell
laravel new {{nama}} --jet --teams
```
#### Lis perintah yang tersedia:
```shell
laravel list
```
{% endraw %}{% raw %}
<h2 id="ls">
  <a href="/id/common/ls.html">ls</a> <a href="#ls"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Menampilkan daftar konten pada direktori.
> Informasi lebih lanjut: <https://www.gnu.org/software/coreutils/ls>.

#### Menampilkan daftar berkas dengan satu item tiap baris:
```shell
ls -1
```
#### Menampilkan daftar semua berkas, termasuk berkas tersembunyi:
```shell
ls -a
```
#### Menampilkan daftar semua berkas, dengan akhiran `/` ditambahkan ke nama direktori:
```shell
ls -F
```
#### Menampilkan daftar berformat panjang (menampilkan izin, kepemilikan, ukuran dan waktu modifikasi pada setiap berkas):
```shell
ls -la
```
#### Menampilkan daftar berformat panjang dan ukuran ditampilkan menggunakan unit yang mudah dibaca manusia (KiB, MiB, GiB):
```shell
ls -lh
```
#### Menampilkan daftar berformat panjang dan diurutkan berdasarkan ukuran (menurun):
```shell
ls -lS
```
#### Menampilkan daftar berformat panjang dari semua berkas dan diurutkan berdasarkan tanggal modifikasi (terlama dulu):
```shell
ls -ltr
```
{% endraw %}{% raw %}
<h2 id="mkdir">
  <a href="/id/common/mkdir.html">mkdir</a> <a href="#mkdir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Membuat sebuah direktori.
> Informasi lebih lanjut: <https://www.gnu.org/software/coreutils/mkdir>.

#### Membuat sebuah direktori di dalam direktori saat ini atau dalam jalan (path) yang diberikan:
```shell
mkdir {{direktori}}
```
#### Membuat sejumlah direktori secara rekursif (berguna untuk membuat direktori bersarang):
```shell
mkdir -p {{jalan/menuju/direktori}}
```
{% endraw %}{% raw %}
<h2 id="mongod">
  <a href="/id/common/mongod.html">mongod</a> <a href="#mongod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Server database MongoDB.
> Informasi lebih lanjut: <https://docs.mongodb.com/manual/reference/program/mongod>.

#### Menentukan berkas konfigurasi:
```shell
mongod --config {{nama_berkas}}
```
#### Menentukan port yang digunakan:
```shell
mongod --port {{port}}
```
#### Menentukan tingkat pencatatan perilaku (*profiling*) database. 0 mati, 1 hanya operasi lambat, 2 semuanya:
```shell
mongod --profile {{0|1|2}}
```
{% endraw %}{% raw %}
<h2 id="mv">
  <a href="/id/common/mv.html">mv</a> <a href="#mv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Memindah atau menamai-ulang file dan direktori.
> Informasi lebih lanjut: <https://www.gnu.org/software/coreutils/mv>.

#### Memindahkan file ke lokasi yang baru:
```shell
mv {{sumber}} {{tujuan}}
```
#### Memindah tanpa meminta konfirmasi sebelum menimpa file yang sudah ada:
```shell
mv -f {{sumber}} {{tujuan}}
```
#### Meminta konfirmasi sebelum menimpa file yang sudah ada, apapun *file permissions*-nya:
```shell
mv -i {{sumber}} {{tujuan}}
```
#### Jangan menimpa file yang sudah ada di direktori tujuan:
```shell
mv -n {{sumber}} {{tujuan}}
```
#### Memindahkan file dalam mode *verbose*, menampilkan file-file yang dipindahkan:
```shell
mv -v {{sumber}} {{tujuan}}
```
{% endraw %}{% raw %}
<h2 id="node">
  <a href="/id/common/node.html">node</a> <a href="#node"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Platform JavaScript sisi server (Node.js).
> Informasi lebih lanjut: <https://nodejs.org>.

#### Menjalankan berkas JavaScript:
```shell
node {{alamat/ke/berkas}}
```
#### Memulai sebuah REPL (shell interaktif):
```shell
node
```
#### Mengevaluasi kode JavaScript dengan memberikanya sebagai sebuah argument:
```shell
node -e "{{kode}}"
```
#### Mengevaluasi dan mencetak hasil, berguna untuk melihat versi dependesni node:
```shell
node -p "{{process.versions}}"
```
#### Mengaktifkan inspector, menjeda eksekusi sampai debugger terhubung segera setelah kode sumber sepenuhnya terparser:
```shell
node --no-lazy --inspect-brk {{alamat/ke/berkas}}
```
{% endraw %}{% raw %}
<h2 id="npm">
  <a href="/id/common/npm.html">npm</a> <a href="#npm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manajer paket JavaScript dan Node.js.
> Mengelola proyek Node.js dan dependensi modulnya.
> Informasi lebih lanjut: <https://www.npmjs.com/>.

#### Membuat file `package.json` secara interaktif:
```shell
npm init
```
#### Unduh semua paket yang terdaftar sebagai dependensi di package.json:
```shell
npm install
```
#### Unduh versi tertentu dari sebuah paket dan menambahkan ke daftar dependensi di `package.json`:
```shell
npm install {{nama_modul}}@{{versi}}
```
#### Unduh paket dan menambahkan ke daftar dependensi dev di package.json:
```shell
npm install {{nama_modul}} --save-dev
```
#### Unduh paket dan instal secara global:
```shell
npm install --global {{nama_modul}}
```
#### Copot pemasangan paket dan hapus dari daftar dependensi di `package.json`:
```shell
npm uninstall {{nama_modul}}
```
#### Mencetak pohon dependensi yang diinstal secara lokal:
```shell
npm list
```
#### Buat daftar modul tingkat atas yang diinstal secara global:
```shell
npm list --global --depth={{0}}
```
{% endraw %}{% raw %}
<h2 id="nvim">
  <a href="/id/common/nvim.html">nvim</a> <a href="#nvim"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Neovim, teks editor programmer berbasis Vim, menyediakan beberapa mode untuk manipulasi teks berbeda jenis.
> Tekan `i` masuk mode edit. `<Esc>` kembali ke mode normal, yang tidak mengizinkan penyisipan teks biasa.
> Informasi lebih lanjut: <https://neovim.io>.

#### Membuka berkas:
```shell
nvim {{berkas}}
```
#### Masuk ke mode pengeditan teks (insert mode):
```shell
<Esc>i
```
#### Menyalin ("yank") atau memotong ("delete") baris saat ini (tempel itu dengan `P`):
```shell
<Esc>{{yy|dd}}
```
#### Batalkan operasi terakhir:
```shell
<Esc>u
```
#### Mencari sebuah pattern pada berkas (tekan `n`/`N` untuk pergi ke kecocokan berikutnya/sebelumnya):
```shell
<Esc>/{{pattern_pencarian}}<Enter>
```
#### Melakukan penggantian ekspresi reguler pada seluruh berkas:
```shell
<Esc>:%s/{{ekspresi_reguler}}/{{pengganti}}/g<Enter>
```
#### Menyimpan (write) berkas, dan keluar:
```shell
<Esc>:wq<Enter>
```
#### Keluar tanpa menyimpan:
```shell
<Esc>:q!<Enter>
```
{% endraw %}{% raw %}
<h2 id="nvm">
  <a href="/id/common/nvm.html">nvm</a> <a href="#nvm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Memasang, melepas, atau mengganti versi Node.js yang dipakai.
> Mendukung nomor versi seperti "0.12" or "v4.2", dan label versi seperti "stable", "system", dsb.
> Informasi lebih lanjut: <https://github.com/creationix/nvm>.

#### Memasang versi Node.js yang ditentukan:
```shell
nvm install {{versi_node_js}}
```
#### Menggunakan versi Node.js tertentu untuk sesi saat ini:
```shell
nvm use {{versi_node_js}}
```
#### Menyetel versi Node.js secara default:
```shell
nvm alias default {{versi_node_js}}
```
#### Menunjukkan daftar versi Node.js yang tersedia dan versi Node.js yang disetel sebagai default:
```shell
nvm list
```
#### Menghapus sebuah versi Node.js yang terpasang melalui `nvm`:
```shell
nvm uninstall {{versi_node_js}}
```
#### Menjalankan interpreter (REPL) Node.js dengan versi tertentu:
```shell
nvm run {{versi_node_js}} --version
```
#### Menjalankan sebuah file atau aplikasi JavaScript di dalam Node.js versi tertentu:
```shell
nvm exec {{versi_node_js}} node {{app.js}}
```
{% endraw %}{% raw %}
<h2 id="pip">
  <a href="/id/common/pip.html">pip</a> <a href="#pip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pengelola paket Python.
> Informasi lebih lanjut: <https://pip.pypa.io>.

#### Memasang paket:
```shell
pip install {{nama_paket}}
```
#### Memasang versi paket tertentu:
```shell
pip install {{nama_paket}}=={{versi_paket}}
```
#### Meningkatakan paket ke versi terbaru:
```shell
pip install -U {{nama_paket}}
```
#### Mencopot pemasangan paket:
```shell
pip uninstall {{nama_paket}}
```
#### Menyimpan daftar paket terpasang ke berkas:
```shell
pip freeze > {{requirements.txt}}
```
#### Memasang paket dari berkas:
```shell
pip install -r {{requirements.txt}}
```
#### Menampilkan informasi paket terpasang:
```shell
pip show {{nama_paket}}
```
{% endraw %}{% raw %}
<h2 id="pip3">
  <a href="/id/common/pip3.html">pip3</a> <a href="#pip3"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pengelola paket Python.
> Informasi lebih lanjut: <https://pip.pypa.io>.

#### Menemukan paket tersedia:
```shell
pip3 search {{nama_paket}}
```
#### Memasang paket:
```shell
pip3 install {{nama_paket}}
```
#### Memasang versi paket tertentu:
```shell
pip3 install {{nama_paket}}=={{versi_paket}}
```
#### Meningkatkan paket ke versi terbaru:
```shell
pip3 install --upgrade {{nama_paket}}
```
#### Mencopot pemasangan paket:
```shell
pip3 uninstall {{nama_paket}}
```
#### Menyimpan daftar paket terpasang ke berkas:
```shell
pip3 freeze > {{requirements.txt}}
```
#### Memasang paket dari berkas:
```shell
pip3 install --requirement {{requirements.txt}}
```
#### Menampilkan informasi paket terinstal:
```shell
pip3 show {{nama_paket}}
```
{% endraw %}{% raw %}
<h2 id="pwd">
  <a href="/id/common/pwd.html">pwd</a> <a href="#pwd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mencetak nama dari direktori saat ini/kerja.
> Informasi lebih lanjut: <https://www.gnu.org/software/coreutils/pwd>.

#### Mencetak direktori saat ini:
```shell
pwd
```
#### Mencetak direktori saat ini, dan menjelaskan semua tautan simbolis (dengan kata lain menampilkan alamat fisik):
```shell
pwd -P
```
{% endraw %}{% raw %}
<h2 id="python">
  <a href="/id/common/python.html">python</a> <a href="#python"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Penerjemah bahasa Python.
> Informasi lebih lanjut: <https://www.python.org>.

#### Menjalankan REPL (shell interaktif):
```shell
python
```
#### Menjalankan skrip pada berkas Python:
```shell
python {{skrip.py}}
```
#### Menjalankan skrip sebagai bagian dari shell interaktif:
```shell
python -i {{skrip.py}}
```
#### Menjalankan ekspresi Python:
```shell
python -c "{{ekspresi}}"
```
#### Menjalankan modul perpustakaan sebagai skrip (diakhiri dengan daftar opsi):
```shell
python -m {{modul}} {{argumen}}
```
#### Mendebug skrip Python secara interaktif:
```shell
python -m pdb {{script.py}}
```
{% endraw %}{% raw %}
<h2 id="rm">
  <a href="/id/common/rm.html">rm</a> <a href="#rm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Menghapus berkas atau direktori.
> Informasi lebih lanjut: <https://www.gnu.org/software/coreutils/rm>.

#### Menghapus berkas dari lokasi manapun:
```shell
rm {{alamat/ke/berkas}} {{alamat/ke/berkas/lainnya}}
```
#### Menghapus direktori dan semua subdirektorinya secara rekursif:
```shell
rm -r {{alamat/ke/direktori}}
```
#### Menghapus direktori secara paksa, tanpa meminta konfirmasi atau menampilkan pesan kesalahan:
```shell
rm -rf {{alamat/ke/direktori}}
```
#### Menghapus banyak berkas secara interaktif, dengan meminta konfirmasi sebelum setiap penghapusan:
```shell
rm -i {{(beberapa)_berkas}}
```
#### Menghapus berkas dengan mode verbose, mencetak pesan untuk setiap berkas yang terhapus:
```shell
rm -v {{alamat/ke/directori/*}}
```
{% endraw %}{% raw %}
<h2 id="scrcpy">
  <a href="/id/common/scrcpy.html">scrcpy</a> <a href="#scrcpy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tampilkan layar and kontrol perangkat Android anda di dalam desktop.
> Informasi lebih lanjut: <https://github.com/Genymobile/scrcpy>.

#### Tampilkan layar sebuah perangkat yang terhubung:
```shell
scrcpy
```
#### Tampilkan layar perangkat tertentu berdasarkan ID atau alamat IP-nya (temukan menggunakan perintah `adb devices`):
```shell
scrcpy --serial {{0123456789abcdef|192.168.0.1:5555}}
```
#### Tampilkan layar dalam mode layar penuh / fullscreen:
```shell
scrcpy --fullscreen
```
#### Putarkan tampilan layar perangkat dalam kelipatan 90 derajat (berlawanan arah jarum jam):
```shell
scrcpy --rotation {{0|1|2|3}}
```
#### Tunjukkan indikator sentuhan pada perangkat fisik:
```shell
scrcpy --show-touches
```
#### Rekam tampilan layar perangkat ke dalam file video tertentu:
```shell
scrcpy --record {{jalan/menuju/file.mp4}}
```
#### Tentukan direktori yang akan digunakan untuk memindahkan file (non-APK) ke dalam perangkat melalui drag-and-drop:
```shell
scrcpy --push-target {{jalan/menuju/direktori}}
```
{% endraw %}{% raw %}
<h2 id="touch">
  <a href="/id/common/touch.html">touch</a> <a href="#touch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mengubah waktu akses (atime) dan waktu modifikasi (mtime) dari sebuah file.
> Informasi lebih lanjut: <https://www.gnu.org/software/coreutils/touch>.

#### Membuat file baru yang kosong atau mengubah waktu file yang telahj ada ke waktu sekarang:
```shell
touch {{nama_file}}
```
#### Mengatur waktu sebuah file ke tanggal dan jam tertentu:
```shell
touch -t {{YYYYMMDDHHMM.SS}} {{nama_file}}
```
#### Menggunakan waktu dari satu file untuk mengatur waktu file yang lain:
```shell
touch -r {{nama_file}} {{nama_file2}}
```
{% endraw %}{% raw %}
<h2 id="vue-build">
  <a href="/id/common/vue-build.html">vue build</a> <a href="#vue-build"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sub-perintah yang disediakan oleh `@vue/cli` dan `@vue/cli-service-global` yang memungkinkan prototipe cepat.
> Informasi lebih lanjut: <https://cli.vuejs.org/guide/prototyping.html>.

#### Membangun berkas `.js` or `.vue` pada mode produksi tanpa konfigurasi:
```shell
vue build {{nama_file}}
```
{% endraw %}{% raw %}
<h2 id="vue-init">
  <a href="/id/common/vue-init.html">vue init</a> <a href="#vue-init"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sub-perintah untuk menginisialisasi proyek warisan framework Vue.js.
> Informasi lebih lanjut: <https://cli.vuejs.org/guide/creating-a-project.html#pulling-2-x-templates-legacy>.

#### Buat proyek baru dengan menggunakan salah satu templat bawaan:
```shell
vue init {{webpack|webpack-simple|browserify|browserify-simple|simple}} {{nama_proyek}}
```
#### Buat proyek baru menggunakan templat lokal:
```shell
vue init {{lokasi/ke/templat_direktori}} {{nama_proyek}}
```
#### Buat proyek baru dengan menggunakan templat dari GitHub:
```shell
vue init {{username}}/{{repo}} {{nama_proyek}}
```
{% endraw %}{% raw %}
<h2 id="vue-serve">
  <a href="/id/common/vue-serve.html">vue serve</a> <a href="#vue-serve"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Sub-perintah yang disediakan oleh `@vue/cli` dan `@vue/cli-service-global` yang memungkinkan prototipe cepat.
> Informasi lebih lanjut: <https://cli.vuejs.org/guide/prototyping.html>.

#### Sajikan berkas `.js` or `.vue` pada mode pengembangan tanpa konfigurasi:
```shell
vue serve {{nama_file}}
```
{% endraw %}{% raw %}
<h2 id="vue">
  <a href="/id/common/vue.html">vue</a> <a href="#vue"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI serba guna untuk Vue.js.
> Informasi lebih lanjut: <https://cli.vuejs.org>.

#### Buat proyek vue baru secara interaktif:
```shell
vue create {{nama_proyek}}
```
#### Buat proyek baru dengan antar muka web:
```shell
vue ui
```
{% endraw %}{% raw %}
<h2 id="yarn">
  <a href="/id/common/yarn.html">yarn</a> <a href="#yarn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Pengelola paket alternatif untuk JavaScript dan Node.js.
> Informasi lebih lanjut: <https://yarnpkg.com>.

#### Memasang modul secara global:
```shell
yarn global add {{nama_modul}}
```
#### Memasang semua dependensi yang dirujuk di berkas `package.json` (`install` adalah opsional):
```shell
yarn install
```
#### Memasang modul dan menyimpannya sebagai dependensi ke berkas `package.json` (tambahkan `--dev` untuk menyimpannya sebagai dependensi pengembangan):
```shell
yarn add {{nama_modul}}@{{versi}}
```
#### Mencopot modul dan menghapusnya dari berkas `package.json`:
```shell
yarn remove {{nama_modul}}
```
#### Membuat berkas `package.json` secara interaktif:
```shell
yarn init
```
#### Mengidentifikasi apakah modul merupakan dependensi dan daftar modul lainnya yang bergantung padanya:
```shell
yarn why {{module_name}}
```
{% endraw %}