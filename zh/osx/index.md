---
layout: default
title: "osx"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#getfileinfo">GetFileInfo</a>
* <a href="#afinfo">afinfo</a>
* <a href="#airport">airport</a>
* <a href="#apachectl">apachectl</a>
* <a href="#archey">archey</a>
* <a href="#as">as</a>
* <a href="#asr">asr</a>
* <a href="#base64">base64</a>
* <a href="#brew">brew</a>
* <a href="#brew-cask">brew cask</a>
* <a href="#brew-mas">brew mas</a>
* <a href="#brightness">brightness</a>
* <a href="#caffeinate">caffeinate</a>
* <a href="#cal">cal</a>
* <a href="#carthage">carthage</a>
* <a href="#chflags">chflags</a>
* <a href="#codesign">codesign</a>
* <a href="#compgen">compgen</a>
* <a href="#date">date</a>
* <a href="#dd">dd</a>
* <a href="#defaults">defaults</a>
* <a href="#diskutil">diskutil</a>
* <a href="#ditto">ditto</a>
* <a href="#dmesg">dmesg</a>
* <a href="#drutil">drutil</a>
* <a href="#du">du</a>
* <a href="#duti">duti</a>
* <a href="#eval">eval</a>
* <a href="#export">export</a>
* <a href="#fc">fc</a>
* <a href="#feh">feh</a>
* <a href="#file">file</a>
* <a href="#fsck">fsck</a>
* <a href="#head">head</a>
* <a href="#hexdump">hexdump</a>
* <a href="#hostname">hostname</a>
* <a href="#imgcat">imgcat</a>
* <a href="#launchctl">launchctl</a>
* <a href="#lldb">lldb</a>
* <a href="#locate">locate</a>
* <a href="#logger">logger</a>
* <a href="#look">look</a>
* <a href="#m">m</a>
* <a href="#md5">md5</a>
* <a href="#mdfind">mdfind</a>
* <a href="#mdutil">mdutil</a>
* <a href="#mkfile">mkfile</a>
* <a href="#n">n</a>
* <a href="#netstat">netstat</a>
* <a href="#networksetup">networksetup</a>
* <a href="#oathtool">oathtool</a>
* <a href="#open">open</a>
* <a href="#opensnoop">opensnoop</a>
* <a href="#osascript">osascript</a>
* <a href="#pbcopy">pbcopy</a>
* <a href="#pbpaste">pbpaste</a>
* <a href="#pdfgrep">pdfgrep</a>
* <a href="#ping">ping</a>
* <a href="#pmset">pmset</a>
* <a href="#pod">pod</a>
* <a href="#popd">popd</a>
* <a href="#port">port</a>
* <a href="#pushd">pushd</a>
* <a href="#pwgen">pwgen</a>
* <a href="#qlmanage">qlmanage</a>
* <a href="#reboot">reboot</a>
* <a href="#route">route</a>
* <a href="#rubocop">rubocop</a>
* <a href="#say">say</a>
* <a href="#scutil">scutil</a>
* <a href="#sed">sed</a>
* <a href="#shuf">shuf</a>
* <a href="#shutdown">shutdown</a>
* <a href="#sips">sips</a>
* <a href="#softwareupdate">softwareupdate</a>
* <a href="#split">split</a>
* <a href="#ssh-add">ssh-add</a>
* <a href="#sshuttle">sshuttle</a>
* <a href="#stat">stat</a>
* <a href="#sw_vers">sw_vers</a>
* <a href="#sysctl">sysctl</a>
* <a href="#system_profiler">system_profiler</a>
* <a href="#systemsetup">systemsetup</a>
* <a href="#textutil">textutil</a>
* <a href="#top">top</a>
* <a href="#trap">trap</a>
* <a href="#tree">tree</a>
* <a href="#uname">uname</a>
* <a href="#w">w</a>
* <a href="#wacaw">wacaw</a>
* <a href="#whereis">whereis</a>
* <a href="#wifi-password">wifi-password</a>
* <a href="#xattr">xattr</a>
* <a href="#xcodebuild">xcodebuild</a>
* <a href="#xctool">xctool</a>
* <a href="#xed">xed</a>
* <a href="#xsltproc">xsltproc</a>
* <a href="#yank">yank</a>

{% raw %}
<h2 id="afinfo">
  <a href="/zh/osx/afinfo.html">afinfo</a> <a href="#afinfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示音频文件元数据 (Metadata) 详细信息 (OS X).
> OS X 自带命令.

#### 显示给定音频文件的详细信息:
```shell
afinfo {{目标 / 路径 / 文件}}
```
#### 显示简化的音频文件信息 (单行):
```shell
afinfo -b {{目标 / 路径 / 文件}}
```
#### 显示音频文件的元数据信息以及其 InfoDictionary 词典:
```shell
afinfo -i {{目标 / 路径 / 文件}}
```
#### 以 xml 格式显示音频文件信息:
```shell
afinfo -x {{目标 / 路径 / 文件}}
```
#### 显示警告信息 (如存在):
```shell
afinfo --warnings {{目标 / 路径 / 文件}}
```
#### 显示完整用法帮助:
```shell
afinfo -h
```
{% endraw %}{% raw %}
<h2 id="airport">
  <a href="/zh/osx/airport.html">airport</a> <a href="#airport"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 无线网络配置工具.

#### 显示当前的无线状态信息:
```shell
airport -I
```
#### 在通道 1 上监察（嗅探）无线流量:
```shell
airport sniff {{1}}
```
#### 扫描可用的无线网络:
```shell
airport -s
```
#### 与当前的 Airport 网络脱离连接:
```shell
sudo airport -z
```
{% endraw %}{% raw %}
<h2 id="apachectl">
  <a href="/zh/osx/apachectl.html">apachectl</a> <a href="#apachectl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用于 macOS 的 Apache HTTP Server 控制接口（工具）.

#### 启动 org.apache.httpd 服务:
```shell
apachectl start
```
#### 停止已启动的服务:
```shell
apachectl stop
```
#### 重新启动服务:
```shell
apachectl restart
```
{% endraw %}{% raw %}
<h2 id="archey">
  <a href="/zh/osx/archey.html">archey</a> <a href="#archey"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 漂亮地显示简单系统信息工具.

#### 显示系统信息（彩色的）:
```shell
archey
```
#### 显示系统信息（单色的）:
```shell
archey --nocolor
```
#### 显示系统信息，使用 MacPorts（命令行软件安装管理工具 port) 来替代 Homebrew（另一种更常用的 mac 命令行软件安装管理工具）:
```shell
archey --macports
```
#### 显示系统信息，但不进行 IP 地址获取和验证:
```shell
archey --offline
```
{% endraw %}{% raw %}
<h2 id="as">
  <a href="/zh/osx/as.html">as</a> <a href="#as"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 便携式 GNU 汇编程序.
> 主要用于汇编 `gcc` 的输出以供 `ld` 使用

#### 汇编文件，将输出写入 a.out:
```shell
as {{文件.s}}
```
#### 将输出汇编到给定文件:
```shell
as {{文件.s}} -o {{输出.o}}
```
#### 通过跳过空白和注释预处理来更快地生成输出.（应该只用于受信任的编译器）:
```shell
as -f {{文件.s}}
```
#### 在目录列表中包含一个给定路径，以搜索 .include 指令中指定的文件:
```shell
as -I {{目标文件夹}} {{文件.s}}
```
{% endraw %}{% raw %}
<h2 id="asr">
  <a href="/zh/osx/asr.html">asr</a> <a href="#asr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将磁盘映像还原（复制）到卷上.
> 命令名称是 Apple Software Restore 的缩写.

#### 将磁盘映像复制到目标卷:
```shell
sudo asr restore --source {{映像名}}.dmg --target {{卷路径}}
```
#### 在复制之前擦除目标卷:
```shell
sudo asr restore --source {{映像名}}.dmg --target {{卷路径}} --erase
```
#### 恢复后跳过验证步骤:
```shell
sudo asr restore --source {{映像名}}.dmg --target {{卷路径}} --noverify
```
#### 不使用中间磁盘映像直接复制卷中的数据:
```shell
sudo asr restore --source {{卷路径}} --target {{复制卷路径}}
```
{% endraw %}{% raw %}
<h2 id="base64">
  <a href="/zh/osx/base64.html">base64</a> <a href="#base64"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 使用 Base64 来进行编码和解码.

#### 编码目标文件:
```shell
base64 --input={{目标文件}}
```
#### 解码目标文件:
```shell
base64 --decode --input={{base64 编码文件}}
```
#### 通过标准输入管道进行解码:
```shell
echo -n {{目标字符串}} | base64
```
#### 解码标准输入管道内容:
```shell
echo -n {{base64 字符串}} | base64 --decode
```
{% endraw %}{% raw %}
<h2 id="brew-cask">
  <a href="/zh/osx/brew-cask.html">brew cask</a> <a href="#brew-cask"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> macOS 上的应用程序包管理工具.

