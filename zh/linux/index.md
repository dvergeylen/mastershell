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
* <a href="#ac">ac</a>
* <a href="#acpi">acpi</a>
* <a href="#add-apt-repository">add-apt-repository</a>
* <a href="#addpart">addpart</a>
* <a href="#addr2line">addr2line</a>
* <a href="#adduser">adduser</a>
* <a href="#alpine">alpine</a>
* <a href="#amixer">amixer</a>
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
* <a href="#arch">arch</a>
* <a href="#archey">archey</a>
* <a href="#archlinux-java">archlinux-java</a>
* <a href="#arecored">arecored</a>
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
* <a href="#authconfig">authconfig</a>
* <a href="#autorandr">autorandr</a>
* <a href="#avahi-browse">avahi-browse</a>
* <a href="#boltctl">boltctl</a>
* <a href="#btrfs">btrfs</a>
* <a href="#btrfs-device">btrfs device</a>
* <a href="#btrfs-filesystem">btrfs filesystem</a>
* <a href="#btrfs-scrub">btrfs scrub</a>
* <a href="#btrfs-subvolume">btrfs subvolume</a>
* <a href="#cpuid">cpuid</a>
* <a href="#debootstrap">debootstrap</a>
* <a href="#debuild">debuild</a>
* <a href="#dmenu">dmenu</a>
* <a href="#dmesg">dmesg</a>
* <a href="#dos2unix">dos2unix</a>
* <a href="#fc-cache">fc-cache</a>
* <a href="#fc-list">fc-list</a>
* <a href="#flameshot">flameshot</a>
* <a href="#flatpak">flatpak</a>
* <a href="#i3">i3</a>
* <a href="#iptables">iptables</a>
* <a href="#konsole">konsole</a>
* <a href="#logsave">logsave</a>
* <a href="#mac2unix">mac2unix</a>
* <a href="#pacman">pacman</a>
* <a href="#poweroff">poweroff</a>
* <a href="#reboot">reboot</a>
* <a href="#unix2dos">unix2dos</a>
* <a href="#unix2mac">unix2mac</a>
* <a href="#yaourt">yaourt</a>
* <a href="#yay">yay</a>
* <a href="#zypper">zypper</a>

{% raw %}
<h2 id="a2disconf">
  <a href="/zh/linux/a2disconf.html">a2disconf</a> <a href="#a2disconf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在基于 Debian 的操作系统上禁用 Apache 配置文件.
> 更多信息: <https://manpages.debian.org/latest/apache2/a2disconf.8.html>.

#### 禁用配置文件:
```shell
sudo a2disconf {{配置文件}}
```
#### 不显示信息性消息:
```shell
sudo a2disconf --quiet {{配置文件}}
```
{% endraw %}{% raw %}
<h2 id="a2dismod">
  <a href="/zh/linux/a2dismod.html">a2dismod</a> <a href="#a2dismod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在基于 Debian 的操作系统上禁用 Apache 模块。
> 更多信息：<https://manpages.debian.org/latest/apache2/a2dismod.8.html>.

#### 禁用模块：
```shell
sudo a2dismod {{模块路径}}
```
#### 不显示信息性消息：
```shell
sudo a2dismod --quiet {{模块路径}}
```
{% endraw %}{% raw %}
<h2 id="a2dissite">
  <a href="/zh/linux/a2dissite.html">a2dissite</a> <a href="#a2dissite"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在基于 Debian 的操作系统上禁用 Apache 虚拟主机。
> 更多信息：<https://manpages.debian.org/latest/apache2/a2dissite.8.html>.

#### 禁用虚拟主机：
```shell
sudo a2dissite {{虚拟主机名}}
```
#### 不显示信息性消息：
```shell
sudo a2dissite --quiet {{虚拟主机名}}
```
{% endraw %}{% raw %}
<h2 id="a2enconf">
  <a href="/zh/linux/a2enconf.html">a2enconf</a> <a href="#a2enconf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在基于 Debian 的操作系统上启用 Apache 配置文件。
> 更多信息：<https://manpages.debian.org/latest/apache2/a2enconf.8.html>.

#### 启用配置文件：
```shell
sudo a2enconf {{配置文件}}
```
#### 不显示信息性消息：
```shell
sudo a2enconf --quiet {{配置文件}}
```
{% endraw %}{% raw %}
<h2 id="a2enmod">
  <a href="/zh/linux/a2enmod.html">a2enmod</a> <a href="#a2enmod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在基于 Debian 的操作系统上启用 Apache 模块。
> 更多信息：<https://manpages.debian.org/latest/apache2/a2enmod.8.html>.

#### 启用模块：
```shell
sudo a2enmod {{模块名}}
```
#### 不显示信息性消息：
```shell
sudo a2enmod --quiet {{模块名}}
```
{% endraw %}{% raw %}
<h2 id="a2ensite">
  <a href="/zh/linux/a2ensite.html">a2ensite</a> <a href="#a2ensite"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在基于 Debian 的操作系统上启用 Apache 虚拟主机。
> 更多信息：<https://manpages.debian.org/latest/apache2/a2ensite.8.html>.

#### 启用虚拟主机：
```shell
sudo a2ensite {{虚拟主机名}}
```
#### 不显示信息性消息：
```shell
sudo a2ensite --quiet {{虚拟主机名}}
```
{% endraw %}{% raw %}
<h2 id="a2query">
  <a href="/zh/linux/a2query.html">a2query</a> <a href="#a2query"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在基于 Debian 的操作系统上查看 Apache 运行配置。
> 更多信息：<https://manpages.debian.org/latest/apache2/a2query.1.html>.

#### 列出启用的 Apache 模块：
```shell
sudo a2query -m
```
#### 查看某个模块是否已安装：
```shell
sudo a2query -m {{模块名}}
```
#### 列出已启用的虚拟主机：
```shell
sudo a2query -s
```
#### 显示已启用的多进程模块：
```shell
sudo a2query -M
```
#### 显示 Apache 版本：
```shell
sudo a2query -v
```
{% endraw %}{% raw %}
<h2 id="ac">
  <a href="/zh/linux/ac.html">ac</a> <a href="#ac"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 打印用户连接时长数据。

#### 以小时为单位打印当前用户连接时间：
```shell
ac
```
#### 以小时为单位打印所有用户连接时间：
```shell
ac --individual-totals
```
#### 以小时为单位打印特定用户连接时间：
```shell
ac --individual-totals {{用户名}}
```
#### 以小时为单位打印特定用户每天连接时间：
```shell
ac --daily-totals --individual-totals {{用户名}}
```
#### 显示附加明细：
```shell
ac --compatibility
```
{% endraw %}{% raw %}
<h2 id="acpi">
  <a href="/zh/linux/acpi.html">acpi</a> <a href="#acpi"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示电池状态或热量信息。
