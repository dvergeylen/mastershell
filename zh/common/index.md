---
layout: default
title: "common"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#7z">7z</a>
* <a href="#7za">7za</a>
* <a href="#7zr">7zr</a>
* <a href="#adguardhome">AdGuardHome</a>
* <a href="#aapt">aapt</a>
* <a href="#ab">ab</a>
* <a href="#abduco">abduco</a>
* <a href="#ack">ack</a>
* <a href="#act">act</a>
* <a href="#adb">adb</a>
* <a href="#adb-install">adb install</a>
* <a href="#adb-reverse">adb reverse</a>
* <a href="#adb-shell">adb shell</a>
* <a href="#ag">ag</a>
* <a href="#airpaste">airpaste</a>
* <a href="#alacritty">alacritty</a>
* <a href="#alias">alias</a>
* <a href="#androguard">androguard</a>
* <a href="#ansible">ansible</a>
* <a href="#ansible-galaxy">ansible-galaxy</a>
* <a href="#ansible-playbook">ansible-playbook</a>
* <a href="#ansiweather">ansiweather</a>
* <a href="#apg">apg</a>
* <a href="#apktool">apktool</a>
* <a href="#apm">apm</a>
* <a href="#apropos">apropos</a>
* <a href="#ar">ar</a>
* <a href="#arch">arch</a>
* <a href="#aria2">aria2</a>
* <a href="#aria2c">aria2c</a>
* <a href="#arp">arp</a>
* <a href="#asar">asar</a>
* <a href="#asciinema">asciinema</a>
* <a href="#asdf">asdf</a>
* <a href="#atom">atom</a>
* <a href="#autoflake">autoflake</a>
* <a href="#autojump">autojump</a>
* <a href="#axel">axel</a>
* <a href="#babel">babel</a>
* <a href="#banner">banner</a>
* <a href="#base32">base32</a>
* <a href="#base64">base64</a>
* <a href="#basename">basename</a>
* <a href="#bash">bash</a>
* <a href="#bashmarks">bashmarks</a>
* <a href="#bat">bat</a>
* <a href="#behat">behat</a>
* <a href="#bg">bg</a>
* <a href="#bmaptool">bmaptool</a>
* <a href="#bower">bower</a>
* <a href="#browser-sync">browser-sync</a>
* <a href="#btm">btm</a>
* <a href="#buku">buku</a>
* <a href="#carbon-now">carbon-now</a>
* <a href="#case">case</a>
* <a href="#cat">cat</a>
* <a href="#cd">cd</a>
* <a href="#clear">clear</a>
* <a href="#code">code</a>
* <a href="#command">command</a>
* <a href="#cp">cp</a>
* <a href="#curl">curl</a>
* <a href="#echo">echo</a>
* <a href="#etcd">etcd</a>
* <a href="#exit">exit</a>
* <a href="#gh-gist">gh gist</a>
* <a href="#gh-repo">gh repo</a>
* <a href="#gpg">gpg</a>
* <a href="#gpg-zip">gpg-zip</a>
* <a href="#gpg2">gpg2</a>
* <a href="#gpgv">gpgv</a>
* <a href="#gunicorn">gunicorn</a>
* <a href="#heroku">heroku</a>
* <a href="#hexo">hexo</a>
* <a href="#jar">jar</a>
* <a href="#jarsigner">jarsigner</a>
* <a href="#java">java</a>
* <a href="#javac">javac</a>
* <a href="#javadoc">javadoc</a>
* <a href="#jps">jps</a>
* <a href="#make">make</a>
* <a href="#matlab">matlab</a>
* <a href="#md5sum">md5sum</a>
* <a href="#mongod">mongod</a>
* <a href="#mpv">mpv</a>
* <a href="#mvn">mvn</a>
* <a href="#ninja">ninja</a>
* <a href="#nmap">nmap</a>
* <a href="#node">node</a>
* <a href="#rsync">rsync</a>
* <a href="#runit">runit</a>
* <a href="#runsv">runsv</a>
* <a href="#runsvchdir">runsvchdir</a>
* <a href="#runsvdir">runsvdir</a>
* <a href="#rustfmt">rustfmt</a>
* <a href="#shasum">shasum</a>
* <a href="#stty">stty</a>
* <a href="#sv">sv</a>
* <a href="#tldr">tldr</a>
* <a href="#uname">uname</a>
* <a href="#units">units</a>
* <a href="#view">view</a>
* <a href="#vim">vim</a>
* <a href="#virtualenv">virtualenv</a>
* <a href="#vlc">vlc</a>
* <a href="#vue-cli">vue-cli</a>
* <a href="#w">w</a>
* <a href="#wget">wget</a>
* <a href="#where">where</a>
* <a href="#which">which</a>
* <a href="#write">write</a>
* <a href="#yarn">yarn</a>
* <a href="#yarn-why">yarn-why</a>
* <a href="#z">z</a>
* <a href="#zsh">zsh</a>
* <a href="#zstd">zstd</a>

{% raw %}
<h2 id="7z">
  <a href="/zh/common/7z.html">7z</a> <a href="#7z"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一个高压缩率的文件归档器.

#### 归档一个文件或文件夹:
```shell
7z a {{归档文件.7z}} {{文件路径}}
```
#### 对已存在的归档文件加密（包括头部）:
```shell
7z a {{加密文件.7z}} -p{{密码}} -mhe=on {{归档文件.7z}}
```
#### 提取一个已存在的 7z 文件，并保持原来的目录结构:
```shell
7z x {{归档文件.7z}}
```
#### 提取一个归档文件到自定义的输出目录:
```shell
7z x {{归档文件.7z}} -o{{输出路径}}
```
#### 使用指定的类型来归档文件:
```shell
7z a -t {{zip|gzip|bzip2|tar|...}} {{归档文件.7z}} {{文件路径}}
```
#### 列出可用的归档文件类型:
```shell
7z i
```
#### 列出一个归档文件的内容:
```shell
7z l {{归档文件.7z}}
```
{% endraw %}{% raw %}
<h2 id="7za">
  <a href="/zh/common/7za.html">7za</a> <a href="#7za"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一个高压缩率的文件归档器.
> `7z`的独立版本，支持的文档类型较少.

#### 归档一个文件或文件夹:
```shell
7za a {{归档文件.7z}} {{文件路径}}
```
#### 提取一个已存在的 7z 文件，并保持原来的目录结构:
```shell
7za x {{归档文件文件}}
```
#### 使用指定的类型来归档文件:
```shell
7za a -t{{zip|gzip|bzip2|tar|...}} {{归档文件}} {{文件路径}}
```
#### 列出可用的归档文件类型:
```shell
7za i
```
#### 列出一个归档文件的内容:
```shell
7za l {{归档文件}}
```
{% endraw %}{% raw %}
<h2 id="7zr">
  <a href="/zh/common/7zr.html">7zr</a> <a href="#7zr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一个高压缩率的文件归档器.
> `7z`的独立版本，只支持 .7z 文件.

#### 归档一个文件或文件夹:
```shell
7zr a {{归档文件.7z}} {{文件路径}}
```
#### 提取一个已存在的 7z 文件，并保持原来的目录结构:
```shell
7zr x {{归档文件.7z}}
```
#### 列出一个归档文件的内容:
```shell
7zr l {{归档文件.7z}}
```
{% endraw %}{% raw %}
<h2 id="aapt">
  <a href="/zh/common/aapt.html">aapt</a> <a href="#aapt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 安卓资源包工具（Android Asset Packaging Tools）.
> 该工具可以查看，创建， 更新资源压缩包(zip, jar, apk)。

#### 列出资源压缩包里的内容:
```shell
aapt list {{路径/到/应用.apk}}
```
#### 查看APK包内指定的内容 (版本, 权限许可等):
```shell
aapt dump badging {{路径/到/应用.apk}}
```
#### 打包生成资源压缩包:
```shell
aapt package -F {{路径/到/应用.apk}} {{路径/到/目录}}
```
{% endraw %}{% raw %}
<h2 id="ab">
  <a href="/zh/common/ab.html">ab</a> <a href="#ab"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Apache 基准测试工具.最简单的压力测试工具.

#### 向目标 URL 执行 100 次 HTTP GET 请求:
```shell
ab -n {{100}} {{url}}
```
#### 使用 10 个并发请求，同时向目标 URL 执行 100 次 HTTP GET 请求:
```shell
ab -n {{100}} -c {{10}} {{url}}
```
#### 使用 keep alive:
```shell
ab -k {{url}}
```
#### 为基准测试设置最大的测试时间（单位：秒）:
```shell
ab -t {{60}} {{url}}
```
{% endraw %}{% raw %}
<h2 id="abduco">
  <a href="/zh/common/abduco.html">abduco</a> <a href="#abduco"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 终端会话管理器.

#### 列出会话:
```shell
abduco
```
#### 附加到一个会话，如果不存在则新建它:
```shell
abduco -A {{会话名}} {{终端}}
```
#### 使用`dvtm`附加到一个会话，如果不存在则新建它:
```shell
abduco -A {{会话名}}
```
#### 从一个会话中分离:
```shell
Ctrl + \
```
#### 以只读模式附加到一个会话:
```shell
abduco -Ar {{会话名}}
```
{% endraw %}{% raw %}
<h2 id="ack">
  <a href="/zh/common/ack.html">ack</a> <a href="#ack"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一个类似 grep 的搜索工具，为程序员优化.

#### 寻找包含"小明"的文件:
```shell
ack {{小明}}
```
#### 在给定文件类型中寻找包含"小明"的文件:
```shell
ack --ruby {{小明}}
```
#### 计算匹配到"小明"的总次数:
```shell
ack -ch {{小明}}
```
#### 列出内容包含"小明"的文件的文件名，并显示在每个文件中匹配的次数:
```shell
ack -cl {{小明}}
```
{% endraw %}{% raw %}
<h2 id="act">
  <a href="/zh/common/act.html">act</a> <a href="#act"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 使用Docker本地运行GitHub Actions
> 更多信息: <https://github.com/nektos/act>.

#### 列出可用的actions清单:
```shell
act -l
```
#### 运行默认event:
```shell
act
```
#### 运行指定event:
```shell
act {{事件类型}}
```
#### 运行指定action:
```shell
act -a {{action_id}}
```
#### 非实际运行actions (也就是dry-run模式):
```shell
act -n
```
#### 展示详细记录:
```shell
act -v
```
{% endraw %}{% raw %}
<h2 id="adb-install">
  <a href="/zh/common/adb-install.html">adb install</a> <a href="#adb-install"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 安卓调试桥-Install: 将应用安装包推送到Android模拟器或已连接的安卓设备.
> 更多信息: <https://developer.android.com/studio/command-line/adb>.

#### 向模拟器/设备推送安卓app:
```shell
adb install {{路径/到/应用.apk}}
```
#### 重装app, 保持原有数据:
```shell
adb install -r {{路径/到/应用.apk}}
```
#### 授予app manifest中列举的所有权限许可:
```shell
adb install -g {{路径/到/应用.apk}}
```
#### 快速部署模式，仅更新APK更改过的部分:
```shell
adb install --fastdeploy {{路径/到/应用.apk}}
```
{% endraw %}{% raw %}
<h2 id="adb-reverse">
  <a href="/zh/common/adb-reverse.html">adb reverse</a> <a href="#adb-reverse"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 安卓调试桥-反射: 反向映射安卓模拟器实例或者已连接的实体设备的套接字连接.
> 更多信息: <https://developer.android.com/studio/command-line/adb>.

#### 列出所有来自模拟器和设备的映射连接
```shell
adb reverse —list
```
#### 将TCP端口从安卓模拟器或设备中映射到localhost:
```shell
adb reverse tcp:{{远程端口}} tcp:{{本地端口}}
```
#### 从安卓模拟器或设备移除一个反向socket连接:
```shell
adb reverse --remove tcp:{{远程端口}}
```
#### 从安卓模拟器或设备移除所有反向socket连接:
```shell
adb reverse --remove-all
```
{% endraw %}{% raw %}
<h2 id="adb-shell">
  <a href="/zh/common/adb-shell.html">adb shell</a> <a href="#adb-shell"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 安卓调试桥-Shell: 运行安卓模拟器或者连接设备上的远程终端命令。