#### 模糊搜索可用命令行工具和软件包:
```shell
brew search {{软件名}}
```
#### 安装一个软件:
```shell
brew cask install {{软件名}}
```
#### 列出全部已安装软件:
```shell
brew cask list
```
#### 列出全部已安装的软件中，可以升级的:
```shell
brew cask outdated
```
#### 将一个已安装的软件升级到最新的版本:
```shell
brew cask upgrade {{软件名}}
```
#### 删除一个软件（仅通过 brew cask install 方式安装的）:
```shell
brew cask uninstall {{软件名}}
```
#### 卸载一个软件并删除相关的设置和文件:
```shell
brew cask zap {{软件名}}
```
#### 显示指定软件的相关信息:
```shell
brew cask info {{软件名}}
```
{% endraw %}{% raw %}
<h2 id="brew-mas">
  <a href="/zh/osx/brew-mas.html">brew mas</a> <a href="#brew-mas"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Mas 是一个简单的 Mac App Store 命令行界面.

#### 按应用名称搜索 Mac App Store 并返回匹配的标识符:
```shell
mas search {{应用名}}
```
#### 安装或更新以前购买的应用程序:
```shell
mas install {{应用名}} {{应用 ID}}
```
#### 显示所有已安装的应用程序及其应用 ID:
```shell
mas list
```
#### 列出等待更新的已安装应用:
```shell
mas outdated
```
#### 升级所有可升级的应用:
```shell
mas upgrade
```
#### 升级指定的应用:
```shell
mas upgrade {{应用 ID}}
```
{% endraw %}{% raw %}
<h2 id="brew">
  <a href="/zh/osx/brew.html">brew</a> <a href="#brew"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> macOS 上的软件包管理工具.

#### 搜索可用的命令行和软件安装包:
```shell
brew search {{软件名}}
```
#### 安装最新版本的命令行软件 （使用 `--devel` 可以指定安装更新的开发版）:
```shell
brew install {{软件名}}
```
#### 列出已（通过 brew) 安装的命令行工具:
```shell
brew list
```
#### 升级已安装的命令行软件（如果未给出命令行软件名称，则升级所有已安装的软件）:
```shell
brew upgrade {{软件名}}
```
#### 从 GitHub 上升级 brew 和软件库到最新:
```shell
brew update
```
#### 显示有关指定软件的信息（版本，安装路径，依赖关系等）:
```shell
brew info {{软件名}}
```
#### 检查本地 Homebrew 安装是否存在潜在问题，并给出一些解决建议:
```shell
brew doctor
```
#### 启动通过 brew 安装的服务，如 nginx,mysql 等。启动后还会自动随开机启动，直到你选择 stop 停止.（缺点是如果发生错误，它也会返回成功，而不是报错）:
```shell
brew services {{start|stop|restart}} {{软件名}}
```
{% endraw %}{% raw %}
<h2 id="brightness">
  <a href="/zh/osx/brightness.html">brightness</a> <a href="#brightness"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 获取或设置所有显示设备的亮度等级.

#### 显示当前亮度:
```shell
brightness -l
```
#### 设置亮度到 100%::
```shell
brightness {{1}}
```
#### 设置亮度到 50%::
```shell
brightness {{0.5}}
```
{% endraw %}{% raw %}
<h2 id="caffeinate">
  <a href="/zh/osx/caffeinate.html">caffeinate</a> <a href="#caffeinate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 防止 Mac 进入休眠模式.

#### 防止进入休眠模式 , 1 小时内 (3600 秒）:
```shell
caffeinate -u -t {{3600}}
```
#### 在指定命令执行完前，禁止进入休眠:
```shell
caffeinate -s {{命令}}
```
#### 在你按 Ctrl-C 之前禁止进入休眠模式:
```shell
caffeinate -i
```
{% endraw %}{% raw %}
<h2 id="cal">
  <a href="/zh/osx/cal.html">cal</a> <a href="#cal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 打印日历信息.

#### 打印本月日历:
```shell
cal
```
#### 显示上个月，当前月，下个月的日历:
```shell
cal -3
```
#### 显示指定月份的日历（月份为 1-12 月）:
```shell
cal -m {{月}}
```
#### 显示全年日历:
```shell
cal -y
```
#### 显示指定某年的日历（年份为 4 个数字）:
```shell
cal {{年}}
```
#### 显示特定年和月的日历:
```shell
cal {{月}} {{年}}
```
#### 显示指定年的复活节日期:
```shell
ncal -e {{年}}
```
{% endraw %}{% raw %}
<h2 id="carthage">
  <a href="/zh/osx/carthage.html">carthage</a> <a href="#carthage"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cocoa 应用程序的依赖性管理工具

#### 下载 Cartfile 中提到的所有依赖项的最新版本，并编译它们:
```shell
carthage update
```
#### 仅针对 IOS 平台，升级依赖文件 :
```shell
carthage update --platform ios
```
#### 仅更新依赖，但不编译它们 :
```shell
carthage update --no-build
```
#### 下载并重新生成依赖项的当前版本（不更新它们）:
```shell
carthage bootstrap
```
#### 重新编译特定依赖项 :
```shell
carthage build {{依赖包}}
```
{% endraw %}{% raw %}
<h2 id="chflags">
  <a href="/zh/osx/chflags.html">chflags</a> <a href="#chflags"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 更改文件或文件夹的标志.

#### 给文件设置 hidden（隐藏） 标签:
```shell
chflags {{hidden}} {{文件路径}}
```
#### 取消文件的 hidden 标签:
```shell
chflags {{hidden}} {{文件路径}}
```
#### 递归地给文件夹中每个文件设置 uchg 标志:
```shell
chflags -R {{uchg}} {{文件夹路径}}
```
#### 递归地撤销文件夹中每个文件设置的 uchg 标志:
```shell
chflags -R {{nouchg}} {{文件夹路径}}
```
{% endraw %}{% raw %}
<h2 id="codesign">
  <a href="/zh/osx/codesign.html">codesign</a> <a href="#codesign"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 为 macOS 的应用程序签名.

#### 用证书签名:
```shell
codesign -s "{{公司名称}}" {{路径 / 应用名.app}}
```
#### 验证应用程序的签名:
```shell
codesign -v {{路径 / 应用名.app}}
```
{% endraw %}{% raw %}
<h2 id="compgen">
  <a href="/zh/osx/compgen.html">compgen</a> <a href="#compgen"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用于在 bash 中自动完成的内置命令，按两次 tab 键即可调用该命令.

#### 显示所有可以执行的命令:
```shell
compgen -c
```
#### 列出所有别名:
```shell
compgen -a
```
#### 列出所有可以运行的函数:
```shell
compgen -A function
```
#### 列出所有 shell 的保留关键字:
```shell
compgen -k
```
#### 查看以 'ls' 开头的所有可用命令和别名:
```shell
compgen -ac {{ls}}
```
{% endraw %}{% raw %}
<h2 id="date">
  <a href="/zh/osx/date.html">date</a> <a href="#date"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 设置或显示系统日期.

#### 使用默认区域设置的格式显示当前日期 :
```shell
date +"%c"
```
#### 以 UTC 和 ISO 8601 格式显示当前日期:
```shell
date -u +"%Y-%m-%dT%H:%M:%SZ"
```
#### 将当前日期显示为 unix 时间戳（自 1970-01-01 00:00:00 以来的秒数）
```shell
date +%s
```
#### 使用默认格式显示特定日期（格式化指定 UNIX 时间戳）:
```shell
date -r 1473305798
```
{% endraw %}{% raw %}
<h2 id="dd">
  <a href="/zh/osx/dd.html">dd</a> <a href="#dd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 转换并复制文件.

#### 从 isohybrid 文件（如 archlinux-xxx.iso）制作可用于引导系统启动的 USB 驱动器.
```shell
dd if={{文件.iso}} of=/dev/{{usb 设备}}
```
#### 将驱动器克隆到具有 4MB 块的另一个驱动器并忽略错误:
```shell
dd if=/dev/{{源设备}} of=/dev/{{目标设备}} bs=4m conv=noerror
```
#### 使用内核随机驱动程序生成 100 个随机字节的文件:
```shell
dd if=/dev/urandom of={{目标驱动器，接收随机数据文件名}} bs=100 count=1
```
#### 对磁盘的写入性能进行基准测试:
```shell
dd if=/dev/zero of={{1GB 的文件名}} bs=1024 count=1000000
```
{% endraw %}{% raw %}
<h2 id="defaults">
  <a href="/zh/osx/defaults.html">defaults</a> <a href="#defaults"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 读取和写入 macOS 应用程序的用户配置.

#### 读取应用程序选项的系统默认值:
```shell
defaults read {{应用名}} {{选项}}
```
#### 读取应用程序选项的默认值:
```shell
defaults read -app {{应用名}} {{选项}}
```
#### 写入应用程序选项的默认值:
```shell
defaults write {{应用名}} {{选项}} {{- 类型}} {{值}}
```
#### 加速任务控制界面弹出动画 （时间设置为 0.1):
```shell
defaults write com.apple.Dock expose-animation-duration -float 0.1
```
#### 删除应用程序的所有默认值:
```shell
defaults delete {{应用名}}
```
{% endraw %}{% raw %}
<h2 id="diskutil">
  <a href="/zh/osx/diskutil.html">diskutil</a> <a href="#diskutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用于管理本地磁盘和卷的实用程序.