> 更多信息：<https://sourceforge.net/projects/acpiclient/files/acpiclient/>.

#### 显示电池信息：
```shell
acpi
```
#### 显示热量（温度）信息：
```shell
acpi -t
```
#### 显示冷却设备信息：
```shell
acpi -c
```
#### 用华氏度单位显示热量（温度）信息：
```shell
acpi -tf
```
#### 显示所有信息：
```shell
acpi -V
```
#### 从 `/proc` 而非 `/sys` 中提取信息：
```shell
acpi -p
```
{% endraw %}{% raw %}
<h2 id="add-apt-repository">
  <a href="/zh/linux/add-apt-repository.html">add-apt-repository</a> <a href="#add-apt-repository"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> apt 仓库管理。

#### 添加一个新的 apt 仓库：
```shell
add-apt-repository {{指定仓库}}
```
#### 移除一个 apt 仓库：
```shell
add-apt-repository --remove {{指定仓库}}
```
#### 添加一个仓库并更新缓存：
```shell
add-apt-repository --update {{指定仓库}}
```
#### 允许从指定仓库下载源码：
```shell
add-apt-repository --enable-source {{指定仓库}}
```
{% endraw %}{% raw %}
<h2 id="addpart">
  <a href="/zh/linux/addpart.html">addpart</a> <a href="#addpart"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将特定分区的存在告知 Linux 内核。
> 这个命令是 `add partition` ioctl 的简单封装。
> 更多信息：<https://manned.org/addpart>.

#### 将特定分区的存在告知 Linux 内核：
```shell
addpart {{设备名}} {{分区名}} {{起始点}} {{长度}}
```
{% endraw %}{% raw %}
<h2 id="addr2line">
  <a href="/zh/linux/addr2line.html">addr2line</a> <a href="#addr2line"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将二进制文件地址转换成文件名和行数。

#### 显示可执行文件的指令地址对应源代码的文件名和行数：
```shell
addr2line --exe={{可执行文件路径}} {{地址}}
```
#### 显示函数名、文件名和行数：
```shell
addr2line --exe={{可执行文件路径}} --functions {{地址}}
```
#### 将 c++ 代码函数名符号重组：
```shell
addr2line --exe={{可执行文件地址}} --functions --demangle {{地址}}
```
{% endraw %}{% raw %}
<h2 id="adduser">
  <a href="/zh/linux/adduser.html">adduser</a> <a href="#adduser"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 添加用户的工具.
> 更多信息： <https://manpages.debian.org/latest/adduser/adduser.html>.

#### 创建一个新用户，在默认路径创建 home 目录，并提示用户设置密码:
```shell
adduser {{用户名}}
```
#### 创建一个新用户，不生成 home 目录:
```shell
adduser --no-create-home {{用户名}}
```
#### 创建一个新用户，并在指定路径下创建 home 目录:
```shell
adduser --home {{home 路径}} {{用户名}}
```
#### 创建一个新用户，并指定登录 shell:
```shell
adduser --shell {{shell 路径}} {{用户名}}
```
#### 创建一个新用户，并指定其用户组:
```shell
adduser --ingroup {{用户组}} {{用户名}}
```
{% endraw %}{% raw %}
<h2 id="alpine">
  <a href="/zh/linux/alpine.html">alpine</a> <a href="#alpine"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一个电子邮件客户端和 usenet 新闻组程序，具有 pico/nano 风格的界面
> 通过 IMAP 支持大多数现代电子邮件服务

#### 正常打开 alpine:
```shell
alpine
```
#### 直接打开写信息界面，并指定电子邮件发送地址:
```shell
alpine {{邮箱地址}}
```
#### 退出 alpine:
```shell
'q' 然后 'y'
```
{% endraw %}{% raw %}
<h2 id="amixer">
  <a href="/zh/linux/amixer.html">amixer</a> <a href="#amixer"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ALSA 声卡驱动程序的混合器。

#### 增加 10% 的主音量：
```shell
amixer -D pulse sset Master {{10%+}}
```
#### 降低 10% 的主音量：
```shell
amixer -D pulse sset Master {{10%-}}
```
{% endraw %}{% raw %}
<h2 id="apache2ctl">
  <a href="/zh/linux/apache2ctl.html">apache2ctl</a> <a href="#apache2ctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Apache HTTP web 服务器命令行管理工具。
> 基于 Debian 的操作系统自带该命令，基于 RHEL 的查看 `httpd`。

#### 启动 Apache 守护进程。如果已运行则发送一个消息：
```shell
sudo apache2ctl start
```
#### 关闭 Apache 守护进程：
```shell
sudo apache2ctl stop
```
#### 重启 Apache 守护进程：
```shell
sudo apache2ctl restart
```
#### 检查配置文件语法：
```shell
sudo apache2ctl -t
```
#### 列出已加载模块：
```shell
sudo apache2ctl -M
```
{% endraw %}{% raw %}
<h2 id="apk">
  <a href="/zh/linux/apk.html">apk</a> <a href="#apk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Alpine Linux 的包管理工具.

#### 从所有的远程仓库中更新仓库索引:
```shell
apk update
```
#### 安装一个新软件包:
```shell
apk add {{软件包}}
```
#### 移除一个软件包:
```shell
apk del {{软件包}}
```
#### 修复或更新软件包而不修改主依赖项:
```shell
apk fix {{软件包}}
```
#### 通过关键字查找软件包:
```shell
apk search {{关键字}}
```
#### 获取指定软件包的相关信息:
```shell
apk info {{软件包}}
```
{% endraw %}{% raw %}
<h2 id="aplay">
  <a href="/zh/linux/aplay.html">aplay</a> <a href="#aplay"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ALSA 声卡驱动程序的命令行声音播放器。
> 更多信息：<https://manned.org/aplay>.

#### 播放一个文件（会自动根据文件格式确定采样率、位深等）：
```shell
aplay {{文件路径}}
```
#### 以 2500 Hz 播放指定文件的前 10 秒：
```shell
aplay --duration={{10}} --rate={{2500}} {{文件路径}}
```
#### 以 22050 Hz，mono，8-bit，Mu-Law 和 `.au` 格式来播放指定原始文件：
```shell
aplay --channels={{1}} --file-type {{raw}} --rate={{22050}} --format={{mu_law}} {{文件路径}}
```
{% endraw %}{% raw %}
<h2 id="apport-bug">
  <a href="/zh/linux/apport-bug.html">apport-bug</a> <a href="#apport-bug"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在 Ubuntu 上提交错误报告。
> 更多信息：<https://wiki.ubuntu.com/Apport>.

#### 报告整个系统的错误：
```shell
apport-bug
```
#### 报告某个软件包的错误：
```shell
apport-bug {{包名}}
```
#### 报告某个可执行文件的错误：
```shell
apport-bug {{可执行文件路径}}
```
#### 报告某个进程的错误：
```shell
apport-bug {{PID}}
```
{% endraw %}{% raw %}
<h2 id="apt-add-repository">
  <a href="/zh/linux/apt-add-repository.html">apt-add-repository</a> <a href="#apt-add-repository"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 管理 apt 仓库。