> 更多信息: <https://developer.android.com/studio/command-line/adb>.

#### 启动模拟器/设备上的远程终端:
```shell
adb shell
```
#### 获取模拟器/设备全部属性:
```shell
adb shell getprop
```
#### 重置所有运行时权限为它们的默认值:
```shell
adb shell pm reset-permissions
```
#### 撤销一个应用的危险权限:
```shell
adb shell pm revoke {{包名}} {{权限}}
```
#### 触发一个键盘敲击事件:
```shell
adb shell input keyevent {{键位码}}
```
#### 清除模拟器/设备上的数据:
```shell
adb shell pm clear {{包名}}
```
#### 启动模拟器/设备上的一个行为:
```shell
adb shell am start -n {{包名}}/{{活动名}}
```
#### 启动模拟器/设备上的首页活动:
```shell
adb shell am start -W -c android.intent.category.HOME -a android.intent.action.MAIN
```
{% endraw %}{% raw %}
<h2 id="adb">
  <a href="/zh/common/adb.html">adb</a> <a href="#adb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 安卓调试桥：与 Android 模拟器或已连接的 Android 设备通信.
> 更多信息: <https://developer.android.com/studio/command-line/adb>.

#### 检查 adb server 进程的是否在运行，并开启它:
```shell
adb start-server
```
#### 终止 adb server 进程:
```shell
adb kill-server
```
#### 在目标模拟器 / 设备实例上开启一个远程 shell:
```shell
adb shell
```
#### 将 Android 应用程序推送到模拟器 / 设备 :
```shell
adb install -r {{路径/到/应用.apk}}
```
#### 从目标设备上拷贝一个文件 / 目录到本地:
```shell
adb pull {{路径/到/设备的文件或目录}} {{路径/到/本地上的目录}}
```
#### 从本地拷贝一个文件 / 目录到目标设备:
```shell
adb push {{路径/到/本地文件或目录}} {{路径/到/设备上的目录}}
```
#### 列出已连接的设备:
```shell
adb devices
```
{% endraw %}{% raw %}
<h2 id="adguardhome">
  <a href="/zh/common/adguardhome.html">AdGuardHome</a> <a href="#adguardhome"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一款全网广告拦截与反跟踪软件.
> 更多信息: <https://github.com/AdguardTeam/AdGuardHome>.

#### 运行 AdGuard Home:
```shell
AdGuardHome
```
#### 使用给定的配置文件运行 AdGuard Home:
```shell
AdGuardHome --config {{给定的/配置文件.yaml}}
```
#### 设置存储数据的工作目录:
```shell
AdGuardHome --work-dir {{工作目录/路径}}
```
#### 安装或卸载 AdGuard Home 的服务:
```shell
AdGuardHome --service {{install|uninstall}}
```
#### 启动 AdGuard Home 的服务:
```shell
AdGuardHome --service start
```
#### 刷新 AdGuard Home 服务的设置项:
```shell
AdGuardHome --service reload
```
#### 停止或重启 AdGuard Home 的服务:
```shell
AdGuardHome --service {{stop|restart}}
```
{% endraw %}{% raw %}
<h2 id="ag">
  <a href="/zh/common/ag.html">ag</a> <a href="#ag"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The Silver Searcher. 类似 ack, 但是更快.
> 更多信息: <https://github.com/ggreer/the_silver_searcher>.

#### 寻找内容包含"小明"的文件，并列出所在的行数:
```shell
ag {{小明}}
```
#### 在指定目录中寻找内容包含"foo"的文件:
```shell
ag {{小明}} {{指定的目录}}
```
#### 寻找内容包含"foo"的文件，但只列出文件名:
```shell
ag -l {{小明}}
```
#### 忽略大小写，寻找内容包含"ABC"的文件，并只输出匹配的内容，而非整行:
```shell
ag -i -o {{ABC}}
```
#### 在文件名包含"小红"的文件中寻找"小明":
```shell
ag {{小明}} -G {{小红}}
```
#### 使用正则表达式来匹配文件内容:
```shell
ag '{{^ba(r|z)$}}'
```
#### 输出文件名包含"小明"的文件名:
```shell
ag -g {{小明}}
```
{% endraw %}{% raw %}
<h2 id="airpaste">
  <a href="/zh/common/airpaste.html">airpaste</a> <a href="#airpaste"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在同一网络下共享信息和文件.
> 更多信息： <https://github.com/mafintosh/airpaste>.

#### 等待接收消息并显示接收到的信息:
```shell
airpaste
```
#### 发送文本:
```shell
echo {{文本}} | airpaste
```
#### 发送文件:
```shell
airpaste < {{文件的路径}}
```
#### 接收文件:
```shell
airpaste > {{文件的路径}}
```
#### 创建 / 加入频道:
```shell
airpaste {{频道名}}
```
{% endraw %}{% raw %}
<h2 id="alacritty">
  <a href="/zh/common/alacritty.html">alacritty</a> <a href="#alacritty"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 跨平台，GPU 加速的终端模拟器.
> 更多信息： <https://github.com/alacritty/alacritty>.

#### 打开一个新的 Alacritty 窗口:
```shell
alacritty
```
#### 运行在指定目录中：
```shell
alacritty --working-directory {{路径}}
```
#### 在新的 Alacritty 窗口中运行命令:
```shell
alacritty -e {{命令}}
```
#### 指定备用配置文件 (默认在 `$XDG_CONFIG_HOME/alacritty/alacritty.yml`):
```shell
alacritty --config-file {{路径/config.yml}}
```
#### 在启用实时配置重新加载的情况下运行（默认情况下也可以在 `alacritty.yml` 中启用）:
```shell
alacritty --live-config-reload --config-file {{路径/config.yml}}
```
{% endraw %}{% raw %}
<h2 id="alias">
  <a href="/zh/common/alias.html">alias</a> <a href="#alias"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 创建别名 -- 用给定的字符串指代特定的命令.
> 别名只会在当前的 shell 会话中生效，除非它们在 shell 的配置文件中被定义，例如`~/.bashrc`.
> 更多信息： <https://tldp.org/LDP/abs/html/aliases.html>.

#### 创建一个通用的别名:
```shell
alias {{别名}}="{{命令}}"
```
#### 通过给定的别名查看它所指代的命令:
```shell
alias {{别名}}
```
#### 移除一个别名:
```shell
unalias {{别名}}
```
#### 列出所有的别名:
```shell
alias -p
```
#### 将 rm 转换为交互式命令:
```shell
alias {{rm}}="{{rm -i}}"
```
#### 创建别名`la`来指代`ls -a`:
```shell
alias {{la}}="{{ls -a}}"
```
{% endraw %}{% raw %}
<h2 id="androguard">
  <a href="/zh/common/androguard.html">androguard</a> <a href="#androguard"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 使用python编写的一款针对安卓应用的逆向工程工具.
> 更多信息: <https://github.com/androguard/androguard>.

#### 展示Android manifest清单文件:
```shell
androguard axml {{路径/至/应用.apk}}
```
#### 展示app元数据 (版本和app ID):
```shell
androguard apkid {{路径/至/应用.apk}}
```
#### 反编译Java代码:
```shell
androguard decompile {{路径/至/应用.apk}} --output {{路径/至/目录}}
```
{% endraw %}{% raw %}
<h2 id="ansible-galaxy">
  <a href="/zh/common/ansible-galaxy.html">ansible-galaxy</a> <a href="#ansible-galaxy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 创建和管理 Ansible 角色.
> 主页：<https://docs.ansible.com/ansible/latest/cli/ansible-galaxy.html>.

#### 安装一个角色:
```shell
ansible-galaxy install {{用户名.角色名}}
```
#### 移除一个角色:
```shell
ansible-galaxy remove {{用户名.角色名}}
```
#### 列出已安装的角色:
```shell
ansible-galaxy list
```
#### 搜索一个指定的角色:
```shell
ansible-galaxy search {{角色名}}
```
#### 创建一个新的角色:
```shell
ansible-galaxy init {{角色名}}
```
{% endraw %}{% raw %}
<h2 id="ansible-playbook">
  <a href="/zh/common/ansible-playbook.html">ansible-playbook</a> <a href="#ansible-playbook"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 通过 SSH 协议在远程计算机上执行 playbook 中定义的任务.
> 主页：<https://docs.ansible.com/ansible/latest/cli/ansible-playbook.html>.

#### 执行 playbook 中的任务:
```shell
ansible-playbook {{playbook}}
```
#### 在给定的主机清单文件中执行 playbook 中的命令:
```shell
ansible-playbook {{playbook}} -i {{清单文件}}
```
#### 通过定义在命令行中额外的变量执行 playbook 中的任务:
```shell
ansible-playbook {{playbook}} -e "{{变量 1}}={{值 1}} {{变量 2}}={{值 2}}"
```
#### 通过定义在一个 json 格式的文件中额外的变量执行 playbook 中的任务:
```shell
ansible-playbook {{playbook}} -e "@{{variables.json}}"
```
{% endraw %}{% raw %}
<h2 id="ansible">
  <a href="/zh/common/ansible.html">ansible</a> <a href="#ansible"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 通过 SSH 协议远程管理计算机组.
> 使用 `/etc/ansible/hosts` 文件来添加组 / 主机.
> 主页：<https://www.ansible.com/>.

#### 列出给定组下的所有主机:
```shell
ansible {{组}} --list-hosts
```
#### 调用 ping 模块来 ping 一组主机:
```shell
ansible {{组}} -m ping
```
#### 通过调用安装模块来显示关于一组主机的信息:
```shell
ansible {{组}} -m setup
```
#### 调用命令模块并使用给定的参数来对一组主机执行命令:
```shell
ansible {{组}} -m command -a '{{命令}}'
```
#### 以管理员权限执行一个命令:
```shell
ansible {{组}} --become --ask-become-pass -m command -a '{{命令}}'
```
#### 使用自定义的清单文件执行一个命令:
```shell
ansible {{组}} -i {{清单文件}} -m command -a '{{命令}}'
```
{% endraw %}{% raw %}
<h2 id="ansiweather">
  <a href="/zh/common/ansiweather.html">ansiweather</a> <a href="#ansiweather"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一个 shell 脚本，用于在终端中显示当前的天气状况.

#### 使用公制单位显示 Rzeszow, Poland 接下来 5 天的天气预报:
```shell
ansiweather -u {{metric}} -f {{5}} -l {{Rzeszow,PL}}
```
#### 显示带符号和日光数据信息的天气预报:
```shell
ansiweather -s {{true}} -d {{true}}
```
#### 显示带风力等级和湿度信息的天气预报:
```shell
ansiweather -w {{true}} -h {{true}}
```
{% endraw %}{% raw %}
<h2 id="apg">
  <a href="/zh/common/apg.html">apg</a> <a href="#apg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 生成任意复杂度的随机密码.
> 更多信息： <https://manned.org/apg>.

#### 生成随机密码 （默认密码长度为 8 位）:
```shell
apg
```
#### 生成密码，包含至少 1 个符号 (S), 1 个数字 (N), 1 个大写字母 (C), 1 个小写字母 (L):
```shell
apg -M SNCL
```
#### 生成 16 个字符的密码:
```shell
apg -m {{16}}
```
#### 生成最大长度为 16 位的密码:
```shell
apg -x {{16}}
```
#### 生成未出现在字典中的密码（必须提供字典文件）
```shell
apg -r {{字典文件}}
```
{% endraw %}{% raw %}
<h2 id="apktool">
  <a href="/zh/common/apktool.html">apktool</a> <a href="#apktool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> APK文件反编译工具
> 更多信息: <https://ibotpeaches.github.io/Apktool/>.