#### 列出所有当前可用的磁盘、分区和已装入的卷:
```shell
diskutil list
```
#### 修复卷的文件系统数据结构:
```shell
diskutil repairVolume {{目标卷文件}}
```
#### 卸载卷:
```shell
diskutil unmountDisk {{目标卷文件}}
```
#### 弹出 CD/DVD （先卸载）:
```shell
diskutil eject {{/dev/ 光驱文件名}}
```
{% endraw %}{% raw %}
<h2 id="ditto">
  <a href="/zh/osx/ditto.html">ditto</a> <a href="#ditto"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 复制文件和目录.

#### 用源目录的内容覆盖目标目录的内容:
```shell
ditto {{源文件路径}} {{目标文件路径}}
```
#### 为复制的每个文件打印一行到终端窗口:
```shell
ditto -V {{源文件路径}} {{目标文件路径}}
```
#### 复制给定的文件或目录，同时保留原始文件权限:
```shell
ditto -rsrc {{源文件路径}} {{目标文件路径}}
```
{% endraw %}{% raw %}
<h2 id="dmesg">
  <a href="/zh/osx/dmesg.html">dmesg</a> <a href="#dmesg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将内核消息写入标准输出.

#### 显示内核消息:
```shell
dmesg
```
#### 显示此系统上有多少可用的物理内存:
```shell
dmesg | grep -i memory
```
#### 一次显示一页内核消息:
```shell
dmesg | less
```
{% endraw %}{% raw %}
<h2 id="drutil">
  <a href="/zh/osx/drutil.html">drutil</a> <a href="#drutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 与 DVD 刻录机交互.

#### 从驱动器中弹出磁盘:
```shell
drutil eject
```
#### 将目录作为 iso9660 文件系统刻录到 DVD 上。完成后不验证和弹出:
```shell
drutil burn -noverify -eject -iso9660
```
{% endraw %}{% raw %}
<h2 id="du">
  <a href="/zh/osx/du.html">du</a> <a href="#du"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 磁盘使用率：估计和汇总文件和目录空间使用率.

#### 以给定单位（kb/mb/gb）列出目录和所有子目录的大小:
```shell
du -{{k|m|g}} {{目标文件夹}}
```
#### 以可读形式列出目录和任何子目录的大小（即自动为转换为选择的适当单位 kb|mb|gb）:
```shell
du -h {{目标文件夹}}
```
#### 以可读单位显示目录大小:
```shell
du -sh {{目标文件夹}}
```
#### 列出目录以及其中所有文件和目录的可读大小:
```shell
du -ah {{目标文件夹}}
```
#### 列出一个目录和任何子目录的可读大小，最深可达 n 级:
```shell
du -h -d {{N}} {{目标文件夹}}
```
#### 列出当前目录子目录中所有.jpg 文件的可读大小，并在末尾显示累计总数:
```shell
du -ch */*.jpg
```
{% endraw %}{% raw %}
<h2 id="duti">
  <a href="/zh/osx/duti.html">duti</a> <a href="#duti"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在 macOS 上为文档类型和网页设置默认打开的应用程序.

#### 将 Safari 设置为 HTML 文档的默认打开程序:
```shell
duti -s {{com.apple.Safari}} {{public.html}} all
```
#### 将 vlc 设置为扩展名为.m4v 的文件的默认查看器:
```shell
duti -s {{org.videolan.vlc}} {{m4v}} viewer
```
#### 将 Finder 设置为 ftp:// URL 访问的应用:
```shell
duti -s {{com.apple.Finder}} {{ftp}}
```
#### 显示有关给定扩展名的默认应用程序的信息:
```shell
duti -x {{ext}}
```
#### 显示给定的 UTI 对应默认的处理程序:
```shell
duti -d {{uti}}
```
#### 显示给定 UTI 对应所有的处理程序:
```shell
duti -l {{uti}}
```
{% endraw %}{% raw %}
<h2 id="eval">
  <a href="/zh/osx/eval.html">eval</a> <a href="#eval"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在当前 shell 中以单个命令的形式执行参数，并返回其结果.

#### 使用 'foo' 做为参数调用 `echo`:
```shell
eval "{{echo foo}}"
```
#### 在当前 shell 程序中设置变量:
```shell
eval "{{foo=bar}}"
```
{% endraw %}{% raw %}
<h2 id="export">
  <a href="/zh/osx/export.html">export</a> <a href="#export"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 命令为当前 shell 中的子进程进行环境变量设置.

#### 设置为新的环境变量:
```shell
export {{某变量名}}={{值}}
```
#### 删除环境变量:
```shell
export -n {{某变量名}}
```
#### 给 PATH 追加新的路径进去:
```shell
export PATH=$PATH:{{追加的 path 路径}}
```
{% endraw %}{% raw %}
<h2 id="fc">
  <a href="/zh/osx/fc.html">fc</a> <a href="#fc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 打开最近的命令并编辑它.

#### 在系统默认编辑器中打开:
```shell
fc
```
#### 指定要使用的的编辑器:
```shell
fc -e {{'emacs'}}
```
#### 从历史记录中列出最近的命令:
```shell
fc -l
```
{% endraw %}{% raw %}
<h2 id="feh">
  <a href="/zh/osx/feh.html">feh</a> <a href="#feh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 轻量级图像查看工具.

#### 查看本地图像或使用 URL:
```shell
feh {{图片路径}}
```
#### 递归查看图像:
```shell
feh --recursive {{图片路径}}
```
#### 使用无边框窗口查看图像:
```shell
feh --borderless {{图片路径}}
```
#### 在浏览完最后一个图像之后退出:
```shell
feh --cycle-once {{图片路径}}
```
#### 设置幻灯片放映周期延迟时间（秒）:
```shell
feh --slideshow-delay {{秒}} {{图片路径}}
```
#### 设置墙纸（居中、填充、最大化、缩放或平铺）:
```shell
feh --bg-{{center|fill|max|scale|tile}} {{图片路径}}
```
{% endraw %}{% raw %}
<h2 id="file">
  <a href="/zh/osx/file.html">file</a> <a href="#file"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 确定文件类型.

#### 提供指定文件类型的描述，对于没有文件扩展名的文件可以正常工作:
```shell
file {{文件名}}
```
#### 查看压缩文件并确定其中的文件类型:
```shell
file -z {{xxx.zip}}
```
#### 允许文件与特殊文件或设备文件一起使用:
```shell
file -s {{文件名}}
```
#### 不要在第一个文件类型匹配时停止；继续执行直到文件结束:
```shell
file -k {{文件名}}
```
#### 确定文件的 mime 编码类型:
```shell
file -I {{文件名}}
```
{% endraw %}{% raw %}
<h2 id="fsck">
  <a href="/zh/osx/fsck.html">fsck</a> <a href="#fsck"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 检查或修复文件系统的完整性，运行命令时应卸载文件系统.
> 它是一个包装器，包含 `fsck_hfs`, `fsck_apfs`, `fsck_msdos`, `fsck_exfat`, `fsck_udf` 作为可选.

#### 检查文件系统 /dev/sda，报告损坏的块:
```shell
fsck {{/dev/sda}}
```
#### 仅当文件系统 /dev/sda 是干净的时才检查它，报告任何损坏的块并以交互方式让用户选择修复每个块:
```shell
fsck -f {{/dev/sda}}
```
#### 仅当文件系统 /dev/sda 干净时才检查它，报告任何损坏的块并自动修复它们:
```shell
fsck -fy {{/dev/sda}}
```
#### 检查文件系统 /dev/sda, 报告是否已完全卸载:
```shell
fsck -q {{/dev/sda}}
```
{% endraw %}{% raw %}
<h2 id="getfileinfo">
  <a href="/zh/osx/getfileinfo.html">GetFileInfo</a> <a href="#getfileinfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 获取有关 HFS+ 目录中文件的信息.

#### 显示有关给定文件的信息:
```shell
GetFileInfo {{路径/文件名}}
```
#### 显示给定文件的创建日期和时间:
```shell
GetFileInfo -d {{路径/文件名}}
```
#### 显示给定文件的上次修改日期和时间:
```shell
GetFileInfo -m {{路径/文件名}}
```
#### 显示给定文件的创建者:
```shell
GetFileInfo -c {{路径/文件名}}
```
{% endraw %}{% raw %}
<h2 id="head">
  <a href="/zh/osx/head.html">head</a> <a href="#head"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 输出文件的开头部分.

#### 输出文件的前几行:
```shell
head -n {{行数}} {{文件名}}
```
#### 输出文件的前几个字节:
```shell
head -c {{字节数}} {{文件名}}
```
{% endraw %}{% raw %}
<h2 id="hexdump">
  <a href="/zh/osx/hexdump.html">hexdump</a> <a href="#hexdump"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一个 ASCII、十进制、十六进制、八进制转换查看工具.