#### 添加一个 apt 仓库：
```shell
apt-add-repository {{repository_spec}}
```
#### 移除一个 apt 仓库：
```shell
apt-add-repository --remove {{repository_spec}}
```
#### 添加一个 apt 仓库之后更新包缓存：
```shell
apt-add-repository --update {{repository_spec}}
```
#### 开启源码包：
```shell
apt-add-repository --enable-source {{repository_spec}}
```
{% endraw %}{% raw %}
<h2 id="apt-cache">
  <a href="/zh/linux/apt-cache.html">apt-cache</a> <a href="#apt-cache"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Debian 和 Ubuntu 的包查询工具.
> 更多信息： <https://manpages.debian.org/latest/apt/apt-cache.8.html>.

#### 在当前的软件源中查找一个软件包:
```shell
apt-cache search {{软件包}}
```
#### 显示指定软件包的相关信息:
```shell
apt-cache show {{软件包}}
```
#### 查看一个软件包是否安装或是否为最新:
```shell
apt-cache policy {{软件包}}
```
#### 显示一个软件包的依赖项:
```shell
apt-cache depends {{软件包}}
```
#### 列出依赖指定软件包的所有软件包:
```shell
apt-cache rdepends {{软件包}}
```
{% endraw %}{% raw %}
<h2 id="apt-file">
  <a href="/zh/linux/apt-file.html">apt-file</a> <a href="#apt-file"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在 apt 软件包中查找文件，其中也包括未安装的软件
> 更多信息： <https://manpages.debian.org/latest/apt-file/apt-file.1.html>.

#### 更新元数据的数据库:
```shell
sudo apt update
```
#### 查找包含指定文件或路径的软件包:
```shell
apt-file search {{文件名或路径}}
```
#### 列出指定包的内容:
```shell
apt-file list {{软件包名}}
```
{% endraw %}{% raw %}
<h2 id="apt-get">
  <a href="/zh/linux/apt-get.html">apt-get</a> <a href="#apt-get"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Debian 和 Ubuntu 的软件包管理工具.
> 使用`apt-cache`查找包.
> 更多信息： <https://manpages.debian.org/latest/apt/apt-get.8.html>.

#### 更新可用软件包及其版本列表（推荐在其他`apt-get`命令运行之前使用）:
```shell
apt-get update
```
#### 安装一个软件包或更新到最新版本:
```shell
apt-get install {{软件包}}
```
#### 移除一个软件包:
```shell
apt-get remove {{软件包}}
```
#### 升级所有已安装软件包到最新版本:
```shell
apt-get upgrade
```
#### 移除所有不再需要的软件包:
```shell
apt-get autoremove
```
#### 升级已安装的软件包（类似于`upgrade`）, 移除过时的软件包并安装额外的软件包以满足新的依赖:
```shell
apt-get dist-upgrade
```
{% endraw %}{% raw %}
<h2 id="apt-key">
  <a href="/zh/linux/apt-key.html">apt-key</a> <a href="#apt-key"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Debian 和 Ubuntu 上的 APT 软件包管理器的密钥管理工具
> 更多信息： <https://manpages.debian.org/latest/apt/apt-key.8.html>.

#### 列出可信密钥:
```shell
apt-key list
```
#### 向可信密钥库中添加一个密钥:
```shell
apt-key add {{密钥文件.asc}}
```
#### 从可信密钥库中移除一个密钥:
```shell
apt-key del {{密钥 id}}
```
#### 向可信密钥库中添加一个远程密钥:
```shell
wget -qO - {{https://host.tld/filename.key}} | apt-key add -
```
#### 指定密钥 ID, 从密钥服务器中添加一个密钥:
```shell
apt-key adv --keyserver {{pgp.mit.edu}} --recv {{密钥 id}}
```
{% endraw %}{% raw %}
<h2 id="apt-mark">
  <a href="/zh/linux/apt-mark.html">apt-mark</a> <a href="#apt-mark"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 修改已安装软件包状态的工具
> 更多信息： <https://manpages.debian.org/latest/apt/apt-mark.8.html>.

#### 将一个软件包标记为自动安装:
```shell
sudo apt-mark auto {{软件包名}}
```
#### 将一个软件包保持在当前版本，防止对其更新:
```shell
sudo apt-mark hold {{软件包名}}
```
#### 允许对一个软件包更新:
```shell
sudo apt-mark unhold {{软件包名}}
```
#### 列出手动安装的软件包:
```shell
apt-mark showmanual
```
#### 列出保持当前版本而不更新的软件包:
```shell
apt-mark showhold
```
{% endraw %}{% raw %}
<h2 id="apt">
  <a href="/zh/linux/apt.html">apt</a> <a href="#apt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 基于 Debian 的发行版上的软件包管理工具.
> 更多信息： <https://manpages.debian.org/latest/apt/apt.8.html>.

#### 更新可用软件包及其版本列表（推荐在运行其他 apt 命令前首先运行该命令）:
```shell
sudo apt update
```
#### 查找指定软件包:
```shell
apt search {{软件包}}
```
#### 显示关于指定软件包的信息:
```shell
apt show {{软件包}}
```
#### 安装指定软件包或将指定软件包更新到最新版本:
```shell
sudo apt install {{软件包}}
```
#### 移除指定软件包（使用`purge`可以同时移除其配置文件）:
```shell
sudo apt remove {{软件包}}
```
#### 将所有已安装软件包更新到最新可用版本:
```shell
sudo apt upgrade
```
{% endraw %}{% raw %}
<h2 id="aptitude">
  <a href="/zh/linux/aptitude.html">aptitude</a> <a href="#aptitude"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Debian 和 Ubuntu 上的软件包管理工具.
> 更多信息： <https://manpages.debian.org/latest/aptitude/aptitude.8.html>.

#### 同步可用软件包及其版本列表，在运行后续 aptitude 命令前，应该首先运行该命令:
```shell
aptitude update
```
#### 安装一个新的软件包及其依赖项:
```shell
aptitude install {{软件包}}
```
#### 查找软件包:
```shell
aptitude search {{软件包}}
```
#### 移除一个软件包并移除所有依赖它的软件包:
```shell
aptitude remove {{软件包}}
```
#### 更新已安装软件包到最新版本:
```shell
aptitude upgrade
```
#### 更新已安装的软件包（类似于`aptitude upgrade`命令）， 移除过时的软件包并安装额外的软件包以满足新的软件包依赖项:
```shell
aptitude full-upgrade
```
{% endraw %}{% raw %}
<h2 id="arch">
  <a href="/zh/linux/arch.html">arch</a> <a href="#arch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示当前系统架构名称.