#### 反编译:
```shell
apktool d {{应用.apk}}
```
#### 将一个文件夹打包为apk文件:
```shell
apktool b {{路径/到/目录}}
```
#### 安装并存储框架:
```shell
apktool if {{框架.apk}}
```
{% endraw %}{% raw %}
<h2 id="apm">
  <a href="/zh/common/apm.html">apm</a> <a href="#apm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Atom 编辑器的包管理工具.
> 参见 `atom`.

#### 下载包：http://atom.io/packages 和主题 http://atom.io/themes:
```shell
apm install {{包名}}
```
#### 移除包 / 主题:
```shell
apm remove {{包名}}
```
#### 升级包 / 主题:
```shell
apm upgrade {{包名}}
```
{% endraw %}{% raw %}
<h2 id="apropos">
  <a href="/zh/common/apropos.html">apropos</a> <a href="#apropos"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在 manpages 中搜索，例如查找一个新命令.
> 更多信息： <https://manned.org/apropos>.

#### 搜索关键字:
```shell
apropos {{正则表达式}}
```
#### 搜索时不限制输出到终端宽度:
```shell
apropos -l {{正则表达式}}
```
{% endraw %}{% raw %}
<h2 id="ar">
  <a href="/zh/common/ar.html">ar</a> <a href="#ar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 创建，修改，提取库文件 (`.a`, `.so`, `.o`).
> 更多信息： <https://manned.org/ar>.

#### 从库文件中提取全部成员:
```shell
ar -x {{a 文件}}
```
#### 列出库文件中的成员:
```shell
ar -t {{a 文件}}
```
#### 替换或添加文件到库文件:
```shell
ar -r {{要被添加内容的 a 文件}} {{o 文件 1}} {{o 文件 2}} {{o 文件 3}}
```
#### 插入对象文件索引（相当于使用`ranlib`):
```shell
ar -s {{a 文件}}
```
#### 使用文件和附带的目标文件索引创建存档:
```shell
ar -rs {{a 文件}} {{o 文件 1}} {{o 文件 2}} {{o 文件 3}}
```
{% endraw %}{% raw %}
<h2 id="arch">
  <a href="/zh/common/arch.html">arch</a> <a href="#arch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 展示系统架构的名称.
> 另见`uname`.
> 更多信息： <https://www.gnu.org/software/coreutils/arch>.

#### 展示系统架构.
```shell
arch
```
{% endraw %}{% raw %}
<h2 id="aria2">
  <a href="/zh/common/aria2.html">aria2</a> <a href="#aria2"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一个轻量级多协议和多源命令行下载工具
> 支持 HTTP, HTTPS, FTP, SFTP, BitTorrent and Metalink.
> 主页：<https://aria2.github.io/>.

#### 下载一个网络资源:
```shell
aria2c {{http://example.org/myLinux.iso}}
```
#### 从多个源处下载一个资源:
```shell
aria2c {{http://mirror1.org/myLinux.iso}} {{http://mirror2.org/myLinux.iso}}
```
#### 使用两个连接下载资源:
```shell
aria2c -x{{2}} {{http://example.org/myLinux.iso}}
```
#### 从 Metalink URI 中下载资源:
```shell
aria2c {{http://example.org/myLinux.metalink}}
```
#### 从 BitTorrent URI 中下载资源:
```shell
aria2c {{http://example.org/myLinux.torrent}}
```
#### 从 BitTorrent Magnet URI 中下载资源:
```shell
aria2c {{'magnet:?xt=urn:btih:248D0A1CD08284299DE78D5C1ED359BB46717D8C'}}
```
#### 从一个文件中下载资源:
```shell
aria2c -i {{uris.txt}}
```
{% endraw %}{% raw %}
<h2 id="aria2c">
  <a href="/zh/common/aria2c.html">aria2c</a> <a href="#aria2c"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 快速下载工具.
> 支持 HTTP(S), FTP, SFTP, BitTorrent, and Metalink.

#### 下载一个 URI 到文件:
```shell
aria2c {{url}}
```
#### 从多个源处下载一个资源:
```shell
aria2c {{url_1}} {{url_2}}
```
#### 通过保存在一个文件中的 URL 列表来下载资源:
```shell
aria2c -i {{文件名}}
```
#### 使用多个连接下载资源:
```shell
aria2c -s {{连接数量}} {{url}}
```
#### 通过带用户名密码验证的 FTP 协议下载资源:
```shell
aria2c --ftp-user={{用户名}} --ftp-passwd={{密码}} {{url}}
```
#### 限制下载速度 (bytes/s):
```shell
aria2c --max-download-limit={{速度}} {{url}}
```
{% endraw %}{% raw %}
<h2 id="arp">
  <a href="/zh/common/arp.html">arp</a> <a href="#arp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示和操作系统的 ARP 缓存.
> 更多信息： <https://manned.org/arp>.

#### 显示当前的 ARP 表:
```shell
arp -a
```
#### 清除整个缓存:
```shell
sudo arp -a -d
```
#### 删除特定条目:
```shell
arp -d {{地址}}
```
#### 创建指定条目:
```shell
arp -s {{地址}} {{MAC 地址}}
```
{% endraw %}{% raw %}
<h2 id="asar">
  <a href="/zh/common/asar.html">asar</a> <a href="#asar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Electron 平台的文件打包工具.

#### 打包一个文件或目录:
```shell
asar pack {{文件或目录路径}} {{输出的 asar 文件}}
```
#### 解压一个 asar 文件:
```shell
asar extract {{asar 文件}}
```
#### 从 asar 文件中解压指定的文件:
```shell
asar extract-file {{asar 文件}} {{文件}}
```
#### 列出一个 asar 文件中的内容:
```shell
asar list {{asar 文件}}
```
{% endraw %}{% raw %}
<h2 id="asciinema">
  <a href="/zh/common/asciinema.html">asciinema</a> <a href="#asciinema"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 录制和播放终端会话，也可以把他们分享到 asciinema.org.

#### 将本地安装的`asciinema`与 asciinema.org 账号关联:
```shell
asciinema auth
```
#### 进行新的录制（完成后，将提示用户上传或在本地保存:
```shell
asciinema rec
```
#### 进行新的录制，保存到本地的文件中:
```shell
asciinema rec {{文件路径}}.cast
```
#### 从本地文件中播放终端录屏:
```shell
asciinema play {{文件路径}}.cast
```
#### 在 asciinema.org 中播放终端录屏:
```shell
asciinema play https://asciinema.org/a/{{文件 ID}}
```
#### 进行新的录制，将闲置时间设置为最多 2.5 秒:
```shell
asciinema rec -i {{2.5}}
```
#### 打印本地保存的录像的完整输出:
```shell
asciinema cat {{文件路径}}.cast
```
#### 从本地上传一个录屏到 asciinema.org:
```shell
asciinema upload {{文件路径}}.cast
```
{% endraw %}{% raw %}
<h2 id="asdf">
  <a href="/zh/common/asdf.html">asdf</a> <a href="#asdf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 可扩展的包版本管理器，支持Nodejs,Ruby,Elixir,Erlang等.
> 更多信息: <https://asdf-vm.com>.

#### 可用插件清单:
```shell
asdf plugin-list-all
```
#### 安装插件:
```shell
asdf plugin-add {{插件名}}
```
#### 软件包的可用版本清单:
```shell
asdf list-all {{软件包名}}
```
#### 安装指定版本的软件包:
```shell
asdf install {{软件包名}} {{版本}}
```
#### 设置软件包的全局安装版本:
```shell
asdf global {{软件包名}} {{版本}}
```
#### 设置软件包的本地版本:
```shell
asdf local {{软件包名}} {{版本}}
```
{% endraw %}{% raw %}
<h2 id="atom">
  <a href="/zh/common/atom.html">atom</a> <a href="#atom"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一个跨平台的，可插拔的文本编辑器.
> 由 `apm` 管理插件.
> 更多信息：<https://atom.io/>.

#### 打开文件或目录:
```shell
atom {{path/to/file_or_directory}}
```
#### 在新窗口中打开文件或目录:
```shell
atom -n {{path/to/file_or_directory}}
```
#### 在已有窗口中打开文件或目录:
```shell
atom --add {{path/to/file_or_directory}}
```
#### 以安全模式启动 Atom （不加载额外插件）:
```shell
atom --safe
```
#### 在终端前台运行 Atom:
```shell
atom --foreground
```
{% endraw %}{% raw %}
<h2 id="autoflake">
  <a href="/zh/common/autoflake.html">autoflake</a> <a href="#autoflake"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一个工具，用于检查python代码中未被使用的引入和变量.
> 更多信息: <https://github.com/myint/autoflake>.

#### 移除指定文件中未使用的变量，并展示diff:
```shell
autoflake --remove-unused-variables {{文件.py}}
```
#### 移除多个文件中未使用的引入，并展示diffs:
```shell
autoflake --remove-all-unused-imports {{文件1.py}} {{文件2.py}} {{文件3.py}}
```
#### 移除未被使用的变量，并覆盖更新:
```shell
autoflake --remove-unused-variables --in-place {{文件.py}}
```
#### 递归地移除指定文件夹下层所有文件中未使用的变量，并覆盖更新:
```shell
autoflake --remove-unused-variables --in-place --recursive {{路径/到/目录}}
```
{% endraw %}{% raw %}
<h2 id="autojump">
  <a href="/zh/common/autojump.html">autojump</a> <a href="#autojump"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 快速跳转，访问次数最多的文件夹优先.
> 使用j、jc、jo作为别名.
> 更多信息: <https://github.com/wting/autojump>.

#### 跳转到包含指定通配符的目录:
```shell
j {{通配符表达式}}
```
#### 跳转到包含指定通配符的目录的下一级:
```shell
jc {{通配符表达式}}
```
#### 使用系统文件管理器，打开指定的目录:
```shell
jo {{通配符表达式}}
```
#### 从autojump数据库中删除不存在的目录:
```shell
j --purge
```
#### 展示autojump数据库数据:
```shell
j -s
```
{% endraw %}{% raw %}
<h2 id="axel">
  <a href="/zh/common/axel.html">axel</a> <a href="#axel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一款下载加速器.
> 支持HTTP, HTTPS, 和 FTP.
> 更多信息: <https://github.com/axel-download-accelerator/axel>.

#### 链接下载:
```shell
axel {{超链接}}
```
#### 链接下载，指定文件名:
```shell
axel {{超链接}} -o {{文件名称}}
```
#### 多连接数下载:
```shell
axel -n {{连接数量}} {{超链接}}
```
#### 查询镜像:
```shell
axel -S {{镜像数量}} {{超链接}}
```
#### 限制下载速度 (字节bite每秒):
```shell
axel -s {{字节数}} {{超链接}}
```
{% endraw %}{% raw %}
<h2 id="babel">
  <a href="/zh/common/babel.html">babel</a> <a href="#babel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一款JavaScript的编译器，将下一代ES语法转换为兼容语法。
> 更多信息: <https://babeljs.io/>.

#### 转编译指定文件到标准输出:
```shell
babel {{路径/到/文件}}
```
#### 转编译指定文件，输入为特定文件:
```shell
babel {{路径/到/输入文件}} --out-file {{路径/到/输出文件}}
```
#### 监听文件变动触发转编译:
```shell
babel {{路径/到/输入文件}} --watch
```
#### 转编译整个目录下的js文件:
```shell
babel {{路径/到/输入文件目录}}
```
#### 跳过指定目录下指定文件的编译（多文件使用英文逗号“,”分隔）:
```shell
babel {{路径/到/输入文件目录}} --ignore {{被忽略文件}}
```
#### 转编译后，执行压缩:
```shell
babel {{路径/到/输入文件}} --minified
```
#### 使用预设值:
```shell
babel {{路径/到/输入文件}} --presets {{预设项}}
```
{% endraw %}{% raw %}
<h2 id="banner">
  <a href="/zh/common/banner.html">banner</a> <a href="#banner"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将给定参数输出为大型 ASCII 文字.
> 更多信息： <https://man.archlinux.org/man/banner.1>.