#### 打印文件的十六进制表示形式:
```shell
hexdump {{文件}}
```
#### 以十六进制显示输入偏移量，并在最后两列中显示其 ASCII 表示形式:
```shell
hexdump -C {{文件}}
```
#### 显示文件的十六进制表示，但只解释输入的 N 个字节:
```shell
hexdump -C -n{{字节数}} {{文件}}
```
{% endraw %}{% raw %}
<h2 id="hostname">
  <a href="/zh/osx/hostname.html">hostname</a> <a href="#hostname"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示或设置系统的主机名.

#### 显示本机的主机名:
```shell
hostname
```
#### 设置本机主机名:
```shell
hostname {{新主机名}}
```
{% endraw %}{% raw %}
<h2 id="imgcat">
  <a href="/zh/osx/imgcat.html">imgcat</a> <a href="#imgcat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 直接在命令行上显示图像的实用程序.
> 需要兼容的终端软件，如 ITerm2.

#### 在命令行上显示图像:
```shell
imgcat {{文件名}}
```
{% endraw %}{% raw %}
<h2 id="launchctl">
  <a href="/zh/osx/launchctl.html">launchctl</a> <a href="#launchctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用于启动守护程序（系统范围的服务）和启动代理程序（每个用户程序）的命令行界面，该界面指向苹果的`launchd` 管理工具.
> `launchd`加载放置在适当位置的基于 XML 的`*.plist`文件，并根据其定义的计划运行相应的命令.

#### 每当用户登录时，自动将 plist 文件加载到 `launchd` :
```shell
launchctl load ~/Library/LaunchAgents/{{我的脚本}}.plist
```
#### 激活需要 root 权限才能运行和 / 或在任何用户登录时都应加载的脚本（注意路径中不能有`~`）:
```shell
sudo launchctl load /Library/LaunchAgents/{{root 脚本}}.plist
```
#### 激活一个系统范围的守护程序，以便在系统启动时加载（即使没有用户登录也会加载）:
```shell
sudo launchctl load /Library/LaunchDaemons/{{系统脚本}}.plist
```
#### 显示所有加载的代理 / 守护进程，如果它们指定的进程当前正在运行，则显示 pid，如果停止那么返回了它们上次运行的时间和退出代码:
```shell
launchctl list
```
#### 卸载当前加载的脚本，例如进行更改（注意：重新启动和 / 或登录后，plist 文件将自动加载到`launchd`）:
```shell
launchctl unload ~/Library/LaunchAgents/{{我的脚本}}.plist
```
#### 手动运行一个已知的（已加载的）脚本 / 守护进程，即使它不是正确的时间（注意：此命令使用脚本的标签，而不是文件名）:
```shell
launchctl start {{我的脚本}}
```
#### 手动终止与已知脚本 / 守护进程关联的进程（如果该进程正在运行）:
```shell
launchctl stop {{我的脚本}}
```
{% endraw %}{% raw %}
<h2 id="lldb">
  <a href="/zh/osx/lldb.html">lldb</a> <a href="#lldb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> LLVM 低级调试器.

#### 调试可执行文件:
```shell
lldb {{可执行的命令}}
```
#### 将 `lldb` 附加到具有给定 PID 的正在运行的进程:
```shell
lldb -p {{进程号 PID}}
```
#### 等待使用给定名称的进程启动，然后附加到该进程上:
```shell
lldb -w -n {{进程名}}
```
{% endraw %}{% raw %}
<h2 id="locate">
  <a href="/zh/osx/locate.html">locate</a> <a href="#locate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 快速查找文件名.

#### 在数据库中查找关键字。注意：数据库定期重新更新（通常每周或每天）:
```shell
locate {{关键字}}
```
#### 按文件名查找文件（不包含填充字符的模式被解释为 `*关键字*`）:
```shell
locate */{{文件名}}
```
#### 重新建立文件数据索引数据库。如果要查找最近添加的文件，则需要执行此操作:
```shell
sudo /usr/libexec/locate.updatedb
```
{% endraw %}{% raw %}
<h2 id="logger">
  <a href="/zh/osx/logger.html">logger</a> <a href="#logger"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 向系统日志增加记录 (/var/log/syslog).

#### 向系统日志增加记录:
```shell
logger {{消息内容}}
```
#### 从 stdin 获取输入并记录到系统日志 syslog:
```shell
echo {{记录内容}} | logger
```
#### 将输出发送到在给定端口上运行的远程系统日志服务器。默认端口为 514:
```shell
echo {{记录内容}} | logger -h {{服务器名}} -P {{端口}}
```
#### 对记录的每一行使用特定的标签。默认值是登录用户的名:
```shell
echo {{记录内容}} | logger -t {{标签}}
```
#### 以给定的错误等级记录消息。默认是 `user.notice`. 使用 `man logger` 查询所有可选等级:
```shell
echo {{记录内容}} | logger -p {{user.warning}}
```
{% endraw %}{% raw %}
<h2 id="look">
  <a href="/zh/osx/look.html">look</a> <a href="#look"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 查找已排序的文件行（注意，必须是已排序的文件）.

#### 它开始寻找一个给定的前缀:
```shell
look {{前缀}} {{文件}}
```
#### 查找行，忽略大小写:
```shell
look -f {{前缀}} {{文件}}
```
{% endraw %}{% raw %}
<h2 id="m">
  <a href="/zh/osx/m.html">m</a> <a href="#m"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> macOS 上的瑞士军刀.

#### 获取电池状态:
```shell
m battery status
```
#### 关闭蓝牙:
```shell
m bluetooth off
```
#### 列出可用于格式化的文件系统:
```shell
m disk filesystems
```
#### 启用 Dock（桌面程序坞） 的自动隐藏功能:
```shell
m dock autohide YES
```
#### 禁用防火墙:
```shell
m firewall disable
```
{% endraw %}{% raw %}
<h2 id="md5">
  <a href="/zh/osx/md5.html">md5</a> <a href="#md5"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 计算 MD5 加密和校验.

#### 计算一个文件的 MD5 校验值:
```shell
md5 {{文件名}}
```
#### 计算多个文件的 MD5 校验值:
```shell
md5 {{文件名 1}} {{文件名 2}}
```
#### 仅输出 MD5 校验值（无文件名）:
```shell
md5 -q {{文件名}}
```
#### 打印给定字符串的 MD5 校验值:
```shell
md5 -s {{字符串}}
```
{% endraw %}{% raw %}
<h2 id="mdfind">
  <a href="/zh/osx/mdfind.html">mdfind</a> <a href="#mdfind"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 列出与给定查询匹配的文件.

#### 按文件名查找文件:
```shell
mdfind -name {{文件}}
```
#### 按内容查找文件:
```shell
mdfind {{查找的字符串}}
```
#### 在给定目录中查找包含字符串的文件:
```shell
mdfind -onlyin {{目录}} {{字符串}}
```
{% endraw %}{% raw %}
<h2 id="mdutil">
  <a href="/zh/osx/mdutil.html">mdutil</a> <a href="#mdutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 管理 Spotlight（聚焦搜索） 用于搜索的索引数据.

#### 显示指定卷 ('/') 的索引状态:
```shell
mdutil -s {{/}}
```
#### 打开 / 关闭给定卷的 Spotlight 索引:
```shell
mdutil -i {{on|off}} {{指定卷文件夹}}
```
#### 清除索引数据并重新建立索引:
```shell
mdutil -E {{指定卷文件夹}}
```
{% endraw %}{% raw %}
<h2 id="mkfile">
  <a href="/zh/osx/mkfile.html">mkfile</a> <a href="#mkfile"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 创建一个或多个任意大小的空文件.

#### 创建一个 15 千字节的空文件:
```shell
mkfile -n {{15k}} {{文件名}}
```
#### 创建给定大小和单位的文件 (bytes, KB, MB, GB):
```shell
mkfile -n {{大小}}{{b|k|m|g}} {{文件名}}
```
#### 创建两个 4 兆字节的文件:
```shell
mkfile -n {{4m}} {{文件名 1}} {{文件名 2}}
```
{% endraw %}{% raw %}
<h2 id="n">
  <a href="/zh/osx/n.html">n</a> <a href="#n"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用于管理多个节点版本的工具.

#### 安装给定版本的节点。如果版本已经安装，它将被激活:
```shell
n {{版本}}
```
#### 显示已安装的版本并以交互方式激活其中一个版本:
```shell
n
```
#### 删除一个版本:
```shell
n rm {{版本}}
```
#### 使用给定版本执行文件:
```shell
n use {{版本}} {{文件.js}}
```
#### 输出指定版本的二进制:
```shell
n bin {{版本}}
```
{% endraw %}{% raw %}
<h2 id="netstat">
  <a href="/zh/osx/netstat.html">netstat</a> <a href="#netstat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示与网络相关的信息，如打开的连接、打开的套接字端口等.