> 参阅`uname`.

#### 显示当前系统架构名称:
```shell
arch
```
{% endraw %}{% raw %}
<h2 id="archey">
  <a href="/zh/linux/archey.html">archey</a> <a href="#archey"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一个可以以新颖的方式显示系统信息的简单工具.

#### 显示系统信息:
```shell
archey
```
{% endraw %}{% raw %}
<h2 id="archlinux-java">
  <a href="/zh/linux/archlinux-java.html">archlinux-java</a> <a href="#archlinux-java"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 提供 Java 环境设置功能的一个帮助脚本。
> 更多信息：<https://github.com/michaellass/archlinux-java-run>.

#### 列出已安装的 Java 环境：
```shell
archlinux-java status
```
#### 设置默认的 Java 环境：
```shell
archlinux-java set {{java_environment}}
```
#### 取消默认的 Java 环境：
```shell
archlinux-java unset
```
#### 自动设置默认的 Java 环境：
```shell
archlinux-java fix
```
{% endraw %}{% raw %}
<h2 id="arecored">
  <a href="/zh/linux/arecored.html">arecored</a> <a href="#arecored"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> ALSA 声卡驱动的声音录制器。
> 更多信息：<https://manned.org/aplay>.

#### 以 "CD" 质量录制一段声音（录制结束以 Ctrl-C 停止）：
```shell
arecord -vv --format=cd {{路径/文件名.wav}}
```
#### 以 "CD" 质量录制 10 秒钟声音：
```shell
arecord -vv --format=cd --duration={{10}} {{路径/文件名.wav}}
```
#### 录制一段声音并以 mp3 格式保存（录制结束以 Ctrl-C 停止）：
```shell
arecord -vv --format=cd --file-type raw | lame -r - {{路径/文件名.mp3}}
```
#### 列出所有的声卡和数字音频设备：
```shell
arecord --list-devices
```
#### 允许交互式界面（例如使用空格键或回车键来播放或暂停）：
```shell
arecord --interactive
```
{% endraw %}{% raw %}
<h2 id="arithmetic">
  <a href="/zh/linux/arithmetic.html">arithmetic</a> <a href="#arithmetic"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 测试见到你的算术问题。
> 更多信息：<https://manpages.debian.org/bsdgames/arithmetic.6.html>.

#### 开始算术测试：
```shell
arithmetic
```
#### 指定一个或多个算术运算符来设计问题：
```shell
arithmetic -o {{+|-|x|/}}
```
#### 指定范围。加法和乘法问题限定 0 到指定范围之间的数字，包含上区间。减法和除法问题限制结果和运算数字必须在 0 到指定范围之间：
```shell
arithmetic -r {{7}}
```
{% endraw %}{% raw %}
<h2 id="ark">
  <a href="/zh/linux/ark.html">ark</a> <a href="#ark"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> KDE 归档工具。
> 更多信息： <https://docs.kde.org/stable5/en/kdeutils/ark/>.

#### 将存档解压缩到当前目录：
```shell
ark --batch {{存档名}}
```
#### 改变解压缩目录：
```shell
ark --batch --destination {{解压缩目录路径}} {{存档名}}
```
#### 创建一个原本不存在的存档并向它添加文件：
```shell
ark --add-to {{存档名}} {{文件1}} {{文件2}}
```
{% endraw %}{% raw %}
<h2 id="arp-scan">
  <a href="/zh/linux/arp-scan.html">arp-scan</a> <a href="#arp-scan"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 发送 ARP 数据包到特定主机（指定 IP 地址或主机名），来扫描本地网络.

#### 扫描当前本地网络:
```shell
arp-scan --localnet
```
#### 扫描带有自定义位掩码的 IP 网络:
```shell
arp-scan {{192.168.1.1}}/{{24}}
```
#### 扫描自定义范围内的 IP 网络:
```shell
arp-scan {{127.0.0.0}}-{{127.0.0.31}}
```
#### 扫描带有自定义子网掩码的 IP 网络:
```shell
arp-scan {{10.0.0.0}}:{{255.255.255.0}}
```
{% endraw %}{% raw %}
<h2 id="as">
  <a href="/zh/linux/as.html">as</a> <a href="#as"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一个可移植的 GUN 汇编器.
> 主要用于汇编`gcc`的输出，以供链接器`ld`使用.

#### 汇编一个文件，输出为 a.out:
```shell
as {{文件.s}}
```
#### 汇编文件，并指定输出文件:
```shell
as {{文件.s}} -o {{输出.o}}
```
#### 通过跳过空格和注释的预处理过程来更快的产生输出文件（只应该用于可信任的编译器的输出）:
```shell
as -f {{文件.s}}
```
#### 将给定路径添加到目录列表，来搜索.include 指令指定的文件:
```shell
as -I {{目录路径}} {{文件.s}}
```
{% endraw %}{% raw %}
<h2 id="ascii">
  <a href="/zh/linux/ascii.html">ascii</a> <a href="#ascii"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示 ASCII 字符的别名。
> 更多信息：<http://www.catb.org/~esr/ascii/>.

#### 显示一个 ASCII 字符的别名：
```shell
ascii {{a}}
```
#### 以较短和脚本友好模式显示 ASCII 字符的别名：
```shell
ascii -t {{a}}
```
#### 显示多个 ASCII 字符的别名：
```shell
ascii -s {{tldr}}
```
#### 显示十进制 ASCII 字符表：
```shell
ascii -d
```
#### 显示十六进制 ASCII 字符表：
```shell
ascii -x
```
#### 显示八进制 ASCII 字符表：
```shell
ascii -o
```
#### 显示二进制 ASCII 字符表：
```shell
ascii -b
```
#### 显示选项总结和整个 ASCII 字符表：
```shell
ascii
```
{% endraw %}{% raw %}
<h2 id="asciiart">
  <a href="/zh/linux/asciiart.html">asciiart</a> <a href="#asciiart"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将图像转换为 ASCII.
> 更多信息: <https://github.com/nodanaonlyzuul/asciiart>.

#### 从文件中读取图像并以 ASCII 打印:
```shell
asciiart {{路径/image.jpg}}
```
#### 从 URL 中读取图像并以 ASCII 打印:
```shell
asciiart {{www.example.com/image.jpg}}
```
#### 选择输出宽度 (默认为 100):
```shell
asciiart -width {{50}} {{路径/image.jpg}}
```
#### 对 ASCII 输出进行着色:
```shell
asciiart --color {{路径/image.jpg}}
```
#### 选择输出格式 (默认格式为文本):
```shell
asciiart --format {{text|html}} {{路径/image.jpg}}
```
#### 反转字符映射:
```shell
asciiart --invert-chars {{路径/image.jpg}}
```
{% endraw %}{% raw %}
<h2 id="aspell">
  <a href="/zh/linux/aspell.html">aspell</a> <a href="#aspell"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 交互式拼写检查工具.

