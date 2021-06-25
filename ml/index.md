---
layout: default
title: "ML"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#linux">Linux</a>
  * <a href="#apt">apt</a>
  * <a href="#cal">cal</a>
  * <a href="#lsmod">lsmod</a>
  * <a href="#nmcli">nmcli</a>
  * <a href="#pacman">pacman</a>


# Linux
{% raw %}
<h2 id="apt">
  <a href="/ml/linux/apt.html">apt</a> <a href="#apt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ഡെബിയൻ അടിസ്ഥാനമാക്കിയുള്ള വിതരണങ്ങൾക്കായുള്ള പാക്കേജ് മാനേജുമെന്റ് യൂട്ടിലിറ്റി.
> ഉബുണ്ടു പതിപ്പുകളിൽ 16.04ലും അതിനുശേഷമുള്ളതിലും സംവേദനാത്മകമായി ഉപയോഗിക്കുമ്പോൾ apt-get പകരം വയ്ക്കാൻ ശുപാർശ ചെയ്യുന്നതു.
> കൂടുതൽ വിവരങ്ങൾ: <https://manpages.debian.org/latest/apt/apt.8.html>.

#### ലഭ്യമായ പാക്കേജുകളുടെയും പതിപ്പുകളുടെയും പട്ടിക അപ്‌ഡേറ്റുചെയ്യുക (മറ്റ് `apt` കമാൻഡുകൾക്ക് മുമ്പ് ഇത് പ്രവർത്തിപ്പിക്കാൻ ശുപാർശ ചെയ്യുന്നു):
```shell
sudo apt update
```
#### പാക്കേജിനായി തിരയുക:
```shell
apt search {{പാക്കേജ്}}
```
#### ഒരു പാക്കേജിന്റെ വിവരങ്ങൾ കാണിക്കുക:
```shell
apt show {{പാക്കേജ്}}
```
#### ഒരു പാക്കേജ് ഇൻസ്റ്റാൾ ചെയ്യുക, അല്ലെങ്കിൽ ലഭ്യമായ ഏറ്റവും പുതിയ പതിപ്പിലേക്ക് അപ്‌ഡേറ്റ് ചെയ്യുക:
```shell
sudo apt install {{പാക്കേജ്}}
```
#### ഒരു പാക്കേജ് നീക്കംചെയ്യുക (പകരം `purge` ഉപയോഗിക്കുന്നത് അതിന്റെ കോൺഫിഗറേഷൻ ഫയലുകളും നീക്കംചെയ്യുന്നു):
```shell
sudo apt remove {{പാക്കേജ്}}
```
#### ഇൻസ്റ്റാളുചെയ്‌ത എല്ലാ പാക്കേജുകളും ലഭ്യമായ ഏറ്റവും പുതിയ പതിപ്പുകളിലേക്ക് അപ്‌ഗ്രേഡുചെയ്യുക:
```shell
sudo apt upgrade
```
#### എല്ലാ പാക്കേജുകളും കാണിക്കുക:
```shell
apt list
```
#### ഇൻസ്റ്റാൾ ചെയ്ത പാക്കേജുകൾ കാണിക്കുക:
```shell
apt list --installed
```
{% endraw %}{% raw %}
<h2 id="cal">
  <a href="/ml/linux/cal.html">cal</a> <a href="#cal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ഇന്നത്തെ ദിവസം അടയാളപ്പെടുത്തിയുള്ള കലണ്ടർ വിവരം കാണിക്കുക .

#### ഇപ്പോഴത്തെ മാസത്തിന്റെ കലണ്ടർ കാണാൻ :
```shell
cal
```
#### കഴിഞ്ഞ മാസവും, ഇപ്പോഴത്തെ മാസവും അടുത്ത മാസവും കാണാൻ :
```shell
cal -3
```
#### ആഴ്ചയുടെ ഒന്നാമത്തെ ദിവസം തിങ്കളാഴ്ച ആയി കാണാൻ :
```shell
cal --monday
```
#### ഒരു പ്രത്യേക കൊല്ലത്തിന്റെ കലണ്ടർ കാണാൻ ( 4 അക്കങ്ങൾ ) :
```shell
cal {{കൊല്ലം}}
```
#### ഒരു പ്രതേക മാസത്തിന്റെയും കൊല്ലത്തിന്റെയും കലണ്ടർ കാണാൻ :
```shell
cal {{മാസം}} {{കൊല്ലം}}
```
{% endraw %}{% raw %}
<h2 id="lsmod">
  <a href="/ml/linux/lsmod.html">lsmod</a> <a href="#lsmod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ലിനക്സ് കെർണൽ മൊഡ്യൂളുകളുടെ അവസ്ഥ കാണാൻ.