> 更多信息: <https://www.unix.com/man-page/osx/1/netstat>.

#### 列出所有端口:
```shell
netstat -a
```
#### 列出所有被侦听端口:
```shell
netstat -l
```
#### 列出侦听的 TCP 端口:
```shell
netstat -t
```
#### 显示监听给定协议监听的 PID 和程序名:
```shell
netstat -p {{协议}}
```
#### 打印路由表:
```shell
netstat -nr
```
{% endraw %}{% raw %}
<h2 id="networksetup">
  <a href="/zh/osx/networksetup.html">networksetup</a> <a href="#networksetup"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 网络系统首选项配置工具.

#### 列出可用的网络服务源（以太网、Wi-Fi、蓝牙等）:
```shell
networksetup -listallnetworkservices
```
#### 显示特定网络设备的配置信息:
```shell
networksetup -getinfo "{{Wi-Fi}}"
```
#### 获取当前连接的 Wi-Fi 网络名称（Wi-Fi 设备通常为 en0 或 en1）:
```shell
networksetup -getairportnetwork {{en0}}
```
#### 连接到给定的 Wi-Fi 网络 Connect to a particular Wi-Fi network:
```shell
networksetup -setairportnetwork {{en0}} "{{无线网 SSID}}" {{密码}}
```
{% endraw %}{% raw %}
<h2 id="oathtool">
  <a href="/zh/osx/oathtool.html">oathtool</a> <a href="#oathtool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> OATH 一次性密码工具.

#### 生成 TOTP 令牌（行为类似于 Google Authenticator）:
```shell
oathtool --totp --base32 {{密码}}
```
#### 根据给定时间产生特定的 TOTP 令牌:
```shell
oathtool --totp --now {{2004-02-29 16:21:42}} --base32 {{密码}}
```
#### 验证 TOTP 令牌:
```shell
oathtool --totp --base32 {{密码}} {{令牌}}
```
{% endraw %}{% raw %}
<h2 id="open">
  <a href="/zh/osx/open.html">open</a> <a href="#open"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 打开文件、目录和应用程序.

#### 使用系统关联的应用程序打开文件:
```shell
open {{filename.extension}}
```
#### 运行图形化的 macOS 应用程序:
```shell
open -a {{应用程序名}}
```
#### 运行指定 包名 的图形化 macOS 应用程序（请参阅`OSascript`命令，查询如何获取应用程序的 包名）:
```shell
open -b {{com.domain.application 应用程序包名}}
```
#### 在"访达 (finder)"中打开当前文件夹:
```shell
open .
```
#### 打开"访达 (finder)", 并且给出指定文件:
```shell
open -R {{文件路径}}
```
#### 使用系统默认应用程序，打开当前目录中所有给定扩展名的文件:
```shell
open {{*.extension}}
```
{% endraw %}{% raw %}
<h2 id="opensnoop">
  <a href="/zh/osx/opensnoop.html">opensnoop</a> <a href="#opensnoop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 跟踪系统中打开的文件标识符.

#### 输出当前系统内被打开的所有文件:
```shell
sudo opensnoop
```
#### 跟踪给定进程名，打开的所有文件:
```shell
sudo opensnoop -n {{进程名}}
```
#### 跟踪给定 PID（进程号）, 打开的所有文件:
```shell
sudo opensnoop -p {{PID 进程号}}
```
#### 跟踪打开了指定文件的继承:
```shell
sudo opensnoop -f {{路径 / 文件}}
```
{% endraw %}{% raw %}
<h2 id="osascript">
  <a href="/zh/osx/osascript.html">osascript</a> <a href="#osascript"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在命令行中运行指定的 AppleScript 或 JavaScript 脚本程序.

#### 运行一个 AppleScript 命令:
```shell
osascript -e '{{say "你好世界"}}'
```
#### 运行多条 AppleScript 命令:
```shell
osascript -e '{{say "你好"}}' -e '{{say "世界"}}'
```
#### 运行一个已编译的脚本 (`*.scpt`), 包脚本 (`*.scptd`), 或明文的 (`*.applescript`) AppleScript 文件:
```shell
osascript {{目录 / 脚本文件.scpt}}
```
#### 获取应用程序的包名 （这个包名，可以用在命令 `open -b` 中）:
```shell
osascript -e 'id of app "{{应用程序名}}"'
```
#### 运行一个 JavaScript 命令:
```shell
osascript -l JavaScript -e '{{console.log("你好世界！");}}'
```
#### 运行 JavaScript 文件:
```shell
osascript -l JavaScript {{路径 / 文件名.js}}
```
{% endraw %}{% raw %}
<h2 id="pbcopy">
  <a href="/zh/osx/pbcopy.html">pbcopy</a> <a href="#pbcopy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将标准输出放入剪贴板（命令行里的 cmd + C).

#### 将文件的内容放入剪贴板:
```shell
pbcopy < {{文件}}
```
#### 将命令的执行结果放入剪贴板:
```shell
find . -type t -name "*.png" | pbcopy
```
{% endraw %}{% raw %}
<h2 id="pbpaste">
  <a href="/zh/osx/pbpaste.html">pbpaste</a> <a href="#pbpaste"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将剪贴板的内容发送到标准输出（命令行）.

#### 将剪贴板的内容写入文件:
```shell
pbpaste > {{文件}}
```
#### 将剪贴板的内容用作命令的输入:
```shell
pbpaste | grep foo
```
{% endraw %}{% raw %}
<h2 id="pdfgrep">
  <a href="/zh/osx/pdfgrep.html">pdfgrep</a> <a href="#pdfgrep"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在 PDF 文件中搜索文本.

#### 在 PDF 中查找与关键词匹配的行:
```shell
pdfgrep {{关键词}} {{文件.pdf}}
```
#### 包含每个匹配行的文件名和页码:
```shell
pdfgrep --with-filename --page-number {{关键词}} {{文件.pdf}}
```
#### 对以 "foo" 开头关键词搜索，返回前 3 个匹配项，不区分大小写:
```shell
pdfgrep --max-count {{3}} --ignore-case {{'^foo'}} {{文件.pdf}}
```
#### 在当前目录中扩展名为.pdf 的文件中递归查找关键词:
```shell
pdfgrep --recursive {{关键词}}
```
#### 在与当前目录中特定文件名 "*book.pdf" 匹配的文件上递归查找关键词:
```shell
pdfgrep --recursive --include {{'*book.pdf'}} {{关键词}}
```
{% endraw %}{% raw %}
<h2 id="ping">
  <a href="/zh/osx/ping.html">ping</a> <a href="#ping"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 向网络主机发送 ICMP 回显请求数据包.

#### Ping 指定的主机:
```shell
ping {{主机}}
```
#### 对主机执行指定定次数的 ping 操作:
```shell
ping -c {{次数}} {{主机}}
```
#### ping `主机` , 指定请求之间的间隔（以`秒`为单位）（默认为 1 秒）:
```shell
ping -i {{秒}} {{主机}}
```
#### Ping `主机`, 但不尝试查找地址的符号名:
```shell
ping -n {{主机}}
```
#### ping `主机` 并在收到数据包时响铃（如果您的终端支持）:
```shell
ping -a {{主机}}
```
#### ping `主机` 并打印接收数据包的时间（此选项是 Apple 的附加项）:
```shell
ping --apple-time {{主机}}
```
{% endraw %}{% raw %}
<h2 id="pmset">
  <a href="/zh/osx/pmset.html">pmset</a> <a href="#pmset"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 配置 macOS 电源管理设置，就像在系统首选项 > 节能程序中一样.
> 修改设置的命令必须以 `sudo` 开头.

#### 显示当前电源管理设置:
```shell
pmset -g
```
#### 显示当前电源和电池电量:
```shell
pmset -g batt
```
#### 当充电器通电时，将显示器设置为从不休眠:
```shell
sudo pmset -c displaysleep 0
```
#### 使用电池电源 15 分钟后将显示器设置为休眠:
```shell
sudo pmset -b displaysleep 15
```
#### 安排计算机在每个工作日上午 9 点自动唤醒:
```shell
sudo pmset repeat wake MTWRF 09:00:00
```
#### 还原为系统默认值:
```shell
sudo pmset -a displaysleep 10 disksleep 10 sleep 30 womp 1
```
{% endraw %}{% raw %}
<h2 id="pod">
  <a href="/zh/osx/pod.html">pod</a> <a href="#pod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Swift 和 Objective-C Cocoa 项目的依赖关系管理.

#### 为当前项目初始化包含默认内容的 podfile:
```shell
pod init
```
#### 下载并安装 pod 文件中定义的所有 pod（以前未安装）:
```shell
pod install
```
#### 列出所有可用的 pod:
```shell
pod list
```
#### 显示过时的 pod（当前安装的 pod）:
```shell
pod outdated
```
#### 将当前安装的所有 pod 更新到其最新版本:
```shell
pod update
```
#### 将特定（以前安装的）pod 更新为其最新版本:
```shell
pod update {{pod_名}}
```
#### 从 Xcode 项目中删除 CocoaPods:
```shell
pod deintegrate {{xcode_项目}}
```
{% endraw %}{% raw %}
<h2 id="popd">
  <a href="/zh/osx/popd.html">popd</a> <a href="#popd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 通过 pushd shell 内置程序删除目录堆栈中的目录.