#### 为一个文件做拼写检查:
```shell
aspell check {{文件路径}}
```
#### 列出来自标准输入的拼写错误单词:
```shell
cat {{文件}} | aspell list
```
#### 列出可用的字典语言:
```shell
aspell dicts
```
#### 指定不同的语言（取 ISO 639 语言代码的 2 个字母）来运行 aspell:
```shell
aspell --lang={{cs}}
```
#### 列出来自标准输入的拼写错误单词，并且忽略个人单词列表中的单词:
```shell
cat {{文件}} | aspell --personal={{个人单词列表.pws}} {{列表}}
```
{% endraw %}{% raw %}
<h2 id="asterisk">
  <a href="/zh/linux/asterisk.html">asterisk</a> <a href="#asterisk"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 电话和交换（手机）服务器。
> 用于管理服务器自身和管理已经在运行的实例。
> 更多信息：<https://wiki.asterisk.org/wiki/display/AST/Home>.

#### 重新连接一个正在运行的服务器，并打开 3 级的日志详细度：
```shell
asterisk -r -vvv
```
#### 重新连接一个正在运行的服务器，执行一个命令，然后返回：
```shell
asterisk -r -x "{{命令}}"
```
#### 显示 chan_SIP 客户端（手机）：
```shell
asterisk -r -x "sip show peers"
```
#### 显示激活的通话和频道：
```shell
asterisk -r -x "core show channels"
```
#### 显示语音邮箱：
```shell
asterisk -r -x "voicemail show users"
```
#### 终止一个频道：
```shell
asterisk -r -x "hangup request {{频道 ID}}"
```
#### 重新载入 chan_SIP 设置：
```shell
asterisk -r -x "sip reload"
```
{% endraw %}{% raw %}
<h2 id="at">
  <a href="/zh/linux/at.html">at</a> <a href="#at"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在指定时间执行命令.
> 更多信息： <https://man.archlinux.org/man/at.1>.

#### 打开`at`提示符创建一组新的定时命令，按`Ctrl + D`保存并退出:
```shell
at {{hh:mm:ss}}
```
#### 运行命令并通过本地电子邮件程序（例如 sendmail) 发送运行结果:
```shell
at {{hh:mm:ss}} -m
```
#### 在指定时间执行一个脚本:
```shell
at {{hh:mm:ss}} -f {{文件路径}}
```
{% endraw %}{% raw %}
<h2 id="auracle">
  <a href="/zh/linux/auracle.html">auracle</a> <a href="#auracle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用来和 Arch Linux 用户仓库交互的命令行工具，这个仓库通常被称作 AUR。
> 更多信息：<https://github.com/falconindy/auracle>.

#### 显示符合一个正则表达式的 AUR 包：
```shell
auracle search '{{regular_expression}}'
```
#### 显示 AUR 包列表的包信息，包名以一个单独的空格分隔：
```shell
auracle info {{package1}} {{package2}}
```
#### 显示 AUR 包列表的 `PKGBUILD` 文件（编译信息），包名以一个单独的空格分隔：
```shell
auracle show {{package1}} {{package2}}
```
#### 显示已安装 AUR 包的更新：
```shell
auracle outdated
```
{% endraw %}{% raw %}
<h2 id="authconfig">
  <a href="/zh/linux/authconfig.html">authconfig</a> <a href="#authconfig"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用于设置系统认证资源的命令行界面。

#### 显示当前的配置（或空运行）：
```shell
authconfig --test
```
#### 设置服务器使用另一种不同的密码散列算法：
```shell
authconfig --update --passalgo={{算法名}}
```
#### 启用 LDAP 认证：
```shell
authconfig --update --enableldapauth
```
#### 关闭 LDAP 认证：
```shell
authconfig --update --disableldapauth
```
#### 开启网络信息服务（NIS）：
```shell
authconfig --update --enablenis
```
#### 开启 Kerberos：
```shell
authconfig --update --enablekrb5
```
#### 开启 Winbind （活动目录）认证：
```shell
authconfig --update --enablewinbindauth
```
#### 开启本地认证：
```shell
authconfig --update --enablelocauthorize
```
{% endraw %}{% raw %}
<h2 id="autorandr">
  <a href="/zh/linux/autorandr.html">autorandr</a> <a href="#autorandr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 自动调节屏幕布局。

#### 保存当前屏幕布局：
```shell
autorandr -s {{配置文件名}}
```
#### 显示保存的配置：
```shell
autorandr
```
#### 切换设置：
```shell
autorandr -l {{配置文件名}}
```
#### 设置默认设置：
```shell
autorandr -d {{配置文件名}}
```
{% endraw %}{% raw %}
<h2 id="avahi-browse">
  <a href="/zh/linux/avahi-browse.html">avahi-browse</a> <a href="#avahi-browse"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示通过 mDNS/DNS-SD 暴露在本地网络的服务和主机。
> Avahi 与苹果设备的 Bonjour (Zeroconf) 兼容。
> 更多信息：<https://www.avahi.org/>.

#### 列出本地网络中的所有服务和他们的地址与端口，忽略他们本地的地址和端口：
```shell
avahi-browse --all --resolve --ignore-local
```
#### 列出所有的域名：
```shell
avahi-browse --browse-domains
```
#### 只搜索一个特定的域名：
```shell
avahi-browse --all --domain={{domain}}
```
{% endraw %}{% raw %}
<h2 id="boltctl">
  <a href="/zh/linux/boltctl.html">boltctl</a> <a href="#boltctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 控制雷电 (thunderbolt) 设备。
> 更多信息：<https://manned.org/boltctl>.

#### 列出已连接并授权的设备：
```shell
boltctl
```
#### 列出已连接的设备，且包含未授权的设备：
```shell
boltctl list
```
#### 临时授权一个设备：
```shell
boltctl authorize {{设备uuid}}
```
#### 授权并记住一个设备：
```shell
boltctl enroll {{设备uuid}}
```
#### 取消一个设备的授权：
```shell
boltctl forget {{设备uuid}}
```
#### 显示一个设备的详细信息：
```shell
boltctl info {{设备uuid}}
```
{% endraw %}{% raw %}
<h2 id="btrfs-device">
  <a href="/zh/linux/btrfs-device.html">btrfs device</a> <a href="#btrfs-device"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 管理 btrfs 文件系统中的设备。
> 更多信息：<https://btrfs.wiki.kernel.org/index.php/Manpage/btrfs-device>。