> ലിനക്സ് കെർണൽ മൊഡ്യൂൾ ലോഡ് ചെയ്യാൻ `modprobe` കാണുക.

#### ഇപ്പോൾ ലോഡ് ചെയ്ത മൊഡ്യൂളുകൾ കാണിക്കുക:
```shell
lsmod
```
{% endraw %}{% raw %}
<h2 id="nmcli">
  <a href="/ml/linux/nmcli.html">nmcli</a> <a href="#nmcli"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> നെറ്റ്‌വർക്ക് മാനേജർ നിയന്ത്രിക്കാൻ വേണ്ടിയുള്ള കമാൻഡ് ലൈൻ ഉപകരണം.
> കൂടുതൽ വിവരങ്ങൾ: <https://man.archlinux.org/man/nmcli.1>.

#### nmcli പതിപ്പ് ഏതാണെന്ന് അറിയാൻ :
```shell
nmcli --version
```
#### പൊതുവെയുള്ള സഹായ വിവരം കാണാൻ :
```shell
nmcli --help
```
#### ഒരു പ്രതേക നിർദേശത്തിന്റെ സഹായ വിവരം കാണാൻ :
```shell
nmcli {{നിർദേശം}} --help
```
#### ഒരു `nmcli` നിർദേശം നിർവഹിക്കാൻ :
```shell
nmcli {{നിർദേശം}}
```
{% endraw %}{% raw %}
<h2 id="pacman">
  <a href="/ml/linux/pacman.html">pacman</a> <a href="#pacman"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ആർച്ച് ലിന്ക്സിന്റെ പാക്കേജ് മാനേജുമെന്റ് യൂട്ടിലിറ്റി.
> കൂടുതൽ വിവരങ്ങൾ: <https://man.archlinux.org/man/pacman.8>.

#### ഇൻസ്റ്റാൾ ചെയ്‌ത എല്ലാ പാക്കേജും അപ്‌ഡേറ്റു ചെയ്യുക:
```shell
pacman -Syu
```
#### പുതിയ പാക്കേജ് ഇൻസ്റ്റാൾ ചെയ്യുക:
```shell
pacman -S {{പാക്കേജ്}}
```
#### ഒരു പാക്കേജും അത് ആശ്രയിക്കുന്ന മറ്റ് പാക്കേജുകളെയും കളയുക :
```shell
pacman -Rs {{പാക്കേജ്}}
```
#### പാക്കേജ് ഡാറ്റാബേസിൽ ഒരു സൂചകപദം അല്ലെങ്കിൽ റെഗുലർ എക്സ്പ്രെഷൻ വെച്ച് തിരയുക :
```shell
pacman -Ss "{{സെർച്ച് പാറ്റേൺ}}"
```
#### ഇൻസ്റ്റാൾ ചെയ്‌ത എല്ലാ പാക്കേജുകളും അതിന്റെ പതിപ്പും കാണിക്കുക:
```shell
pacman -Q
```
#### നേരെ ഇൻസ്റ്റാൾ ചെയ്ത പാക്കേജ്‌സ് മാത്റം കാണിക്കുക:
```shell
pacman -Qe
```
#### ഏത് പാക്കേജാണ് ഒരു ഫയലിന്റെ ഉടമ എന്ന് കണ്ടുപിടിക്കാൻ:
```shell
pacman -Qo {{ഫയലിന്റെ പേര്}}
```
#### പാക്കേജ് ക്യാഷ് കാലിയാക്കി സ്റ്റോറേജ്‌ മുക്തമാക്കുക:
```shell
pacman -Scc
```
{% endraw %}