#### 将文字信息打印为大横幅（引号是可选的）:
```shell
banner "{{Hello World}}"
```
#### 将文字信息打印为横幅，宽度为 50 个字:
```shell
banner -w {{50}} "{{Hello World}}"
```
#### 从 stdin 中读取文本:
```shell
banner
```
{% endraw %}{% raw %}
<h2 id="base32">
  <a href="/zh/common/base32.html">base32</a> <a href="#base32"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将文件或标准输入编码到Base32或从Base32解码为标准输出。
> 更多信息： <https://www.gnu.org/software/coreutils/base32>.

#### 编码一个文件:
```shell
base32 {{文件名}}
```
#### 解码一个文件:
```shell
base32 --decode {{文件名}}
```
#### 从标准输入编码:
```shell
{{某指令}} | base32
```
#### 将标准输入解码:
```shell
{{某指令}} | base32 --decode
```
{% endraw %}{% raw %}
<h2 id="base64">
  <a href="/zh/common/base64.html">base64</a> <a href="#base64"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 将文件或标准输入编码到Base64或从Base64解码为标准输出。
> 更多信息： <https://www.gnu.org/software/coreutils/base64>.

#### 编码一个文件:
```shell
base64 {{文件名}}
```
#### 解码一个文件:
```shell
base64 --decode {{文件名}}
```
#### 从标准输入编码:
```shell
{{某指令}} | base64
```
#### 将标准输入解码:
```shell
{{某指令}} | base64 --decode
```
{% endraw %}{% raw %}
<h2 id="basename">
  <a href="/zh/common/basename.html">basename</a> <a href="#basename"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 移除一个路径的目录部分字符.
> 更多信息： <https://www.gnu.org/software/coreutils/basename>.

#### 仅显示文件名:
```shell
basename {{路径/到/文件}}
```
#### 显示路径字符最右边表示目录的字符:
```shell
basename {{路径/到/目录/}}
```
#### 展示无后缀的文件名称:
```shell
basename {{路径/到/文件}} {{后缀}}
```
{% endraw %}{% raw %}
<h2 id="bash">
  <a href="/zh/common/bash.html">bash</a> <a href="#bash"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bourne-Again SHell.
> 兼容`sh`的命令行解释器.
> 更多信息: <https://gnu.org/software/bash>.

#### 启动交互式 shell:
```shell
bash
```
#### 执行命令:
```shell
bash -c "{{command}}"
```
#### 执行脚本文件:
```shell
bash {{file.sh}}
```
#### 执行脚本文件，并将所有执行过的命令输出到终端:
```shell
bash -x {{file.sh}}
```
#### 执行脚本文件，并在第一个错误处终止:
```shell
bash -e {{file.sh}}
```
#### 从输入 (stdin) 读取命令:
```shell
bash -s
```
#### 将跟随的所有选项原样传递到要执行的脚本文件（可与`-s`选项共用来将选项传递到来自输入的命令 / 脚本）
```shell
bash --
```
#### 打印 bash 的版本信息 （使用`echo $BASH_VERSION`来获得纯粹的版本字符串）:
```shell
bash --version
```
{% endraw %}{% raw %}
<h2 id="bashmarks">
  <a href="/zh/common/bashmarks.html">bashmarks</a> <a href="#bashmarks"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 使用一个字母的命令，保存或者跳转到常用的目录
> 更多信息: <https://github.com/huyng/bashmarks>.

#### 可访问书签清单:
```shell
l
```
#### 保存当前目录到某书签里:
```shell
s {{书签名}}
```
#### 跳转到指定书签
```shell
g {{书签名}}
```
#### 打印书签目录内容
```shell
p {{书签名}}
```
#### 删除书签：
```shell
d {{书签名}}
```
{% endraw %}{% raw %}
<h2 id="bat">
  <a href="/zh/common/bat.html">bat</a> <a href="#bat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 可以打印并且合并文件的命令.
> `cat`的复制品，外加无法高亮和git集成.
> 更多信息: <https://github.com/sharkdp/bat>.

#### 文件内容打印:
```shell
bat {{文件}}
```
#### 多文件合并到目标文件:
```shell
bat {{文件1}} {{文件2}} > {{目标文件}}
```
#### 在指定文件后追加多个文件合并的内容:
```shell
bat {{文件1}} {{文件2}} >> {{目标文件}}
```
#### 打印时，显示行号:
```shell
bat -n {{文件}}
```
#### 高亮一个json文件:
```shell
bat --language json {{文件.json}}
```
#### 受支持的语言清单:
```shell
bat --list-languages
```
{% endraw %}{% raw %}
<h2 id="behat">
  <a href="/zh/common/behat.html">behat</a> <a href="#behat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 基于Behaviour-Driven Development的自动化测试PHP框架
> 更多信息: <https://behat.org>.

#### 初始化一个PHP behat项目:
```shell
behat --init
```
#### 运行所有测试:
```shell
behat
```
#### 运行指定组所有的测试用例:
```shell
behat --suite={{组名}}
```
#### 运行所有测试，指定输入格式:
```shell
behat --format {{pretty|progress}}
```
#### 将测试结果输出到指定文件:
```shell
behat --out {{路径/到/文件}}
```
#### 展示测试组所在的目录清单:
```shell
behat --definitions
```
{% endraw %}{% raw %}
<h2 id="bg">
  <a href="/zh/common/bg.html">bg</a> <a href="#bg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 恢复被挂起的任务 (如. 使用 `Ctrl + Z`), 使它们在后台运行.
> 更多信息： <https://manned.org/bg>.

#### 恢复最近被挂起的任务，在后台运行:
```shell
bg
```
#### 恢复特定的任务 (使用 `jobs -l` 可以获取任务ID) 并在后台运行:
```shell
bg %{{job_id}}
```
{% endraw %}{% raw %}
<h2 id="bmaptool">
  <a href="/zh/common/bmaptool.html">bmaptool</a> <a href="#bmaptool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 便捷地创建或复制块文件映射（被设计的比`cp`或`dd`更快）.
> 更多信息: <https://source.tizen.org/documentation/reference/bmaptool>.

#### 使用图片生成块图文件:
```shell
bmaptool create -o {{blockmap格式文件.bmap}} {{图片文件}}
```
#### 复制图片到指定目录:
```shell
bmaptool copy --bmap {{blockmap格式文件}} {{图片文件}} {{/开发路径/sdb}}
```
#### 复制压缩后的图片到指定目录:
```shell
bmaptool copy --bmap {{blockmap格式文件}} {{图片文件.gz}} {{/开发路径/sdb}}
```
#### 复制图片的时候，不将图片转成块图:
```shell
bmaptool copy --nobmap {{图片文件}} {{/开发路径/sdb}}
```
{% endraw %}{% raw %}
<h2 id="bower">
  <a href="/zh/common/bower.html">bower</a> <a href="#bower"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 前端web开发的包管理优化工具。
> 一个包可以是GitHub中user/repo的缩写，一个Git端口，一个URL链接或者一个已注册的包。
> 更多信息: <https://bower.io/>.

#### 安装列在项目下 的bower.json文件中的依赖:
```shell
bower install
```
#### 安装一个或者多个依赖到bower_components目录:
```shell
bower install {{包名1}} {{包名2}}
```
#### 从本地的bower_components目录卸载依赖
```shell
bower uninstall {{包名1}} {{包名2}}
```
#### 列出本地包和可能的更新项:
```shell
bower list
```
#### 显示bower指令的帮助信息:
```shell
bower help {{指令}}
```
#### 创建你的项目的bower.json:
```shell
bower init
```
#### 安装时候指定依赖的版本号，并添加到bower.json:
```shell
bower install {{local_name}}={{package}}#{{version}} --save
```
{% endraw %}{% raw %}
<h2 id="browser-sync">
  <a href="/zh/common/browser-sync.html">browser-sync</a> <a href="#browser-sync"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 启动一个本地的服务，可以监听文件改动，刷新浏览器.
> 更多信息: <https://browsersync.io/docs/command-line>.

#### 将指定目录发成服务:
```shell
browser-sync start --server {{路径/到/目录}} --files {{路径/到/目录}}
```
#### 启动当前目录服务，同时监听指定目录下css文件的变动
```shell
browser-sync start --server --files '{{路径/到/目录/*.css}}'
```
#### 创建配置文件:
```shell
browser-sync init
```
#### 按指定配置文件中的配置启动服务:
```shell
browser-sync start --config {{配置文件}}
```
{% endraw %}{% raw %}
<h2 id="btm">
  <a href="/zh/common/btm.html">btm</a> <a href="#btm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 命令行`top`的替代品.
> 比`top更轻便，支持跨平台、图表更丰富`.
> 更多信息: <https://github.com/ClementTsang/bottom>.

#### 展示默认布局 (cpu, 内存, 温度, 磁盘, 网络和 进程):
```shell
btm
```
#### 开启基础模式,关闭图表和高亮(接近于 `top`):
```shell
btm --basic
```
#### 将图表中的小点换成大点:
```shell
btm --dot_marker
```
#### 展示电池充电和健康状态:
```shell
btm --battery
```
#### 设置图表刷新间隔和留存数据的时长:
```shell
btm --rate 250 --default_time_value 30000
```
{% endraw %}{% raw %}
<h2 id="buku">
  <a href="/zh/common/buku.html">buku</a> <a href="#buku"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 命令行版本的书签管理器.
> 更多信息: <https://github.com/jarun/Buku>.

#### 根据关键词和标签查找书签:
```shell
buku {{关键字}} --stag {{标签}}
```
#### 添加书签，并且打上标签:
```shell
buku --add {{https://example.com}} {{搜索引擎}}, {{标签}}
```
#### 删除一个书签:
```shell
buku --delete {{书签id}}
```
#### 打开编辑器，修改书签:
```shell
buku --write {{书签id}}
```
#### 将指定标签移除:
```shell
buku --update {{书签id}} --tag {{-}} {{搜索引擎}}
```
{% endraw %}{% raw %}
<h2 id="carbon-now">
  <a href="/zh/common/carbon-now.html">carbon-now</a> <a href="#carbon-now"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 创建漂亮的代码图片。
> 更多信息在 <https://github.com/mixn/carbon-now-cli>.

#### 使用默认设置从文件创建图片:
```shell
carbon-now {{文件}}
```
#### 使用默认设置从剪贴板创建图片:
```shell
carbon-now --from-clipboard
```
#### 使用默认设置从标准输入创建图片:
```shell
{{输入}} | carbon-now
```
#### 以交互方式创建图片以进行自定义设置，还可以选择保存预设:
```shell
carbon-now -i {{文件}}
```
#### 从先前保存的预设创建图片:
```shell
carbon-now -p {{预设}} {{文件}}
```
#### 从指定的文本行开始:
```shell
carbon-now -s {{行号}} {{文件}}
```
#### 结束于指定的文本行:
```shell
carbon-now -e {{行号}} {{文件}}
```
#### 在浏览器中打开图片而不是保存:
```shell
carbon-now --open {{文件}}
```
{% endraw %}{% raw %}
<h2 id="case">
  <a href="/zh/common/case.html">case</a> <a href="#case"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> case ... esac 与其他语言中的 switch ... case 语句类似，是一种多分枝选择结构.
> 更多信息： <https://manned.org/case>.

#### 通过字符串字面量判断执行分支:
```shell
case {{入参变量}} in {{字符字面量1}} {{执行语句块1}} ;; {{字符字面量2}}) {{执行语句块2}} ;; *) {{默认执行语句块}} ;; esac
```
#### 搭配通配符进行匹配，判断执行分支:
```shell
case {{入参变量}} in {{通配符或者字符字面量}}) {{执行语句块1}} ; ;; {{通配符或者字符字面量}}) {{执行语句块1}}; ;; *) {{echo "what?"}}; ;; esac
```
{% endraw %}{% raw %}
<h2 id="cat">
  <a href="/zh/common/cat.html">cat</a> <a href="#cat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 打印和拼接文件的工具.
> 更多信息： <https://www.gnu.org/software/coreutils/cat>.