#### 将一个或多个设备添加到 b​​trfs 文件系统中：
```shell
sudo btrfs device add {{指向设备1的路径}} [{{指向设备2的路径}}] {{指向 btrfs 文件系统的路径}}
```
#### 从 btrfs 文件系统中删除设备：
```shell
sudo btrfs device remove {{指向设备的路径|设备 ID}} [{{...}}]
```
#### 显示错误统计：
```shell
sudo btrfs device stats {{指向 btrfs 文件系统的路径}}
```
#### 扫描所有磁盘并将所有检测到的 btrfs 文件系统通知内核：
```shell
sudo btrfs device scan --all-devices
```
#### 显示详细的每个磁盘的空间分配统计信息：
```shell
sudo btrfs device usage {{指向 btrfs 文件系统的路径}}
```
{% endraw %}{% raw %}
<h2 id="btrfs-filesystem">
  <a href="/zh/linux/btrfs-filesystem.html">btrfs filesystem</a> <a href="#btrfs-filesystem"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 管理 btrfs 文件系统。
> 更多信息：<https://btrfs.wiki.kernel.org/index.php/Manpage/btrfs-filesystem>。

#### 显示文件系统使用情况（可以选择以 root 身份运行以显示详细信息）：
```shell
btrfs filesystem usage {{指向挂载点的路径}}
```
#### 显示各个设备的使用情况：
```shell
sudo btrfs filesystem show {{指向挂载点的路径}}
```
#### 对 btrfs 文件系统上的单个文件进行碎片整理（避免在运行数据去重的同时运行）：
```shell
sudo btrfs filesystem defragment -v {{指向文件的路径}}
```
#### 递归对目录进行碎片整理（不跨越子卷边界）：
```shell
sudo btrfs filesystem defragment -v -r {{指向目录的路径}}
```
#### 强制将未写入的数据块同步到磁盘：
```shell
sudo btrfs filesystem sync {{指向挂载点的路径}}
```
#### 递归总结目录中文件的磁盘使用情况：
```shell
sudo btrfs filesystem du --summarize {{指向目录的路径}}
```
{% endraw %}{% raw %}
<h2 id="btrfs-scrub">
  <a href="/zh/linux/btrfs-scrub.html">btrfs scrub</a> <a href="#btrfs-scrub"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 清理 btrfs 文件系统以验证数据完整性。
> 建议每月运行一次 scrub。
> 更多信息：<https://btrfs.wiki.kernel.org/index.php/Manpage/btrfs-scrub>。

#### 开始 scrub：
```shell
sudo btrfs scrub start {{指向挂载点的路径}}
```
#### 显示正在进行或上次完成的 scrub 的状态：
```shell
sudo btrfs scrub status {{指向挂载点的路径}}
```
#### 取消正在进行的 scrub：
```shell
sudo btrfs scrub cancel {{指向挂载点的路径}}
```
#### 恢复先前取消的 scrub：
```shell
sudo btrfs scrub resume {{指向挂载点的路径}}
```
#### 开始擦洗，但要等到 scrub 完成后才能退出：
```shell
sudo btrfs scrub start -B {{指向挂载点的路径}}
```
#### 在安静模式下启动 scrub（不打印错误或统计信息）：
```shell
sudo btrfs scrub start -q {{指向挂载点的路径}}
```
{% endraw %}{% raw %}
<h2 id="btrfs-subvolume">
  <a href="/zh/linux/btrfs-subvolume.html">btrfs subvolume</a> <a href="#btrfs-subvolume"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 管理 btrfs 子卷和快照。
> 更多信息：<https://btrfs.wiki.kernel.org/index.php/Manpage/btrfs-subvolume>。

#### 创建一个新的空子卷：
```shell
sudo btrfs subvolume create {{指向新子卷的路径}}
```
#### 列出指定文件系统中的所有子卷和快照：
```shell
sudo btrfs subvolume list {{指向 btrfs 文件系统的路径}}
```
#### 删除一个子卷：
```shell
sudo btrfs subvolume delete {{指向子卷的路径}}
```
#### 创建现有子卷的只读快照：
```shell
sudo btrfs subvolume snapshot -r {{指向源子卷的路径}} {{指向目标的路径}}
```
#### 创建现有子卷的读写快照：
```shell
sudo btrfs subvolume snapshot {{指向源子卷的路径}} {{指向目标的路径}}
```
#### 显示有关子卷的详细信息：
```shell
sudo btrfs subvolume show {{指向子卷的路径}}
```
{% endraw %}{% raw %}
<h2 id="btrfs">
  <a href="/zh/linux/btrfs.html">btrfs</a> <a href="#btrfs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一种基于写时复制（COW）原理的 Linux 文件系统。

#### 创建子卷：
```shell
sudo btrfs subvolume create {{指向子卷的路径}}
```
#### 列出子卷：
```shell
sudo btrfs subvolume list {{指向挂载点的路径}}
```
#### 显示空间使用情况信息：
```shell
sudo btrfs filesystem df {{指向挂载点的路径}}
```
#### 启用配额（quota）：
```shell
sudo btrfs quota enable {{指向子卷的路径}}
```
#### 显示配额（quota）：
```shell
sudo btrfs qgroup show {{指向子卷的路径}}
```
{% endraw %}{% raw %}
<h2 id="cpuid">
  <a href="/zh/linux/cpuid.html">cpuid</a> <a href="#cpuid"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示有关所有 CPU 的详细信息.

#### 显示所有 CPU 的信息:
```shell
cpuid
```
#### 仅显示当前 CPU 的信息:
```shell
cpuid -1
```
#### 显示原始十六进制信息，不进行解码:
```shell
cpuid -r
```
{% endraw %}{% raw %}
<h2 id="debootstrap">
  <a href="/zh/linux/debootstrap.html">debootstrap</a> <a href="#debootstrap"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 创建一个基本的 `Debian` 系统。
> 更多信息：<https://wiki.debian.org/Debootstrap>.

#### 在 `debian-root` 目录中创建一个 `Debian` 稳定分支系统：
```shell
sudo debootstrap stable {{path/to/debian-root/}} http://deb.debian.org/debian
```
#### 使用本地镜像在 `focal-root` 目录中创建一个 `Ubuntu 20.04` 系统：
```shell
sudo debootstrap focal {{path/to/focal-root/}} {{file:///path/to/mirror/}}
```
#### 切换到可引导系统：
```shell
sudo chroot {{path/to/root}}
```
#### 列出可用的版本：
```shell
ls /usr/share/debootstrap/scripts/
```
{% endraw %}{% raw %}
<h2 id="debuild">
  <a href="/zh/linux/debuild.html">debuild</a> <a href="#debuild"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 从源代码构建 `Debian` 软件包的工具。
> 更多信息：<https://manpages.debian.org/debuild>.

#### 在当前目录中生成软件包：
```shell
debuild
```
#### 仅构建二进制包：
```shell
debuild -b
```
#### 生成软件包后，不运行 `lintian` （检查常见打包错误）：
```shell
debuild --no-lintian
```
{% endraw %}{% raw %}
<h2 id="dmenu">
  <a href="/zh/linux/dmenu.html">dmenu</a> <a href="#dmenu"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 动态菜单。