#### 从堆栈中删除顶部目录，并用 `cd` 跳转到该目录:
```shell
popd
```
#### 删除第 n 个目录（从零开始，以用 `dirs` 打印的列表左侧开始）:
```shell
popd +N
```
#### 删除第 n 个目录（从零开始，以用 `dirs` 打印的列表右侧开始）:
```shell
popd -N
```
{% endraw %}{% raw %}
<h2 id="port">
  <a href="/zh/osx/port.html">port</a> <a href="#port"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> macOS 包管理器软件（类似 brew).

#### 搜索包:
```shell
port search {{搜索的包名}}
```
#### 安装软件包:
```shell
sudo port install {{报名}}
```
#### 列出已安装的软件包:
```shell
port installed
```
#### 更新 port 自身，并获取可用包的最新列表:
```shell
sudo port selfupdate
```
#### 升级过时的软件包:
```shell
sudo port upgrade outdated
```
#### 删除已安装的软件包的旧版本:
```shell
sudo port uninstall inactive
```
{% endraw %}{% raw %}
<h2 id="pushd">
  <a href="/zh/osx/pushd.html">pushd</a> <a href="#pushd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将目录放在堆栈上，以便以后访问.
> 另请参阅 `popd` 命令说明，以切换回原始目录.

#### 切换到目录并将其添加到堆栈上:
```shell
pushd {{directory}}
```
#### 切换堆栈上的第一个和第二个目录:
```shell
pushd
```
#### 通过使第 5 个元素成为堆栈的顶部来旋转堆栈:
```shell
pushd +4
```
{% endraw %}{% raw %}
<h2 id="pwgen">
  <a href="/zh/osx/pwgen.html">pwgen</a> <a href="#pwgen"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 生成可拼写发音的密码.

#### 生成指定长度的随机密码:
```shell
pwgen -y {{长度}}
```
#### 生成安全、难以记忆的密码:
```shell
pwgen -s {{长度}}
```
#### 生成至少包含一个大写字母的密码:
```shell
pwgen -c {{长度}}
```
{% endraw %}{% raw %}
<h2 id="qlmanage">
  <a href="/zh/osx/qlmanage.html">qlmanage</a> <a href="#qlmanage"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> QuickLook 服务器工具.

#### 快速显示一个或多个文件:
```shell
qlmanage -p {{文件名}} {{文件名 2}}
```
#### 计算生成当前目录中所有 jpeg 文件的缩略图，300px 宽 png 格式，并将它们放在一个指定目录中:
```shell
qlmanage {{*.jpg}} -t -s {{300}} {{指定目录}}
```
#### 重置快速查看:
```shell
qlmanage -r
```
{% endraw %}{% raw %}
<h2 id="reboot">
  <a href="/zh/osx/reboot.html">reboot</a> <a href="#reboot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 重启系统.

#### 立刻重启:
```shell
sudo reboot
```
#### 立即重启，而无需正常关机:
```shell
sudo reboot -q
```
{% endraw %}{% raw %}
<h2 id="route">
  <a href="/zh/osx/route.html">route</a> <a href="#route"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 手动操作路由表.
> 需要 root 权限.

#### 通过网关向目标添加路由:
```shell
sudo route add {{路由 ip 地址}} {{网关地址}}
```
#### 通过网关向 子网 / 24 添加路由:
```shell
sudo route add {{子网 ip}}/24 {{网关地址}}
```
#### 在测试模式下运行（不做任何操作，只打印）:
```shell
sudo route -t add {{路由 ip 地址}}/24 {{网关地址}}
```
#### 删除所有路由:
```shell
sudo route flush
```
#### 删除特定路由:
```shell
sudo route delete {{路由 ip 地址}}/24
```
#### 查找并显示目标的路由（主机名或 IP 地址）:
```shell
sudo route get {{目标}}
```
{% endraw %}{% raw %}
<h2 id="rubocop">
  <a href="/zh/osx/rubocop.html">rubocop</a> <a href="#rubocop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 格式化 Ruby 文件.

#### 检查当前目录中的所有文件（包括子目录）:
```shell
rubocop
```
#### 检查一个或多个指定文件或目录:
```shell
rubocop {{目录 / 文件名}} {{目录 /}}
```
#### 将输出写入指定文件:
```shell
rubocop --out {{目录 / 文件名}}
```
#### 查看规则列表（格式化规则）:
```shell
rubocop --show-cops
```
#### 排除格式规则:
```shell
rubocop --except {{规则 1}} {{规则 2}}
```
#### 只运行指定的规则:
```shell
rubocop --only {{规则 1}} {{规则 2}}
```
#### 自动更正文件（实验）:
```shell
rubocop --auto-correct
```
{% endraw %}{% raw %}
<h2 id="say">
  <a href="/zh/osx/say.html">say</a> <a href="#say"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将文本转换为语音.

#### 大声说出一个句子:
```shell
say "{{你好，世界！}}"
```
#### 播放文本文件内容音频:
```shell
say -f {{文件名.txt}}
```
#### 用自定义的语音和语音速率说出一个句子:
```shell
say -v {{语音库名}} -r {{每分钟多少词}} "{{你好，我可以说中文.}}"
```
#### 列出可用的语音库:
```shell
say --voice="?"
```
#### 创建文本的音频文件:
```shell
say -o {{文件名.aiff}} "{{你好，请将录音内容输出到文件.}}"
```
{% endraw %}{% raw %}
<h2 id="scutil">
  <a href="/zh/osx/scutil.html">scutil</a> <a href="#scutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 管理系统配置参数.
> 设置配置时必须是 root 权限.

#### 显示 DNS 配置:
```shell
scutil --dns
```
#### 显示代理配置:
```shell
scutil --proxy
```
#### 获取计算机名称:
```shell
scutil --get ComputerName
```
#### 设置计算机名称:
```shell
sudo scutil --set ComputerName {{我的计算机名}}
```
#### 获取主机名 ( HostName ):
```shell
scutil --get HostName
```
#### 设置主机名:
```shell
scutil --set HostName {{hostname}}
```
{% endraw %}{% raw %}
<h2 id="sed">
  <a href="/zh/osx/sed.html">sed</a> <a href="#sed"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 以可用脚本的来批量编辑文本.
> 更多信息： <https://ss64.com/osx/sed.html>.

#### 替换文件中第一个出现的字符串，并打印结果:
```shell
sed 's/{{查找内容}}/{{替换内容}}/' {{文件名}}
```
#### 替换文件中所有符合正则表达式的部分:
```shell
sed -E 's/{{正则表达式}}/{{替换内容}}/g' {{文件名}}
```
#### 替换文件中所有出现的字符串，覆盖文件（直接覆盖文件）:
```shell
sed --in-place='' 's/{{查找内容}}/{{替换内容}}/g' {{文件名}}
```
#### 仅替换与行模式（一种搜索条件）匹配的行内容:
```shell
sed '/{{行模式}}/s/{{查找内容}}/{{替换内容}}/' {{文件名}}
```
#### 只打印第 n 行到下一行之间的文本:
```shell
sed -n '{{行号}},/^$/p' {{文件名}}
```
#### 将多个查找替换表达式应用于文件:
```shell
sed -e 's/{{查找内容}}/{{替换内容}}/' -e 's/{{查找内容}}/{{替换内容}}/' {{文件名}}
```
#### 将分隔符 / 替换为查找或替换模式中没有用到的的任何其他字符，例如 # （用于查找或替换内容中使用了 / 的情况）:
```shell
sed 's#{{查找内容}}#{{替换内容}}#' {{文件名}}
```
{% endraw %}{% raw %}
<h2 id="shuf">
  <a href="/zh/osx/shuf.html">shuf</a> <a href="#shuf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 生成随机排列.

#### 随机化文件中的行顺序并输出结果:
```shell
shuf {{文件名}}
```
#### 只输出结果的前 5 条:
```shell
shuf -n {{5}} {{文件名}}
```
#### 将结果输出写入另一个文件:
```shell
shuf {{文件名}} -o {{输出_文件名}}
```
#### 生成范围 (1-10) 内的随机数:
```shell
shuf -i {{1-10}}
```
{% endraw %}{% raw %}
<h2 id="shutdown">
  <a href="/zh/osx/shutdown.html">shutdown</a> <a href="#shutdown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 关闭并重新启动系统.

#### 立即关机:
```shell
shutdown -h now
```
#### 立即休眠:
```shell
shutdown -s now
```
#### 立即重启:
```shell
shutdown -r now
```
#### 倒计时 5 分钟重启:
```shell
shutdown -r +{{5}}
```
{% endraw %}{% raw %}
<h2 id="sips">
  <a href="/zh/osx/sips.html">sips</a> <a href="#sips"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 苹果的处理文件脚本系统.