#### 以标准输出，打印文件内容:
```shell
cat {{file}}
```
#### 多文件合并到目标文件:
```shell
cat {{file1}} {{file2}} > {{target_file}}
```
#### 多文件合并，并追加到目标文件:
```shell
cat {{file1}} {{file2}} >> {{target_file}}
```
#### 显示行号:
```shell
cat -n {{file}}
```
#### 显示不可打印和空白的字符 (使用`M-` 前缀标记非ASCII字符):
```shell
cat -v -t -e {{file}}
```
{% endraw %}{% raw %}
<h2 id="cd">
  <a href="/zh/common/cd.html">cd</a> <a href="#cd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 更改当前工作目录.
> 更多信息： <https://man.archlinux.org/man/cd.n>.

#### 转到指定目录:
```shell
cd {{路径}}
```
#### 转到当前用户的主（home）目录:
```shell
cd
```
#### 转到当前目录的父目录:
```shell
cd ..
```
#### 转到刚才选择的目录:
```shell
cd -
```
{% endraw %}{% raw %}
<h2 id="clear">
  <a href="/zh/common/clear.html">clear</a> <a href="#clear"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 清空终端的屏幕.
> 更多信息： <https://manned.org/clear>.

#### 清空屏幕（相当于在 Bash shell 中按 Control-L 键）:
```shell
clear
```
#### 清空屏幕但保留终端的回滚缓冲区:
```shell
clear -x
```
#### 指明要清空的终端类型（默认为环境变量 `TERM` 的值）:
```shell
clear -T {{type_of_terminal}}
```
#### 显示 `clear` 使用的 `ncurses` 版本:
```shell
clear -V
```
{% endraw %}{% raw %}
<h2 id="code">
  <a href="/zh/common/code.html">code</a> <a href="#code"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Visual Studio Code.
> 更多信息: <https://github.com/microsoft/vscode>.

#### 打开 VS Code:
```shell
code
```
#### 在 VS Code 中打开当前目录:
```shell
code .
```
#### 在 VS Code 打开一个文件或目录:
```shell
code {{路径/文件或目录}}
```
#### 在当前打开的 VS Code 窗口中打开一个文件或目录:
```shell
code --reuse-window {{路径/文件或目录}}
```
#### 在 VS Code 中对比两个文件:
```shell
code -d {{文件1}} {{文件2}}
```
#### 用超级用户 (sudo) 权限打开 VS Code:
```shell
sudo code {{路径/文件或目录}} --user-data-dir
```
{% endraw %}{% raw %}
<h2 id="command">
  <a href="/zh/common/command.html">command</a> <a href="#command"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 命令强制 shell 执行命令程序，并忽略具有相同名称的任何函数、内置函数和别名（会忽略掉一切别名，执行命令本身）.
> 更多信息： <https://manned.org/command>.

#### 从字面上执行 `ls` 程序，即使存在 ls 别名:
```shell
command {{ls}}
```
{% endraw %}{% raw %}
<h2 id="cp">
  <a href="/zh/common/cp.html">cp</a> <a href="#cp"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 复制文件和文件夹。
> 更多信息：<https://www.gnu.org/software/coreutils/cp>.

#### 将文件复制到另一个位置：
```shell
cp {{某路径/源文件.ext}} {{某路径/目标文件.ext}}
```
#### 将文件复制到另一个文件夹，并保留原来的文件名：
```shell
cp {{某路径/源文件.ext}} {{某路径/目标文件夹}}
```
#### 以递归方式将文件夹内的内容复制到另一个位置（如果目标文件夹存在，则将此文件夹复制到目标文件夹中）：
```shell
cp -R {{某路径/源文件夹}} {{某路径/目标文件夹}}
```
#### 以详细模式递归复制目录（在复制文件时显示文件信息）：
```shell
cp -vR {{某路径/源文件夹}} {{某路径/目标文件夹}}
```
#### 以交互方式将文本文件复制到另一个位置（覆盖之前会提示用户）：
```shell
cp -i {{*.txt}} {{某路径/目标文件夹}}
```
#### 复制之前，请遵循符号链接：
```shell
cp -L {{符号文件}} {{某路径/目标文件夹}}
```
{% endraw %}{% raw %}
<h2 id="curl">
  <a href="/zh/common/curl.html">curl</a> <a href="#curl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 向 / 从一个服务器传输数据.
> 支持大多数协议，包括 HTTP, FTP, 和 POP3.
> 更多信息：<https://curl.se>.

#### 将指定 URL 的内容下载到文件:
```shell
curl {{http://example.com}} --output {{文件名}}
```
#### 将文件从 URL 保存到由 URL 指示的文件名中:
```shell
curl --remote-name {{http://example.com/filename}}
```
#### 下载文件，跟随 重定向，并且自动 续传（恢复）前序文件传输:
```shell
curl --remote-name --location --continue-at - {{http://example.com/filename}}
```
#### Send form-encoded data (POST request of type `application/x-www-form-urlencoded`):
```shell
curl --data {{'name=bob'}} {{http://example.com/form}}
```
#### 发送带有额外请求头，使用自定义请求方法的请求:
```shell
curl --header {{'X-My-Header: 123'}} --request {{PUT}} {{http://example.com}}
```
#### 发送 JSON 格式的数据，并附加正确的 `Content-Type` 请求头:
```shell
curl --data {{'{"name":"bob"}'}} --header {{'Content-Type: application/json'}} {{http://example.com/users/1234}}
```
#### 使用用户名和密码，授权访问服务器:
```shell
curl --user myusername:mypassword {{http://example.com}}
```
#### 为指定资源使用客户端证书和密钥，并且跳过证书验证:
```shell
curl --cert {{client.pem}} --key {{key.pem}} --insecure {{https://example.com}}
```
{% endraw %}{% raw %}
<h2 id="echo">
  <a href="/zh/common/echo.html">echo</a> <a href="#echo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 输出给定参数.
> 更多信息： <https://www.gnu.org/software/coreutils/echo>.

#### 输出文本信息. 注意: 引号是可选的:
```shell
echo "{{Hello World}}"
```
#### 输出带有环境变量的信息:
```shell
echo "{{My path is $PATH}}"
```
#### 打印不带尾随换行符的信息：
```shell
echo -n "{{Hello World}}"
```
#### 向文件添加信息:
```shell
echo "{{Hello World}}" >> {{file.txt}}
```
#### 启用反斜杠转义的解释（特殊字符）:
```shell
echo -e "{{Column 1\tColumn 2}}"
```
{% endraw %}{% raw %}
<h2 id="etcd">
  <a href="/zh/common/etcd.html">etcd</a> <a href="#etcd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 分布式，可靠的键值存储，用于分布式系统中存储最关键的数据。
> 更多信息见：<https://etcd.io>.

#### 启动单节点 etcd 集群：
```shell
etcd
```
#### 启动一个单节点 etcd 集群，在自定义 URL 上侦听客户端请求：
```shell
etcd --advertise-client-urls {{http://127.0.0.1:1234}} --listen-client-urls {{http://127.0.0.1:1234}}
```
#### 使用自定义名称启动单节点 etcd 集群：
```shell
etcd --name {{my_etcd_cluster}}
```
#### 启动单节点 etcd 集群，同时可以在这里看到大量监控指标 http://localhost:2379/debug/pprof/:
```shell
etcd --enable-pprof --metrics extensive
```
{% endraw %}{% raw %}
<h2 id="exit">
  <a href="/zh/common/exit.html">exit</a> <a href="#exit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 退出终端程序。
> 更多信息见：<https://manned.org/exit>.

#### 使用最后执行命令的退出代码，退出终端程序：
```shell
exit
```
#### 使用指定的退出代码，退出终端程序：
```shell
exit {{exit_code}}
```
{% endraw %}{% raw %}
<h2 id="gh-gist">
  <a href="/zh/common/gh-gist.html">gh gist</a> <a href="#gh-gist"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在命令行上使用 GitHub Gists.
> 更多信息: <https://cli.github.com/manual/gh_gist>.

#### 从一个以空格分隔的文件列表中创建一个新的 Gist:
```shell
gh gist create {{路径/文件}}
```
#### 创建一个带有描述的新 Gist:
```shell
gh gist create {{文件名}} --desc "{{描述}}"
```
#### 编辑一个 Gist:
```shell
gh gist edit {{id_或_url}}
```
#### 列出当前登录用户所拥有的 Gist:
```shell
gh gist list --limit {{int}}
```
#### 在默认浏览器中查看 Gist，且不渲染 Markdown:
```shell
gh gist view {{id_或_url}} --web --raw
```
{% endraw %}{% raw %}
<h2 id="gh-repo">
  <a href="/zh/common/gh-repo.html">gh repo</a> <a href="#gh-repo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在命令行上操作 GitHub 仓库.
> 更多信息: <https://cli.github.com/manual/gh_repo>.

#### 创建一个新的仓库(如果没有设置仓库名称，默认将为当前目录的名称):
```shell
gh repo create {{名称}}
```
#### 克隆一个仓库:
```shell
gh repo clone {{拥有者}}/{{仓库}}
```
#### 复刻并克隆一个仓库:
```shell
gh repo fork {{拥有者}}/{{仓库}} --clone
```
#### 在网络浏览器中查看仓库:
```shell
gh repo view {{仓库}} --web
```
{% endraw %}{% raw %}
<h2 id="gpg-zip">
  <a href="/zh/common/gpg-zip.html">gpg-zip</a> <a href="#gpg-zip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 使用`GPG`加密存档中的文件和目录。
> 更多信息： <https://www.gnupg.org/documentation/manuals/gnupg/gpg_002dzip.html>.

#### 使用密码将一个目录加密为`archive.gpg`：
```shell
gpg-zip --symmetric --output {{archive.gpg}} {{path/to/directory}}
```
#### 将`archive.gpg`解密到同名目录中：
```shell
gpg-zip --decrypt {{path/to/archive.gpg}}
```
#### 列出加密的`archive.gpg`的内容：
```shell
gpg-zip --list-archive {{path/to/archive.gpg}}
```
{% endraw %}{% raw %}
<h2 id="gpg">
  <a href="/zh/common/gpg.html">gpg</a> <a href="#gpg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> GNU Privacy Guard。
> 请参阅`gpg2`了解 GNU Privacy Guard 2。
> 更多信息：<https://docs.releng.linuxfoundation.org/en/latest/gpg.html>。

#### 不加密，仅对`doc.txt`进行签名（生成`doc.txt.asc`，格式为 ASCII 码形式）：
```shell
gpg --clearsign {{doc.txt}}
```
#### 对`doc.txt`进行签名并加密（生成`doc.txt.asc`，格式为 ASCII 码形式）：
```shell
gpg --local-user {{sender_id}} --recipient {{recipient_id}} --armor --sign --encrypt {{doc.txt}}
```
#### 为接收者 alice@example.com 加密`doc.txt`（生成`doc.txt.gpg`）：
```shell
gpg --encrypt --recipient {{alice@example.com}} {{doc.txt}}
```
#### 只用密码加密`doc.txt`（生成`doc.txt.gpg`）：
```shell
gpg --symmetric {{doc.txt}}
```
#### 解密`doc.txt.gpg`（输出到标准输出）：
```shell
gpg --decrypt {{doc.txt.gpg}}
```
#### 导入一个公钥：
```shell
gpg --import {{public.gpg}}
```
#### 导出 alice@example.com 的公钥（输出到标准输出）：
```shell
gpg --export --armor {{alice@example.com}}
```
#### 导出 alice@example.com 的私钥（输出到标准输出）：
```shell
gpg --export-secret-keys --armor {{alice@example.com}}
```
{% endraw %}{% raw %}
<h2 id="gpg2">
  <a href="/zh/common/gpg2.html">gpg2</a> <a href="#gpg2"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> GNU Privacy Guard 2。
> GNU Privacy Guard 1 请参见`gpg`。
> 更多信息：<https://docs.releng.linuxfoundation.org/en/latest/gpg.html>。