> 根据文本输入创建菜单，其中每一项都在新行中。

#### 显示 `ls` 命令输出的菜单：
```shell
{{ls}} | dmenu
```
#### 显示包含自定义项目的菜单，并用新行（`\n`）分隔：
```shell
echo -e "{{red}}\n{{green}}\n{{blue}}" | dmenu
```
#### 让用户在多个项目之间进行选择，然后将所选项目保存到文件中：
```shell
echo -e "{{red}}\n{{green}}\n{{blue}}" | dmenu > {{color.txt}}
```
#### 在特定的监视器上启动 `dmenu`：
```shell
ls | dmenu -m {{1}}
```
#### 在屏幕底部显示 `dmenu`：
```shell
ls | dmenu -b
```
{% endraw %}{% raw %}
<h2 id="dmesg">
  <a href="/zh/linux/dmesg.html">dmesg</a> <a href="#dmesg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示或控制内核环形缓冲区。
> 更多信息：<https://manned.org/dmesg>.

#### 显示来自内核环形缓冲区的所有消息：
```shell
dmesg
```
#### 只显示严重错误级别的消息：
```shell
dmesg --level err
```
#### 等待新消息。仅在具有可读性的系统上支持此功能，类似于 `tail -f`（从内核 3.5.0 版本开始）：
```shell
dmesg -w
```
#### 显示此系统上有多少物理内存可用：
```shell
dmesg | grep -i memory
```
#### 以分页方式显示内核缓冲区的所有消息：
```shell
dmesg | less
```
#### 打印人类可读的时间戳（从内核 3.5.0 版本开始）：
```shell
dmesg -T
```
#### 启用人类可读的输出：
```shell
dmesg -H
```
#### 着色输出：
```shell
dmesg -L
```
{% endraw %}{% raw %}
<h2 id="dos2unix">
  <a href="/zh/linux/dos2unix.html">dos2unix</a> <a href="#dos2unix"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将 DOS 样式的行尾更改为 Unix 样式.
> 用 CR 替换 CRLF.

#### 更改文件的行尾:
```shell
dos2unix {{文件名}}
```
#### 使用 Unix 样式的行尾创建副本:
```shell
dos2unix -n {{文件名}} {{文件名}}
```
{% endraw %}{% raw %}
<h2 id="fc-cache">
  <a href="/zh/linux/fc-cache.html">fc-cache</a> <a href="#fc-cache"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 扫描字体目录，以便建立字体缓存文件。

#### 生成字体缓存文件：
```shell
fc-cache
```
#### 强制重建所有字体缓存文件，而不检查缓存是否为最新版本：
```shell
fc-cache -f
```
#### 删除字体缓存文件，然后生成新的字体缓存文件：
```shell
fc-cache -r
```
{% endraw %}{% raw %}
<h2 id="fc-list">
  <a href="/zh/linux/fc-list.html">fc-list</a> <a href="#fc-list"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 列出系统上安装的可用字体。

#### 返回系统中已安装字体的列表：
```shell
fc-list
```
#### 返回具有给定名称的已安装字体的列表：
```shell
fc-list | grep '{{DejaVu Serif}}'
```
#### 返回系统中已安装字体的数量：
```shell
fc-list | wc -l
```
{% endraw %}{% raw %}
<h2 id="flameshot">
  <a href="/zh/linux/flameshot.html">flameshot</a> <a href="#flameshot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 带有gui界面的Screenshot工具，支持基本的图像编辑，例如文本，形状，颜色和imgur.
> 更多信息: <https://flameshot.js.org>.

#### 在GUI模式下启动Flameshot:
```shell
flameshot launcher
```
#### 通过单击并拖动来截取屏幕截图:
```shell
flameshot gui
```
#### 全屏截图:
```shell
flameshot full
```
#### 将保存屏幕快照的路径设置为:
```shell
flameshot full --path {{path/to/directory}}
```
#### 将屏幕截图延迟N毫秒，然后输出到剪贴板:
```shell
flameshot full --delay {{2000}} --clipboard
```
{% endraw %}{% raw %}
<h2 id="flatpak">
  <a href="/zh/linux/flatpak.html">flatpak</a> <a href="#flatpak"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 构建、安装和运行 Flatpak 应用和运行时。

#### 运行已安装应用：
```shell
flatpak run {{应用名}}
```
#### 从远程源安装应用：
```shell
flatpak install {{远程源名}} {{应用名}}
```
#### 列出所有应用和运行时：
```shell
flatpak list
```
#### 更新所有已安装的应用和运行时：
```shell
flatpak update
```
#### 添加远程源：
```shell
flatpak remote-add --if-not-exists {{远程源名}} {{远程源网址}}
```
#### 列出所有已配置的远程源：
```shell
flatpak remote-list
```
{% endraw %}{% raw %}
<h2 id="i3">
  <a href="/zh/linux/i3.html">i3</a> <a href="#i3"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一款动态平铺窗口管理器。
> 更多信息：https://i3wm.org/docs/userguide.html>.

#### 启动 i3（注意在此命令运行前，务必关闭其它先前存在的窗口管理器）：
```shell
i3
```
#### 打开新终端窗口：
```shell
Super + Return
```
#### 创建新工作区：
```shell
Super + Shift + {{数字键}}
```
#### 切换到 {{数字}} 号工作区：
```shell
Super + {{数字键}}
```
#### 水平布局打开新窗口：
```shell
Super + h
```
#### 垂直布局打开新窗口：
```shell
Super + v
```
#### 打开应用（在执行命令后输入应用名称）：
```shell
Super + D
```
{% endraw %}{% raw %}
<h2 id="iptables">
  <a href="/zh/linux/iptables.html">iptables</a> <a href="#iptables"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 可用于配置 Linux 内核防火墙提供的过滤表、规则链和规则的程序。
> 更多信息： <https://www.netfilter.org/projects/iptables/>.

#### 查看过滤表的规则链、规则以及数据包/字节计数器：
```shell
sudo iptables -vnL
```
#### 设定规则链策略规则：
```shell
sudo iptables -P {{规则链}} {{规则}}
```
#### 追加规则到 IP 的规则链策略：
```shell
sudo iptables -A {{规则链}} -s {{ip}} -j {{规则}}
```
#### 追加规则到 IP 的规则链策略（考虑协议与端口）：
```shell
sudo iptables -A {{规则链}} -s {{ip}} -p {{协议}} --dport {{端口}} -j {{规则}}
```
#### 删除规则链中的规则：
```shell
sudo iptables -D {{规则链}} {{规则所在行号}}
```
#### 将指定过滤表的 iptables 配置保存到文件中：
```shell
sudo iptables-save -t {{过滤表名}} > {{iptables_文件路径}}
```
#### 从文件中还原 iptables 配置：
```shell
sudo iptables-restore < {{iptables_文件路径}}
```
{% endraw %}{% raw %}
<h2 id="konsole">
  <a href="/zh/linux/konsole.html">konsole</a> <a href="#konsole"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Konsole: KDE 终端模拟器.