> 光栅 / 查询图像 和 颜色同步 ICC 配置文件.

#### S 指定一个输出目录，这样原始文件就不会被修改:
```shell
sips --out {{目标 / 文件夹 / 输出文件夹}}
```
#### 以指定的大小对图像重新采样，图像纵横比可能会更改:
```shell
sips -z {{1920}} {{300}} {{图片文件。扩展名}}
```
#### 对图像重新取样，使高度和宽度不大于指定的大小（注意大写 Z）:
```shell
sips -Z {{1920}} {{300}} {{图片文件。扩展名}}
```
#### 对目录中的所有图像重新取样，以适应 960px 的宽度（保持纵横比）:
```shell
sips --resampleWidth {{960}} {{目标 / 文件夹 / 所有图片文件}}
```
#### 将图像从 CMYK 转换为 RGB:
```shell
sips --matchTo '/System/Library/ColorSync/Profiles/Generic RGB Profile.icc' {{目标 / 文件夹 / 图片。扩展}} {{目标 / 文件夹 / 输出文件夹}}
```
#### 从图像中删除 ColorSync ICC 配置:
```shell
sips -d profile --deleteColorManagementProperties {{目标 / 文件夹 / 图片。扩展}}
```
{% endraw %}{% raw %}
<h2 id="softwareupdate">
  <a href="/zh/osx/softwareupdate.html">softwareupdate</a> <a href="#softwareupdate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 通过命令行更新 macOS 应用商店中应用程序的工具.

#### 列出所有可用的更新:
```shell
softwareupdate -l
```
#### 下载并安装所有更新:
```shell
softwareupdate -ia
```
#### 下载并安装所有推荐的更新:
```shell
softwareupdate -ir
```
#### 下载并安装特定的应用程序:
```shell
softwareupdate -i {{更新应用程序名}}
```
{% endraw %}{% raw %}
<h2 id="split">
  <a href="/zh/osx/split.html">split</a> <a href="#split"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 把一个文件拆分成几块.

#### 分割一个文件，每个分割部分有 10 行（除了最后一个）:
```shell
split -l {{10}} {{文件名}}
```
#### 用正则表达式拆分文件。匹配行将是下一个输出文件的第一行:
```shell
split -p {{cat|^[dh]og}} {{文件名}}
```
#### 拆分一个文件，每个拆分中有 512 个字节（除了最后一个文件，使用 512K 表示 Kb，512M 表示 Mb）:
```shell
split -b {{512}} {{文件名}}
```
{% endraw %}{% raw %}
<h2 id="ssh-add">
  <a href="/zh/osx/ssh-add.html">ssh-add</a> <a href="#ssh-add"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在 ssh 代理中管理加载的 ssh 密钥.
> 需要确保 ssh 代理已启动并正在运行以加载其中的密钥.

#### 将 `~/.ssh` 中的默认 ssh 密钥添加到 `ssh` 代理:
```shell
ssh-add
```
#### 向 ssh 代理添加指定密钥:
```shell
ssh-add {{目录 / 私钥文件}}
```
#### 列出当前加载的密钥的指纹:
```shell
ssh-add -l
```
#### 从 ssh 代理中删除密钥:
```shell
ssh-add -d {{目录 / 私钥文件}}
```
#### 从 ssh 代理中删除所有当前已有的密钥:
```shell
ssh-add -D
```
#### 向 ssh 代理和密钥链添加密钥:
```shell
ssh-add -K {{目录 / 私钥文件}}
```
{% endraw %}{% raw %}
<h2 id="sshuttle">
  <a href="/zh/osx/sshuttle.html">sshuttle</a> <a href="#sshuttle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 通过 ssh 连接传输流量的透明代理服务器.
> 不需要管理员或远程 ssh 服务器上的任何特殊设置.

#### 通过远程 ssh 服务器转发所有 IPv4 TCP 流量:
```shell
sshuttle --remote={{用户名}}@{{服务器名}} {{0.0.0.0/0}}
```
#### 转发所有 IPv4 TCP 和 DNS 流量:
```shell
sshuttle --dns --remote={{用户名}}@{{服务器名}} {{0.0.0.0/0}}
```
#### 使用 tproxy 方法转发所有 IPv4 和 IPv6 流量:
```shell
sudo sshuttle --method=tproxy --remote={{用户名}}@{{服务器名}} {{0.0.0.0/0}} {{::/0}} --exclude={{你本地 IP 地址}} --exclude={{SSH 服务器的 IP 地址}}
```
{% endraw %}{% raw %}
<h2 id="stat">
  <a href="/zh/osx/stat.html">stat</a> <a href="#stat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示文件状态.

#### 显示文件属性，如大小、权限、创建和访问日期等:
```shell
stat {{文件}}
```
#### 与上面相同，但更详细（更类似于 Linux 的 `stat`）:
```shell
stat -x {{文件}}
```
#### 只显示文件权限:
```shell
stat -f %Mp%Lp {{文件}}
```
#### 显示文件的所有者和所属组:
```shell
stat -f "%Su %Sg" {{文件}}
```
#### 以字节为单位显示文件的大小:
```shell
stat -f "%z %N" {{文件}}
```
{% endraw %}{% raw %}
<h2 id="sw_vers">
  <a href="/zh/osx/sw_vers.html">sw_vers</a> <a href="#sw_vers"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 打印 macOS 软件版本信息.

#### 打印 macOS 版本:
```shell
sw_vers -productVersion
```
#### 打印 macOS 构建版本:
```shell
sw_vers -buildVersion
```
{% endraw %}{% raw %}
<h2 id="sysctl">
  <a href="/zh/osx/sysctl.html">sysctl</a> <a href="#sysctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 访问内核状态信息.

#### 显示所有可用变量及其值:
```shell
sysctl -a
```
#### 显示 Apple 型号标识符:
```shell
sysctl -n hw.model
```
#### 显示 CPU 模型:
```shell
sysctl -n machdep.cpu.brand_string
```
#### 显示可用的 CPU 功能 (MMX, SSE, SSE2, SSE3, AES, 等）:
```shell
sysctl -n machdep.cpu.features
```
#### 设置一个可更改的内核状态变量:
```shell
sysctl -w {{部分。可修改的变量}}={{值}}
```
{% endraw %}{% raw %}
<h2 id="system_profiler">
  <a href="/zh/osx/system_profiler.html">system_profiler</a> <a href="#system_profiler"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 报告系统硬件和软件配置.

#### 显示可由 System Profiler.app 打开的完整系统资源报告:
```shell
system_profiler -xml > MyReport.spx
```
#### 显示硬件概述（型号、CPU、内存、串行等）:
```shell
system_profiler SPHardwareDataType
```
#### 打印系统序列号:
```shell
system_profiler SPHardwareDataType|grep "Serial Number (system)" |awk '{print $4}'
```
{% endraw %}{% raw %}
<h2 id="systemsetup">
  <a href="/zh/osx/systemsetup.html">systemsetup</a> <a href="#systemsetup"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 配置系统首选项计算机设置.

#### 启用远程登录 (SSH):
```shell
systemsetup -setremotelogin on
```
#### 指定时区、NTP 服务器并启用网络时间:
```shell
systemsetup -settimezone {{美国 / 太平洋}} -setnetworktimeserver {{us.pool.ntp.org}} -setusingnetworktime on
```
#### 使机器从不休眠，并在电源故障或内核死机时自动重新启动:
```shell
systemsetup -setsleep off -setrestartpowerfailure on -setrestartfreeze on
```
#### disks 选择启动:
```shell
systemsetup -liststartupdisks
```
#### 指定新的启动盘:
```shell
systemsetup -setstartupdisk {{路径}}
```
{% endraw %}{% raw %}
<h2 id="textutil">
  <a href="/zh/osx/textutil.html">textutil</a> <a href="#textutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用于操作各种格式的文本文件.

#### 显示有关 `foo.rtf` 的信息:
```shell
textutil -info {{foo.rtf}}
```
#### 将 `foo.rtf` 转换为 `foo.html`:
```shell
textutil -convert {{html}} {{foo.rtf}}
```
#### 将带格式的 rtf 文本转换为普通 txt 文本:
```shell
textutil {{foo.rtf}} -convert {{txt}}
```
#### 将 `foo.txt` 转换为 `foo.rtf`, 字体使用 Times 字号 10:
```shell
textutil -convert {{rtf}} -font {{Times}} -fontsize {{10}} {{foo.txt}}
```
#### 加载当前目录中的所有 RTF 文件，连接其内容，并将结果作为 `index.html` 写入，HTML 标题设置为"多个文件":
```shell
textutil -cat {{html}} -title "多个文件" -output {{index.html}} *.rtf
```
{% endraw %}{% raw %}
<h2 id="top">
  <a href="/zh/osx/top.html">top</a> <a href="#top"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示运行进程的动态实时信息.