#### 列出导入的密钥（公钥）：
```shell
gpg2 --list-keys
```
#### 为指定的接收者加密指定的文件，将输出结果写到一个新的文件中，并附加`.gpg`：
```shell
gpg2 --encrypt --recipient {{alice@example.com}} {{path/to/doc.txt}}
```
#### 只用密码（对称加密）对指定文件进行加密，将输出结果写入一个附加`.gpg`的新文件：
```shell
gpg2 --symmetric {{path/to/doc.txt}}
```
#### 解密指定的文件，并将结果写入标准输出：
```shell
gpg2 --decrypt {{path/to/doc.txt.gpg}}
```
#### 导入一个公钥：
```shell
gpg2 --import {{path/to/public_key.gpg}}
```
#### 将指定电子邮件地址的公钥导出到标准输出：
```shell
gpg2 --export --armor {{alice@example.com}}
```
#### 将指定电子邮件地址的私钥导出到标准输出：
```shell
gpg2 --export-secret-keys --armor {{alice@example.com}}
```
{% endraw %}{% raw %}
<h2 id="gpgv">
  <a href="/zh/common/gpgv.html">gpgv</a> <a href="#gpgv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 验证 OpenPGP 签名。
> 更多信息：<https://www.gnupg.org/documentation/manuals/gnupg/gpgv.html>。

#### 验证签名文件：
```shell
gpgv {{path/to/file}}
```
#### 使用分离式签名验证已签名的文件：
```shell
gpgv {{path/to/signature}} {{path/to/file}}
```
#### 在 keyrings 列表中添加一个文件（一个导出的钥匙也算作一个 keyring）：
```shell
gpgv --keyring {{path/to/keyring_file}} {{path/to/signature}} {{path/to/file}}
```
{% endraw %}{% raw %}
<h2 id="gunicorn">
  <a href="/zh/common/gunicorn.html">gunicorn</a> <a href="#gunicorn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Python 的 WSGI http 服务器.

#### 运行 python web 应用程序:
```shell
gunicorn {{导入路径：应用程序}}
```
#### 在 localhost 上监听 8080 端口:
```shell
gunicorn --bind {{localhost}}:{{8080}} {{导入路径：应用程序}}
```
#### 启用实时自动加载:
```shell
gunicorn --reload {{导入路径：应用程序}}
```
#### 使用 4 个工作进程处理请求:
```shell
gunicorn --workers {{4}} {{导入路径：应用程序}}
```
#### 使用 4 个工作线程处理请求:
```shell
gunicorn --threads {{4}} {{导入路径：应用程序}}
```
#### 通过 https 运行应用程序:
```shell
gunicorn --certfile {{cert.pem}} --keyfile {{key.pem}} {{导入路径：应用程序}}
```
{% endraw %}{% raw %}
<h2 id="heroku">
  <a href="/zh/common/heroku.html">heroku</a> <a href="#heroku"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 从命令行创建和管理 Heroku 应用.
> 更多信息: <https://www.heroku.com/>.

#### 登录到你的 heroku 帐户:
```shell
heroku login
```
#### 创建一个 heroku 应用:
```shell
heroku create
```
#### 显示应用的日志:
```shell
heroku logs --app {{app_name}}
```
#### 在 dyno（Heroku 虚拟机）中运行一次性进程:
```shell
heroku run {{process_name}} --app {{app_name}}
```
#### 列出应用的 dyno（Heroku 虚拟机）:
```shell
heroku ps --app {{app_name}}
```
#### 永久销毁应用:
```shell
heroku destroy --app {{app_name}}
```
{% endraw %}{% raw %}
<h2 id="hexo">
  <a href="/zh/common/hexo.html">hexo</a> <a href="#hexo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 快速、简洁且高效的博客框架.
> 更多信息: <https://hexo.io/>.

#### 初始化一个网站:
```shell
hexo init {{path/to/directory}}
```
#### 创建一篇新文章:
```shell
hexo new {{layout}} {{title}}
```
#### 构建静态文件:
```shell
hexo generate
```
#### 启动本地服务器:
```shell
hexo server
```
#### 部署网站:
```shell
hexo deploy
```
#### 清理缓存文件 (`db.json`) 和生成的文件 (`public/`):
```shell
hexo clean
```
{% endraw %}{% raw %}
<h2 id="jar">
  <a href="/zh/common/jar.html">jar</a> <a href="#jar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Java 应用程序 / 类库打包程序。
> 更多信息见：<https://docs.oracle.com/javase/tutorial/deployment/jar/basicsindex.html>.

#### 将当前目录中的所有文件递归归档到 `.jar` 文件中：
```shell
jar cf {{file.jar}} *
```
#### 将 `.jar` / `.war` 文件解压缩到当前目录：
```shell
jar -xvf {{file.jar}}
```
#### 列出 `.jar` / `.war` 文件内容：
```shell
jar tf {{path/to/file.jar}}
```
#### 列出带有详细输出的 `.jar` / `.war` 文件内容：
```shell
jar tvf {{path/to/file.jar}}
```
{% endraw %}{% raw %}
<h2 id="jarsigner">
  <a href="/zh/common/jarsigner.html">jarsigner</a> <a href="#jarsigner"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 签名并验证 Java 存档（JAR）文件。
> 更多信息见：<https://docs.oracle.com/javase/9/tools/jarsigner.htm>.

#### 签名一个 `JAR` 文件：
```shell
jarsigner {{path/to/file.jar}} {{keystore_alias}}
```
#### 使用特定算法对 `JAR` 文件进行签名：
```shell
jarsigner -sigalg {{algorithm}} {{path/to/file.jar}} {{keystore_alias}}
```
#### 验证 `JAR` 文件的签名：
```shell
jarsigner -verify {{path/to/file.jar}}
```
{% endraw %}{% raw %}
<h2 id="java">
  <a href="/zh/common/java.html">java</a> <a href="#java"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Java 程序启动器.
> 更多信息: <https://java.com>.

#### 通过提供类名称运行一个含有 main 函数的 java .class 程序:
```shell
java {{类名称}}
```
#### 运行一个 .jar 程序:
```shell
java -jar {{文件名.jar}}
```
#### 运行一个 .jar 程序并且在端口5005等待调试器:
```shell
java -agentlib:jdwp=transport=dt_socket,server=y,suspend=y,address=*:5005 -jar {{文件名.jar}}
```
#### 显示 JDK, JRE 和 HotSpot 的版本:
```shell
java -version
```
#### 显示详细的帮助:
```shell
java -help
```
{% endraw %}{% raw %}
<h2 id="javac">
  <a href="/zh/common/javac.html">javac</a> <a href="#javac"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Java 程序编译器.

#### 编译一个 `.java` 文件:
```shell
javac {{文件名.java}}
```
#### 编译多个 `.java` 文件:
```shell
javac {{文件名1.java}} {{文件名2.java}} {{文件名3.java}}
```
#### 编译当前目录内所有 `.java` 文件:
```shell
javac {{*.java}}
```
#### 编译一个 `.java` 文件并将生成的 class 字节码文件放入一个指定目录:
```shell
javac -d {{输出目录}} {{文件名.java}}
```
{% endraw %}{% raw %}
<h2 id="javadoc">
  <a href="/zh/common/javadoc.html">javadoc</a> <a href="#javadoc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 从源代码以 HTML 格式生成 Java API 文档。
> 更多信息见：https://docs.oracle.com/javase/9/javadoc/javadoc-command.htm>.

#### 生成 Java 源代码的文档并将结果保存在文件夹中：
```shell
javadoc -d {{path/to/directory/}} {{path/to/java_source_code}}
```
#### 生成指定编码的文档：
```shell
javadoc -docencoding {{UTF-8}} {{path/to/java_source_code}}
```
#### 生成文档时，排除掉某些软件包：
```shell
javadoc -exclude {{package_list}} {{path/to/java_source_code}}
```
{% endraw %}{% raw %}
<h2 id="jps">
  <a href="/zh/common/jps.html">jps</a> <a href="#jps"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示当前用户的 JVM 进程状态。
> 详细信息见：<https://docs.oracle.com/en/java/javase/11/tools/jps.html>.

#### 列出所有 JVM 进程：
```shell
jps
```
#### 列出所有 JVM 进程，只打印进程号：
```shell
jps -q
```
#### 显示传递给进程的参数：
```shell
jps -m
```
#### 显示所有进程的完整软件包名称：
```shell
jps -l
```
#### 显示传递给 JVM 的参数：
```shell
jps -v
```
{% endraw %}{% raw %}
<h2 id="make">
  <a href="/zh/common/make.html">make</a> <a href="#make"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Makefile 文件描述目标的任务运行器。
> 通常用于控制源代码中可执行文件的编译。
> 更多信息见：<https://www.gnu.org/software/make/manual/make.html>.

#### 调用 Makefile 中指定的第一个目标（通常命名为 "all"）：
```shell
make
```
#### 调用指定目标：
```shell
make {{目标}}
```
#### 调用一个指定的目标，一次并行执行4个作业：
```shell
make -j{{4}} {{目标}}
```
#### 使用指定的 Makefile 文件：
```shell
make --file {{文件}}
```
#### 从另一个目录执行 make ：
```shell
make --directory {{文件夹}}
```
#### 即使源文件未更改，也强制执行目标：
```shell
make --always-make {{目标}}
```
#### 覆盖在 Makefile 中定义的环境变量：
```shell
make --environment-overrides {{目标}}
```
{% endraw %}{% raw %}
<h2 id="matlab">
  <a href="/zh/common/matlab.html">matlab</a> <a href="#matlab"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> MathWorks 制作的数值计算环境。
> 更多信息: <https://uk.mathworks.com/help/matlab/>.

#### 在启动过程中，运行时不出现闪屏:
```shell
matlab -nosplash
```
#### 执行 MATLAB 语句:
```shell
matlab -r "{{matlab_语句}}"
```
#### 运行 MATLAB 脚本:
```shell
matlab -r "run({{路径/script.m}})"
```
{% endraw %}{% raw %}
<h2 id="md5sum">
  <a href="/zh/common/md5sum.html">md5sum</a> <a href="#md5sum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 计算 MD5 加密校验和.
> 更多信息： <https://www.gnu.org/software/coreutils/md5sum>.

#### 计算文件的 MD5 校验和:
```shell
md5sum {{filename1}}
```
#### 计算多个文件的 MD5 校验和:
```shell
md5sum {{filename1}} {{filename2}}
```
#### 读取 MD5SUM 的文件并验证所有文件是否具有匹配的校验和:
```shell
md5sum -c {{filename.md5}}
```
{% endraw %}{% raw %}
<h2 id="mongod">
  <a href="/zh/common/mongod.html">mongod</a> <a href="#mongod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> MongoDB 数据库服务器。
> 更多信息见：<https://docs.mongodb.com/manual/reference/program/mongod>.

#### 指定配置文件：
```shell
mongod --config {{filename}}
```
#### 指定要监听的端口：
```shell
mongod --port {{port}}
```
#### 指定数据库分析级别，用于性能调优分析。 0 - 关闭，1 - 仅是记录慢速操作，2 - 全部：
```shell
mongod --profile {{0|1|2}}
```
{% endraw %}{% raw %}
<h2 id="mpv">
  <a href="/zh/common/mpv.html">mpv</a> <a href="#mpv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一个基于 MPlayer 的音频/视频播放器.
> 更多信息: <https://mpv.io>.

#### 播放一个音频或视频文件:
```shell
mpv {{文件名}}
```
#### 往后/往前 跳跃5秒:
```shell
LEFT <or> RIGHT
```
#### 往后/往前 跳跃一分钟:
```shell
DOWN <or> UP
```
#### 减少/增加 10% 播放速度:
```shell
[ <or> ]
```
#### 以指定速度播放文件 (0.01 到 100, 默认是 1):
```shell
mpv --speed {{速度}} {{文件名}}
```
#### 用 `mpv.conf` 中指定的一个用户配制播放文件:
```shell
mpv --profile {{配制名称}} {{文件名}}
```
#### 播放摄像头或其他设备的输出:
```shell
mpv /dev/{{video0}}
```
{% endraw %}{% raw %}
<h2 id="mvn">
  <a href="/zh/common/mvn.html">mvn</a> <a href="#mvn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Apache Maven.