> 更多信息: <https://konsole.kde.org>.

#### 在特定目录中打开一个新的 Konsole:
```shell
konsole --workdir {{path/to/directory}}
```
#### 运行特定命令，退出窗口后不要关闭窗口:
```shell
konsole --noclose -e {{命令}}
```
#### 打开新标签页:
```shell
konsole --new-tab
```
#### 在后台打开 Konsole 并在按下 Ctrl+Shift+F12 (默认) 时显示在最前面:
```shell
konsole --background-mode
```
#### 使用紧急备冗配置文件打开 Konsole:
```shell
konsole --fallback-profile
```
{% endraw %}{% raw %}
<h2 id="logsave">
  <a href="/zh/linux/logsave.html">logsave</a> <a href="#logsave"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将一个命令的输出保存在日志文件中.
> 更多信息: <https://manned.org/logsave>.

#### 使用指定的参数执行命令并将其输出保存到日志文件中:
```shell
logsave {{path/to/logfile}} {{command}}
```
#### 从标准输入中获取输入并将其保存在日志文件中:
```shell
logsave {{logfile}} -
```
#### 将输出追加到日志文件，而不是替换其当前内容:
```shell
logsave -a {{logfile}} {{command}}
```
#### 显示详细输出:
```shell
logsave -v {{logfile}} {{command}}
```
{% endraw %}{% raw %}
<h2 id="mac2unix">
  <a href="/zh/linux/mac2unix.html">mac2unix</a> <a href="#mac2unix"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将 macOS 样式的行尾更改为 Unix 样式.
> 用 CR 替换 LF.

#### 更改文件的行尾:
```shell
mac2unix {{文件名}}
```
#### 使用 Unix 样式的行尾创建副本:
```shell
mac2unix -n {{文件名}} {{新文件名}}
```
{% endraw %}{% raw %}
<h2 id="pacman">
  <a href="/zh/linux/pacman.html">pacman</a> <a href="#pacman"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux 的软件包管理器工具。
> 更多信息: <https://man.archlinux.org/man/pacman.8>.

#### 同步并更新所有软件包：
```shell
pacman -Syu
```
#### 安装一个新的软件包：
```shell
pacman -S {{软件包}}
```
#### 删除一个软件包及其依赖：
```shell
pacman -Rs {{软件包}}
```
#### 在软件包数据库中搜索正则表达式或关键字：
```shell
pacman -Ss "{{软件包}}"
```
#### 列出已安装的软件包和版本：
```shell
pacman -Q
```
#### 仅列出明确安装的软件包和版本：
```shell
pacman -Qe
```
#### 查找哪个包拥有某个文件：
```shell
pacman -Qo {{文件名}}
```
#### 清空软件包缓存以释放空间：
```shell
pacman -Scc
```
{% endraw %}{% raw %}
<h2 id="poweroff">
  <a href="/zh/linux/poweroff.html">poweroff</a> <a href="#poweroff"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 关闭系统.

#### 关闭系统电源:
```shell
sudo poweroff
```
{% endraw %}{% raw %}
<h2 id="reboot">
  <a href="/zh/linux/reboot.html">reboot</a> <a href="#reboot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 重新启动系统.

#### 立即重新启动:
```shell
reboot
```
#### 立即重启，而无需正常关闭:
```shell
reboot -f
```
{% endraw %}{% raw %}
<h2 id="unix2dos">
  <a href="/zh/linux/unix2dos.html">unix2dos</a> <a href="#unix2dos"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将 Unix 样式的行尾更改为 DOS 样式.
> 用 CRLF 替换 CR.

#### 更改文件的行尾:
```shell
unix2dos {{文件名}}
```
#### 使用 DOS 样式的行尾创建副本:
```shell
unix2dos -n {{文件名}} {{新文件名}}
```
{% endraw %}{% raw %}
<h2 id="unix2mac">
  <a href="/zh/linux/unix2mac.html">unix2mac</a> <a href="#unix2mac"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将 Unix 样式的行尾更改为 macOS 样式.
> 用 LF 替换 CR.

#### 更改文件的行尾:
```shell
unix2mac {{文件名}}
```
#### 使用 macOS 样式的行尾创建副本:
```shell
unix2mac -n {{文件名}} {{新文件名}}
```
{% endraw %}{% raw %}
<h2 id="yaourt">
  <a href="/zh/linux/yaourt.html">yaourt</a> <a href="#yaourt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Arch Linux 中用于从 Arch User Repository 中构建软件包的工具。

#### 同步并更新所有软件包（包括 AUR）：
```shell
yaourt -Syua
```
#### 安装一个新的软件包（包括 AUR）：
```shell
yaourt -S {{软件包}}
```
#### 移除一个软件包和它的依赖（包括 AUR 软件包）：
```shell
yaourt -Rs {{软件包}}
```
#### 在软件包数据库中搜索一个关键字（包括 AUR）：
```shell
yaourt -Ss {{软件包}}
```
#### 列出已安装的软件包、版本和仓库（AUR 软件包将被列在 'local' 仓库下):
```shell
yaourt -Q
```
{% endraw %}{% raw %}
<h2 id="yay">
  <a href="/zh/linux/yay.html">yay</a> <a href="#yay"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Yet Another Yogurt: 一个用于 Arch Linux 的工具，用于从 Arch User Repository 中构建和安装软件包。
> 另见 `pacman`。
> 更多信息: <https://github.com/Jguer/yay>.

#### 从仓库和 AUR 中交互式搜索和安装软件包：
```shell
yay {{软件包|搜索词}}
```
#### 同步并更新所有来自仓库和 AUR 的软件包：
```shell
yay
```
#### 只同步和更新 AUR 软件包：
```shell
yay -Sua
```
#### 从仓库和 AUR 中安装一个新的软件包。
```shell
yay -S {{软件包}}
```
#### 从仓库和 AUR 中搜索软件包数据库中的关键词：
```shell
yay -Ss {{关键词}}
```
#### 显示已安装软件包和系统健康状况的统计数据：
```shell
yay -Ps
```
{% endraw %}{% raw %}
<h2 id="zypper">
  <a href="/zh/linux/zypper.html">zypper</a> <a href="#zypper"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> SUSE & openSUSE 的软件包管理工具。

#### 同步可用的软件包和版本列表：
```shell
zypper refresh
```
#### 安装一个新的软件包：
```shell
zypper install {{软件包}}
```
#### 移除一个软件包：
```shell
zypper remove {{软件包}}
```
#### 将已安装的软件包升级到最新的可用版本：
```shell
zypper update
```
#### 通过关键字搜索软件包：
```shell
zypper search {{关键字}}
```
{% endraw %}