#### 执行 top 命令，界面中提供所有选项:
```shell
top
```
#### 按内部内存大小排序进程（默认顺序 - 进程 ID):
```shell
top -o mem
```
#### 首先按 CPU 启动顺序排序进程，然后按运行时间排序:
```shell
top -o cpu -O time
```
#### 只显示给定用户拥有的进程:
```shell
top -user {{用户名}}
```
#### 获取有关交互式命令的帮助（我测试并没看到这个功能）:
```shell
?
```
{% endraw %}{% raw %}
<h2 id="trap">
  <a href="/zh/osx/trap.html">trap</a> <a href="#trap"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在进程或操作系统接收到信号后自动执行命令.
> 可用于对用户中断或其他操作执行清理.

#### 列出设置 trap 的可用信号:
```shell
trap -l
```
#### 列出当前 shell 程序的活动 trap 程序:
```shell
trap -p
```
#### 设置 trap 以在检测到一个或多个信号时执行命令:
```shell
trap 'echo "检测到信号 {{SIGHUP}}"' {{SIGHUP}}
```
#### 移除活动 trap:
```shell
trap - {{SIGHUP}} {{SIGINT}}
```
{% endraw %}{% raw %}
<h2 id="tree">
  <a href="/zh/osx/tree.html">tree</a> <a href="#tree"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 以树的形式显示当前目录的内容.

#### 显示深度达到 “级数” 级的文件和目录（其中 1 表示当前目录）:
```shell
tree -L {{级数}}
```
#### 只显示目录:
```shell
tree -d
```
#### 同时显示隐藏文件:
```shell
tree -a
```
#### 打印没有缩进行的树，显示完整路径（使用`-N`不转义空格和特殊字符）:
```shell
tree -i -f
```
#### 以可读格式打印每个文件节点的大小，目录显示其累积大小（类似在`du`命令中所示）:
```shell
tree -s -h --du
```
#### 使用通配符（glob）模式在树层次结构中查找文件，并删除不包含匹配文件的目录:
```shell
tree -P '{{*.txt}}' --prune
```
#### 在树层次结构中查找目录，删除不属于所需目录的目录:
```shell
tree -P {{文件夹名}} --matchdirs --prune
```
{% endraw %}{% raw %}
<h2 id="uname">
  <a href="/zh/osx/uname.html">uname</a> <a href="#uname"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 打印当前计算机及其上运行的操作系统的详细信息.
> 注意：有关操作系统的其他信息，请尝试使用 `sw-vers` 命令.

#### 打印硬件相关：架构信息和处理器:
```shell
uname -mp
```
#### 打印软件相关信息：操作系统、版本号和版本:
```shell
uname -srv
```
#### 打印系统的节点名称（主机名）:
```shell
uname -n
```
#### 打印所有可用的系统信息（硬件、软件、节点名）:
```shell
uname -a
```
{% endraw %}{% raw %}
<h2 id="w">
  <a href="/zh/osx/w.html">w</a> <a href="#w"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示谁登录以及他们在做什么.
> 打印用户登录、tty、远程主机、登录时间、空闲时间、当前进程.

#### 显示登录用户信息:
```shell
w
```
#### 显示没有标题的登录用户信息:
```shell
w -h
```
#### 显示有关已登录用户的信息，按其空闲时间排序:
```shell
w -i
```
{% endraw %}{% raw %}
<h2 id="wacaw">
  <a href="/zh/osx/wacaw.html">wacaw</a> <a href="#wacaw"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一个用于 macOS 的小命令行工具，允许您从连接的摄像头捕获静止图片和视频

#### 从网络摄像机拍照:
```shell
wacaw {{文件名}}
```
#### 录制视频:
```shell
wacaw --video {{文件名}} -D {{录制多少秒}}
```
#### 用自定义分辨率拍照:
```shell
wacaw -x {{宽}} -y {{高}} {{文件名}}
```
#### 将刚拍摄的图像复制到剪贴板:
```shell
wacaw --to-clipboard
```
#### 可用设备列表:
```shell
wacaw -L
```
{% endraw %}{% raw %}
<h2 id="whereis">
  <a href="/zh/osx/whereis.html">whereis</a> <a href="#whereis"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 找到命令的二进制，源文件和手册文件.

#### 找到 `ssh` 命令的二进制、源文件和手册页:
```shell
whereis {{ssh}}
```
#### 查找 `ls` 命令的二进制和手册页:
```shell
whereis -bm {{ls}}
```
#### 找到 `gc` 的源文件和 `git` 的手册页:
```shell
whereis -s {{gcc}} -m {{git}}
```
#### 仅在 /usr/bin/ 目录中查找 `gcc` 的二进制文件:
```shell
whereis -b -B {{/usr/bin/}} -f {{gcc}}
```
{% endraw %}{% raw %}
<h2 id="wifi-password">
  <a href="/zh/osx/wifi-password.html">wifi-password</a> <a href="#wifi-password"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 获取 wifi 的密码.
> 更多信息: <https://github.com/rauchg/wifi-password>.

#### 获取你当前登录的 wifi 的密码:
```shell
wifi-password
```
#### 获取特定 SSID 的 wifi 的密码:
```shell
wifi-password {{ssid}}
```
#### 仅输出密码:
```shell
wifi-password -q
```
{% endraw %}{% raw %}
<h2 id="xattr">
  <a href="/zh/osx/xattr.html">xattr</a> <a href="#xattr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用于扩展文件系统属性的实用程序.

#### 列出 键：值 列表，显示指定文件的值扩展属性:
```shell
xattr -l {{文件名}}
```
#### 为给定文件写入属性:
```shell
xattr -w {{属性键名}} {{属性值}} {{文件名}}
```
#### 从给定文件中删除属性:
```shell
xattr -d {{com.apple.quarantine}} {{文件名}}
```
#### 从给定文件中删除所有扩展属性:
```shell
xattr -c {{文件名}}
```
#### 递归删除给定目录中文件的属性:
```shell
xattr -rd {{属性键名}} {{目录}}
```
{% endraw %}{% raw %}
<h2 id="xcodebuild">
  <a href="/zh/osx/xcodebuild.html">xcodebuild</a> <a href="#xcodebuild"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 构建 Xcode 项目.

#### 构建工作区:
```shell
xcodebuild -workspace {{工作区名.工作区}} -scheme {{主题名}} -configuration {{配置名}} clean build SYMROOT={{SYMROOT_路径}}
```
#### 构建项目:
```shell
xcodebuild -target {{目标名}} -configuration {{配置名}} clean build SYMROOT={{SYMROOT_路径}}
```
#### 显示 SDK:
```shell
xcodebuild -showsdks
```
{% endraw %}{% raw %}
<h2 id="xctool">
  <a href="/zh/osx/xctool.html">xctool</a> <a href="#xctool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用于构建 Xcode 项目的工具.

#### 在没有任何工作区的情况下生成单个项目:
```shell
xctool -project {{你的项目.名称}} -scheme {{方案}} build
```
#### 构建属于工作区的项目:
```shell
xctool -workspace {{你的工作区.名字}} -scheme {{方案}} build
```
#### 清理、构建和执行所有测试:
```shell
xctool -workspace {{你的工作区.名字}} -scheme {{方案}} clean build test
```
{% endraw %}{% raw %}
<h2 id="xed">
  <a href="/zh/osx/xed.html">xed</a> <a href="#xed"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用 Xcode 打开要编辑的文件.

#### 用 Xcode 打开文件 :
```shell
xed {{文件名}}
```
#### 在 Xcode 中打开文件，如果不存在则创建:
```shell
xed -c {{文件名}}
```
#### 在 Xcode 中打开一个文件并跳转到第 75 行:
```shell
xed -l 75 {{文件名}}
```
{% endraw %}{% raw %}
<h2 id="xsltproc">
  <a href="/zh/osx/xsltproc.html">xsltproc</a> <a href="#xsltproc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用 XSLT 转换 XML 以生成输出（通常是 HTML 或 XML ）.

#### 使用特定的 XSLT 样式表转换 XML 文件:
```shell
xsltproc --output {{输出.html}} {{样式表.xslt}} {{xml 文件.xml}}
```
#### 将值传递给样式表中的参数:
```shell
xsltproc --output {{输出.html}} --stringparam {{键名}} {{值}} {{样式表.xslt}} {{xml 文件.xml}}
```
{% endraw %}{% raw %}
<h2 id="yank">
  <a href="/zh/osx/yank.html">yank</a> <a href="#yank"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 从 stdin 读取输入并显示一个选择界面，该界面允许选择一个字段并将其复制到剪贴板.

#### 使用默认分隔符 (\f, \n, \r, \s, \t):
```shell
{{sudo dmesg}} | yank
```
#### 输入单行:
```shell
{{sudo dmesg}} | yank -l
```
#### 使用特定分 `=` 隔符输入:
```shell
{{echo hello=world}} | yank -d {{=}}
```
#### 只有与特定正则表达式匹配的内容才输入:
```shell
{{ps ux}} | yank -g "{{[0-9]+}}"
```
{% endraw %}