> 用于构建和管理基于 Java 的项目的工具。
> 更多信息见：<https://maven.apache.org>.

#### 编译项目：
```shell
mvn compile
```
#### 将编译后的代码打包成可分发格式，比如 `jar`：
```shell
mvn package
```
#### 编译和打包，跳过单元测试：
```shell
mvn package -Dmaven.test.skip=true
```
#### 在本地 maven 存储库中安装构建的包（这也会调用 compile 和 package 命令）：
```shell
mvn install
```
#### 从目标目录中删除构建工件，通常用来清理之前的编译结果：
```shell
mvn clean
```
#### 执行清理操作，然后进行编译打包：
```shell
mvn clean package
```
#### 执行清理操作并使用给定的构建配置打包代码，比如 `profileId` 如果有dev、test、pro，可以指定其中一个 `profileId` 用来选择具体执行环境：
```shell
mvn clean -P{{profileId}} package
```
#### 使用 main 方法运行一个类：
```shell
mvn exec:java -Dexec.mainClass="{{com.example.Main}}" -Dexec.args="{{参数1 参数2}}"
```
{% endraw %}{% raw %}
<h2 id="ninja">
  <a href="/zh/common/ninja.html">ninja</a> <a href="#ninja"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一个快速的构建系统.
> 更多信息: <https://ninja-build.org/manual.html>.

#### 在当前目录下构建:
```shell
ninja
```
#### 在指定的目录中构建一个程序:
```shell
ninja -C {{路径}}
```
#### 查看 target（如 `install` 和 `uninstall`):
```shell
ninja -t targets
```
#### 查看帮助:
```shell
ninja -h
```
{% endraw %}{% raw %}
<h2 id="nmap">
  <a href="/zh/common/nmap.html">nmap</a> <a href="#nmap"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 网络探索工具和安全/端口扫描程序。
> 仅当以特权运行 Nmap 时，某些功能才激活。
> 更多信息见: <https://nmap.org>.

#### 检查IP地址是否可用，并猜测远程主机的操作系统：
```shell
nmap -O {{IP 或者 主机名}}
```
#### 尝试确定指定的主机是否启动以及它们的名称是什么：
```shell
nmap -sn {{IP 或者 主机名}} {{可选的其它地址}}
```
#### 像上面一样，如果主机启动了，还可以运行默认的1000端口TCP扫描：
```shell
nmap {{IP 或者 主机名}} {{可选的其它地址}}
```
#### 也可以启用脚本，服务检测，操作系统指纹识别和跟踪路由：
```shell
nmap -A {{一个地址 或者 多个地址}}
```
#### 假设网络连接良好并加快执行速度：
```shell
nmap -T4 {{一个地址 或者 多个地址}}
```
#### 扫描端口的特定列表（使用 `-p` 参数覆盖所有端口，如 `-p 1-65535`，也可以明确指定几个端口，如 `-p 3306,3307,3308`）：
```shell
nmap -p {{端口1, 端口2, ..., 端口N}} {{一个地址 或者 多个地址}}
```
#### 执行 TCP 和 UDP 扫描（`-sU` 只用 UDP 扫描，`-sZ` 用 SCTP 扫描，`-sO` 用于 IP 扫描）：
```shell
nmap -sSU {{一个地址 或者 多个地址}}
```
#### 使用默认 NSE 脚本执行针对该主机地址的完整端口、服务、版本检测扫描，以确定弱点和信息：
```shell
nmap -sC -sV {{一个地址 或者 多个地址}}
```
{% endraw %}{% raw %}
<h2 id="node">
  <a href="/zh/common/node.html">node</a> <a href="#node"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 服务器后端 JavaScript 平台 (Node.js).
> 更多信息: <https://nodejs.org>.

#### 运行一个 JavaScript 文件:
```shell
node {{文件名}}
```
#### 开始一个 REPL 交互式解释器:
```shell
node
```
#### 执行输入的 JavaScript 代码:
```shell
node -e "{{代码}}"
```
#### 执行输入的 JavaScript 代码并显示结果:
```shell
node -p "{{代码}}"
```
#### 启动检查器并在程序源码解析完成后等待调试器连接:
```shell
node --no-lazy --inspect-brk {{文件名}}
```
{% endraw %}{% raw %}
<h2 id="rsync">
  <a href="/zh/common/rsync.html">rsync</a> <a href="#rsync"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 一种快速，通用，远程（和本地）文件复制工具。
> 更多信息：<https://man7.org/linux/man-pages/man1/rsync.1.html>。

#### 从本地传输文件到远程主机：
```shell
rsync {{path/to/local_file}} {{remote_host}}:{{path/to/remote_directory}}
```
#### 从远程主机传输文件到本地：
```shell
rsync {{remote_host}}:{{path/to/remote_file}} {{path/to/local_directory}}
```
#### 将本地文件以归档模式并保留几乎所有属性，同时使用压缩功能传输到远程主机，并以人类可读方式输出详细信息和进度条：
```shell
rsync --archive --compress --verbose --human-readable --progress {{path/to/local_file}} {{remote_host}}:{{path/to/remote_directory}}
```
#### 将远程主机目录上的所有文件，以递归模式传输到本地：
```shell
rsync --recursive {{remote_host}}:{{path/to/remote_directory}} {{path/to/local_directory}}
```
#### 将远程主机该目录下的所有内容（不包含该目录），以递归方式传输到本地：
```shell
rsync --recursive {{remote_host}}:{{path/to/remote_directory}}/ {{path/to/local_directory}}
```
#### 递归方式传输目录，保留几乎所有属性，解析软连接，并忽略已传输的文件：
```shell
rsync --recursive --archive --update --copy-links {{remote_host}}:{{path/to/remote_file}} {{path/to/local_directory}}
```
#### 指定本地和远程之间通信方式：
```shell
rsync --rsh ssh {{remote_host}}:{{path/to/remote_file}} {{path/to/local_file}}
```
#### 指定本地和远程之间通信方式，使用指定端口，并显示进度条：
```shell
rsync --rsh 'ssh -p {{port}}' --progress {{remote_host}}:{{path/to/remote_file}} {{path/to/local_file}}
```
{% endraw %}{% raw %}
<h2 id="runit">
  <a href="/zh/common/runit.html">runit</a> <a href="#runit"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 三级初始化系统.
> 更多信息： <https://wiki.archlinux.org/index.php/Runit>.

#### 启动 runit 的三阶段初始化方案:
```shell
runit
```
#### 停止运行 runit:
```shell
kill --CONT {{runit 进程 id}}
```
{% endraw %}{% raw %}
<h2 id="runsv">
  <a href="/zh/common/runsv.html">runsv</a> <a href="#runsv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 启动和管理 runit 服务.
> 更多信息： <https://manpages.ubuntu.com/manpages/latest/man8/runsv.8.html>.

#### 以当前用户身份启动 runit 服务:
```shell
runsv {{目录 / 服务文件}}
```
#### 以 root 用户身份启动 runit 服务:
```shell
sudo runsv {{目录 / 服务文件}}
```
{% endraw %}{% raw %}
<h2 id="runsvchdir">
  <a href="/zh/common/runsvchdir.html">runsvchdir</a> <a href="#runsvchdir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 更改默认使用的 `runsvdir` 目录.
> 更多信息： <https://manpages.ubuntu.com/manpages/latest/man8/runsvchdir.8.html>.

#### 切换 `runsvdir` 目录:
```shell
sudo runsvchdir {{指定 / 目录}}
```
{% endraw %}{% raw %}
<h2 id="runsvdir">
  <a href="/zh/common/runsvdir.html">runsvdir</a> <a href="#runsvdir"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 运行整个目录下的服务.
> 更多信息： <https://manpages.ubuntu.com/manpages/latest/man8/runsvdir.8.html>.

#### 以当前用户身份启动和管理目录中的所有服务:
```shell
runsvdir {{目录 / 服务文件}}
```
#### 以 root 用户身份启动和管理目录中的所有服务:
```shell
sudo runsvdir {{目录 / 服务文件}}
```
#### 在单独会话中启动服务:
```shell
runsvdir -P {{目录 / 服务文件}}
```
{% endraw %}{% raw %}
<h2 id="rustfmt">
  <a href="/zh/common/rustfmt.html">rustfmt</a> <a href="#rustfmt"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 格式化 Rust 源代码的工具.
> 更多信息: <https://github.com/rust-lang/rustfmt>.

#### 格式化文件，就地覆盖原始文件:
```shell
rustfmt {{source.rs}}
```
#### 检查文件的格式并在控制台上显示所有更改:
```shell
rustfmt --check {{source.rs}}
```
#### 格式化之前，备份所有修改过的文件(原始文件的扩展名为 `.bk`):
```shell
rustfmt --backup {{source.rs}}
```
{% endraw %}{% raw %}
<h2 id="shasum">
  <a href="/zh/common/shasum.html">shasum</a> <a href="#shasum"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 计算或检查加密 SHA 校验值.

#### 计算文件的 SHA1 校验值:
```shell
shasum {{文件名}}
```
#### 计算文件的 SHA256 校验值:
```shell
shasum --algorithm 256 {{文件名}}
```
#### 计算多个文件的 SHA512 校验值:
```shell
shasum --algorithm 512 {{文件名 1}} {{文件名 2}}
```
#### 计算一个文件内列出的所有的目录文件的相对应的总数:
```shell
shasum --check {{列表文件}}
```
#### 从标准输入中获取并计算 SHA1 校验值:
```shell
{{其他命令}} | shasum
```
{% endraw %}{% raw %}
<h2 id="stty">
  <a href="/zh/common/stty.html">stty</a> <a href="#stty"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 设置终端设备接口的选项.
> 更多信息： <https://www.gnu.org/software/coreutils/stty>.

#### 显示当前终端的所有设置:
```shell
stty -a
```
#### 设置行数:
```shell
stty rows {{行数}}
```
#### 设置列数:
```shell
stty cols {{列数}}
```
#### 获取设备的实际传输速度:
```shell
stty -F {{目标 / 文件夹 / 驱动设备文件}} speed
```
#### 将当前终端的所有模式重置为合理值:
```shell
stty sane
```
{% endraw %}{% raw %}
<h2 id="sv">
  <a href="/zh/common/sv.html">sv</a> <a href="#sv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 控制正在运行的服务.
> 更多信息： <https://manpages.ubuntu.com/manpages/latest/man8/sv.8.html>.

#### 启动服务:
```shell
sudo sv up {{目标目录 / 服务文件}}
```
#### 停止服务:
```shell
sudo sv down {{目标目录 / 服务文件}}
```
#### 获取服务状态:
```shell
sudo sv status {{目标目录 / 服务文件}}
```
{% endraw %}{% raw %}
<h2 id="tldr">
  <a href="/zh/common/tldr.html">tldr</a> <a href="#tldr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 简化过的 man 帮助手册.
> 更多信息：<https://tldr.sh>.

#### 获取一个命令的用例 （提示：这就是你怎么得到本信息的）:
```shell
tldr {{command}}
```
#### 展示 Linux 下 tar 的 tldr 文档:
```shell
tldr -p {{linux}} {{tar}}
```
#### 获取一个 Git 子命令的帮助:
```shell
tldr {{git checkout}}
```
#### 更新本地页面 (如果客户端支持缓存):
```shell
tldr -u
```
{% endraw %}{% raw %}
<h2 id="uname">
  <a href="/zh/common/uname.html">uname</a> <a href="#uname"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 输出关于当前机器和运行在该机器上的操作系统的详细信息。
> 注意：如需了解操作系统的其他信息，请尝试使用 `lsb_release` 命令。
> 更多信息： <https://www.gnu.org/software/coreutils/uname>.

#### 打印硬件相关信息：机器和处理器：
```shell
uname -mp
```
#### 打印软件相关信息：操作系统、发行号和版本：
```shell
uname -srv
```
#### 打印系统的名称（主机名）：
```shell
uname -n
```
#### 打印所有可用的系统信息（硬件、软件、名称）：
```shell
uname -a
```
{% endraw %}{% raw %}
<h2 id="units">
  <a href="/zh/common/units.html">units</a> <a href="#units"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 提供两个度量单位之间的转换.
> 更多信息： <https://www.gnu.org/software/units/>.

#### 以交互模式运行:
```shell
units
```
#### 显示两个简单单位之间的转换:
```shell
units {{quarts（夸脱）}} {{tablespoons（大汤匙）}}
```
#### 单位与数量之间的转换:
```shell
units "{{15 pounds（磅）}}" {{kilograms（公斤）}}
```
#### 显示两个复合单位之间的转换:
```shell
units "{{meters（米） / second（秒）}}" "{{inches（英尺） / hour（小时）}}"
```
#### 显示具有不同维度的单位之间的转换:
```shell
units "{{acres（英亩）}}" "{{ft（英尺）^2（平方）}}"
```
#### 显示字节乘数的转换:
```shell
units "{{15 megabytes（兆字节）}}" {{bytes（字节）}}
```
{% endraw %}{% raw %}
<h2 id="view">
  <a href="/zh/common/view.html">view</a> <a href="#view"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> `vim` 的只读版本.
> 等效于 `vim -R`.

#### 打开文件:
```shell
view {{file}}
```
{% endraw %}{% raw %}
<h2 id="vim">
  <a href="/zh/common/vim.html">vim</a> <a href="#vim"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Vi IMproved, 一个程序员的文本编辑器，提供为不同类型的文档修改设计的多种模式
> 在`vim`内使用任何命令时请确认未使用中文输入法，否则可能会出现奇怪的问题
> 按下`i`来进入编辑模式，`<esc>`回到标准模式 （不允许普通的字符输入）
> 更多信息：<https://www.vim.org>.

#### 打开文档:
```shell
vim {{file}}
```
#### 进入编辑模式 （插入模式）:
```shell
<Esc>i
```
#### 复制 ("yank") 或剪切 ("delete") 当前行 （使用`P`来粘贴）:
```shell
<Esc>{{yy|dd}}
```
#### 撤销上一个操作:
```shell
<Esc>u
```
#### 在文件中搜寻 （按下 `n`/`N` 来在上一个 / 下一个结果中切换）:
```shell
<Esc>/{{search_pattern}}<Enter>
```
#### 对整个文件使用正则表达式进行替换:
```shell
<Esc>:%s/{{pattern}}/{{replacement}}/g<Enter>
```
#### 保存 （写入） 文件，然后退出:
```shell
<Esc>:wq<Enter>
```
#### 不保存退出:
```shell
<Esc>:q!<Enter>
```
{% endraw %}{% raw %}
<h2 id="virtualenv">
  <a href="/zh/common/virtualenv.html">virtualenv</a> <a href="#virtualenv"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 创建被隔离的的 Python 虚拟环境.
> 更多信息：<https://virtualenv.pypa.io/>.

#### 创建新环境:
```shell
virtualenv {{path/to/venv}}
```
#### 自定义提示符:
```shell
virtualenv --prompt={{prompt_prefix}} {{path/to/venv}}
```
#### 为虚拟环境使用不同的 Python 版本:
```shell
virtualenv --python={{path/to/pythonbin}} {{path/to/venv}}
```
#### 启动 （选择） 环境:
```shell
source {{path/to/venv}}/bin/activate
```
#### 停止环境:
```shell
deactivate
```
{% endraw %}{% raw %}
<h2 id="vlc">
  <a href="/zh/common/vlc.html">vlc</a> <a href="#vlc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 跨平台多媒体播放器.
> 更多信息: <https://www.videolan.org/vlc/>.

#### 播放一个文件:
```shell
vlc {{文件名}}
```
#### 全屏播放:
```shell
vlc --fullscreen {{文件名}}
```
#### 静音播放:
```shell
vlc --no-audio {{文件名}}
```
#### 循环播放:
```shell
vlc --loop {{文件名}}
```
#### 播放网络连接:
```shell
vlc {{连接}}
```
{% endraw %}{% raw %}
<h2 id="vue-cli">
  <a href="/zh/common/vue.html">vue-cli</a> <a href="#vue-cli"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 用于初始化 Vue.js 项目的 CLI.
> 本帮助适用于旧的 `vue-cli@2` 和 `@vue/cli-init` 插件，新版 CLI 文档请参见更多信息
> 官方模板包括：webpack, webpack-simple, browserify, browserify-simple, simple.
> 更多信息：<https://cli.vuejs.org>.

#### 从模板创建新项目:
```shell
vue init {{template}} {{project_name}}
```
#### 从本地模板创建新项目:
```shell
vue init {{path/to/template_directory}} {{project_name}}
```
#### 从 GitHub 上拉取模板并创建新项目:
```shell
vue init {{username}}/{{repo}} {{project_name}}
```
{% endraw %}{% raw %}
<h2 id="w">
  <a href="/zh/common/w.html">w</a> <a href="#w"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 显示有哪些用户登录了本机以及他们当前的活动.
> 打印用户登录，TTY, 远程主机，登录时间，闲置时间，当前进程.

#### 获取已登录用户信息:
```shell
w
```
#### 无标题栏模式:
```shell
w -h
```
{% endraw %}{% raw %}
<h2 id="wget">
  <a href="/zh/common/wget.html">wget</a> <a href="#wget"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 从网络上下载文件.
> 支持 HTTP, HTTPS, 和 FTP.
> 更多信息：<https://www.gnu.org/software/wget>.

#### 将该 URL 的内容下载到文件中 （在这个例子中文件名为 "foo"）:
```shell
wget {{https://example.com/foo}}
```
#### 将该 URL 的内容下载到文件中 （在这个例子中文件名为 "bar"）:
```shell
wget --output-document {{bar}} {{https://example.com/foo}}
```
#### 以每三秒一个请求的速度下载一个网页和其所有资源 （脚本，样式表，图片等等）:
```shell
wget --page-requisites --convert-links --wait=3 {{https://example.com/somepage.html}}
```
#### 从一个目录中下载所有列出的文件和其所有子文件夹 （不下载内嵌网页）:
```shell
wget --mirror --no-parent {{https://example.com/somepath/}}
```
#### 限制下载速度和重试次数:
```shell
wget --limit-rate={{300k}} --tries={{100}} {{https://example.com/somepath/}}
```
#### 使用基本授权来从 HTTP/FTP 服务器中下载文件:
```shell
wget --user={{username}} --password={{password}} {{https://example.com}}
```
#### 继续一个未完成的下载任务:
```shell
wget --continue {{https://example.com}}
```
#### 将指定文件中所有列出的 URL 下载到一个目录中:
```shell
wget --directory-prefix {{path/to/directory}} --input-file {{URLs.txt}}
```
{% endraw %}{% raw %}
<h2 id="where">
  <a href="/zh/common/where.html">where</a> <a href="#where"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 报告所有已知的命令入口.
> 它可以是一个在`PATH`中的可执行文件，一个别名，或者一个 shell 內建命令.

#### 报告所有已知命令入口:
```shell
where {{command}}
```
{% endraw %}{% raw %}
<h2 id="which">
  <a href="/zh/common/which.html">which</a> <a href="#which"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 在用户的`PATH`中寻找可执行文件的路径

#### 在`PATH`中寻找可执行文件并打印第一个匹配的结果:
```shell
which {{executable}}
```
#### 如果有多个匹配结果则打印所有结果:
```shell
which -a {{executable}}
```
{% endraw %}{% raw %}
<h2 id="write">
  <a href="/zh/common/write.html">write</a> <a href="#write"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 向某个终端上的特定用户的屏幕写入信息 （Ctrl-C 来停止写入）.
> 使用 `who` 命令来获取所有活动用户的终端 id. 参见 `mesg`.

#### 向指定的终端 ID 上的指定用户写入信息:
```shell
write {{username}} {{terminal_id}}
```
#### 向终端 "/dev/tty/5" 上的用户 "testuser" 发送信息:
```shell
write {{testuser}} {{tty/5}}
```
#### 向伪终端 "/dev/pts/5" 上的用户 "johndoe" 发送信息 :
```shell
write {{johndoe}} {{pts/5}}
```
{% endraw %}{% raw %}
<h2 id="yarn-why">
  <a href="/zh/common/yarn-why.html">yarn-why</a> <a href="#yarn-why"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 确认安装这个 Yarn 软件包的原因.
> 更多信息：<https://www.npmjs.com/package/yarn-why>.

#### 打印安装这个 Yarn 软件包的原因:
```shell
yarn-why {{package_name}}
```
{% endraw %}{% raw %}
<h2 id="yarn">
  <a href="/zh/common/yarn.html">yarn</a> <a href="#yarn"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> JavaScript 和 Node.js package manager 的一个替代.
> 更多信息：<https://yarnpkg.com>.

#### 全局安装一个模块:
```shell
yarn global add {{module_name}}
```
#### 安装 `package.json` 中指定的依赖 (`install` 命令是可选的 -- 你可以直接输入`yarn`):
```shell
yarn install
```
#### 安装一个模块并将其写入 `package.json` 中的依赖项 （增加 `--dev` 来作为开发依赖写入）:
```shell
yarn add {{module_name}}@{{version}}
```
#### 卸载一个模块并将其从 `package.json` 的依赖项中移除:
```shell
yarn remove {{module_name}}
```
#### 交互式地创建一个 `package.json` 文件:
```shell
yarn init
```
#### 确认一个模块是否是一个依赖项并且列出依赖其的模块:
```shell
yarn why {{module_name}}
```
{% endraw %}{% raw %}
<h2 id="z">
  <a href="/zh/common/z.html">z</a> <a href="#z"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 记录被使用次数最多的目录并允许在它们之间以字符串或正则表达式来进行匹配和跳转.
> 更多信息：<https://github.com/rupa/z>.

#### 跳转到一个名字带有 "foo" 的文件夹:
```shell
z {{foo}}
```
#### 跳转到一个名字带有 "foo" 并且后面带有 "bar" 的文件夹（例：`fooesbar`):
```shell
z {{foo}} {{bar}}
```
#### 跳转到名字带有 "foo" 并且拥有最高访问次数的文件夹:
```shell
z -r {{foo}}
```
#### 跳转到最近使用的名字带有 "foo" 的文件夹:
```shell
z -t {{foo}}
```
#### 列出在 `z` 的数据库中名字带有 "foo" 的文件夹:
```shell
z -l {{foo}}
```
#### 将当前文件夹从 `z`的数据库中移除:
```shell
z -x .
```
{% endraw %}{% raw %}
<h2 id="zsh">
  <a href="/zh/common/zsh.html">zsh</a> <a href="#zsh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Z SHell.
> 与 `bash` 和 `sh` 兼容的命令行解释器.
> 更多信息：<https://www.zsh.org>.

#### 启动交互式解释器:
```shell
zsh
```
#### 执行从参数传入的命令:
```shell
zsh -c {{command}}
```
#### 从文件执行命令 （脚本）:
```shell
zsh {{file}}
```
#### 从文件执行命令并将执行过的命令打印到终端:
```shell
zsh -x {{file}}
```
{% endraw %}{% raw %}
<h2 id="zstd">
  <a href="/zh/common/zstd.html">zstd</a> <a href="#zstd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> 使用 Zstandard 压缩来压缩 / 解压文件.
> 更多信息：<https://github.com/facebook/zstd>.

#### 将一个文件压缩到一个 `.zst` 后缀的压缩文件中:
```shell
zstd {{file}}
```
#### 解压缩一个文件:
```shell
zstd -d {{file}}.zst
```
#### 将文件解压缩到标准输出 (stdout):
```shell
zstd -dc {{file}}.zst
```
#### 使用指定的压缩等级来压缩一个文件.0 = 最差，19 = 最好 （默认等级是 3):
```shell
zstd -{{level}} {{file}}
```
#### 使用更多内存 （解压或压缩时） 来得到更高的压缩比:
```shell
zstd --ultra -{{level}} {{file}}
```
{% endraw %}