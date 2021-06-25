---
layout: default
title: "osx"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#getfileinfo">GetFileInfo</a>
* <a href="#safeejectgpu">SafeEjectGPU</a>
* <a href="#afinfo">afinfo</a>
* <a href="#afplay">afplay</a>
* <a href="#airport">airport</a>
* <a href="#apachectl">apachectl</a>
* <a href="#arch">arch</a>
* <a href="#archey">archey</a>
* <a href="#as">as</a>
* <a href="#asr">asr</a>
* <a href="#base64">base64</a>
* <a href="#bless">bless</a>
* <a href="#brew-bundle">brew bundle</a>
* <a href="#brew-cask">brew cask</a>
* <a href="#brightness">brightness</a>
* <a href="#caffeinate">caffeinate</a>
* <a href="#cal">cal</a>
* <a href="#carthage">carthage</a>
* <a href="#chflags">chflags</a>
* <a href="#codesign">codesign</a>
* <a href="#compgen">compgen</a>
* <a href="#csshx">csshX</a>
* <a href="#dark-mode">dark-mode</a>
* <a href="#date">date</a>
* <a href="#dd">dd</a>
* <a href="#defaults">defaults</a>
* <a href="#diskutil">diskutil</a>
* <a href="#ditto">ditto</a>
* <a href="#dmesg">dmesg</a>
* <a href="#dot_clean">dot_clean</a>
* <a href="#drutil">drutil</a>
* <a href="#du">du</a>
* <a href="#duti">duti</a>
* <a href="#eval">eval</a>
* <a href="#export">export</a>
* <a href="#fc">fc</a>
* <a href="#fdesetup">fdesetup</a>
* <a href="#feh">feh</a>
* <a href="#file">file</a>
* <a href="#fileicon">fileicon</a>
* <a href="#fsck">fsck</a>
* <a href="#hdiutil">hdiutil</a>
* <a href="#head">head</a>
* <a href="#hexdump">hexdump</a>
* <a href="#hostname">hostname</a>
* <a href="#icalbuddy">icalBuddy</a>
* <a href="#imgcat">imgcat</a>
* <a href="#indent">indent</a>
* <a href="#istats">istats</a>
* <a href="#launchctl">launchctl</a>
* <a href="#lldb">lldb</a>
* <a href="#locate">locate</a>
* <a href="#logger">logger</a>
* <a href="#look">look</a>
* <a href="#m">m</a>
* <a href="#mas">mas</a>
* <a href="#md5">md5</a>
* <a href="#mdfind">mdfind</a>
* <a href="#mdls">mdls</a>
* <a href="#mdutil">mdutil</a>
* <a href="#mkfile">mkfile</a>
* <a href="#n">n</a>
* <a href="#netstat">netstat</a>
* <a href="#networksetup">networksetup</a>
* <a href="#nm">nm</a>
* <a href="#oathtool">oathtool</a>
* <a href="#open">open</a>
* <a href="#opensnoop">opensnoop</a>
* <a href="#osascript">osascript</a>
* <a href="#pbcopy">pbcopy</a>
* <a href="#pbpaste">pbpaste</a>
* <a href="#pdfgrep">pdfgrep</a>
* <a href="#ping">ping</a>
* <a href="#pkgutil">pkgutil</a>
* <a href="#plutil">plutil</a>
* <a href="#pmset">pmset</a>
* <a href="#pod">pod</a>
* <a href="#port">port</a>
* <a href="#pwgen">pwgen</a>
* <a href="#qlmanage">qlmanage</a>
* <a href="#readlink">readlink</a>
* <a href="#reboot">reboot</a>
* <a href="#rename">rename</a>
* <a href="#route">route</a>
* <a href="#rubocop">rubocop</a>
* <a href="#say">say</a>
* <a href="#screencapture">screencapture</a>
* <a href="#scutil">scutil</a>
* <a href="#security">security</a>
* <a href="#sed">sed</a>
* <a href="#shuf">shuf</a>
* <a href="#shutdown">shutdown</a>
* <a href="#sips">sips</a>
* <a href="#softwareupdate">softwareupdate</a>
* <a href="#split">split</a>
* <a href="#spotify">spotify</a>
* <a href="#ssh-add">ssh-add</a>
* <a href="#sshuttle">sshuttle</a>
* <a href="#stat">stat</a>
* <a href="#sw_vers">sw_vers</a>
* <a href="#sysctl">sysctl</a>
* <a href="#system_profiler">system_profiler</a>
* <a href="#systemsetup">systemsetup</a>
* <a href="#textutil">textutil</a>
* <a href="#tmutil">tmutil</a>
* <a href="#top">top</a>
* <a href="#trap">trap</a>
* <a href="#tree">tree</a>
* <a href="#uname">uname</a>
* <a href="#uptime">uptime</a>
* <a href="#uuidgen">uuidgen</a>
* <a href="#valet">valet</a>
* <a href="#w">w</a>
* <a href="#wacaw">wacaw</a>
* <a href="#whatis">whatis</a>
* <a href="#whence">whence</a>
* <a href="#whereis">whereis</a>
* <a href="#wifi-password">wifi-password</a>
* <a href="#xar">xar</a>
* <a href="#xattr">xattr</a>
* <a href="#xcode-select">xcode-select</a>
* <a href="#xcodebuild">xcodebuild</a>
* <a href="#xctool">xctool</a>
* <a href="#xed">xed</a>
* <a href="#xip">xip</a>
* <a href="#xsltproc">xsltproc</a>
* <a href="#yaa">yaa</a>
* <a href="#yabai">yabai</a>
* <a href="#yank">yank</a>

{% raw %}
<h2 id="afinfo">
  <a href="/en/osx/afinfo.html">afinfo</a> <a href="#afinfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Audio file metadata parser for OS X.
> Built-in command of OS X.

#### Display info of a given audio file:
```shell
afinfo {{path/to/file}}
```
#### Print a one line description of the audio file:
```shell
afinfo -b {{path/to/file}}
```
#### Print metadata info and contents of the audio file's InfoDictionary:
```shell
afinfo -i {{path/to/file}}
```
#### Print output in xml format:
```shell
afinfo -x {{path/to/file}}
```
#### Print warnings for the audio file if any:
```shell
afinfo --warnings {{path/to/file}}
```
#### Display help for full usage:
```shell
afinfo -h
```
{% endraw %}{% raw %}
<h2 id="afplay">
  <a href="/en/osx/afplay.html">afplay</a> <a href="#afplay"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line audio player.

#### Play a sound file (waits until playback ends):
```shell
afplay {{path/to/file}}
```
#### Play a sound file at 2x speed (playback rate):
```shell
afplay --rate {{2}} {{path/to/file}}
```
#### Play a sound file at half speed:
```shell
afplay --rate {{0.5}} {{path/to/file}}
```
#### Play the first N seconds of a sound file:
```shell
afplay --time {{seconds}} {{path/to/file}}
```
{% endraw %}{% raw %}
<h2 id="airport">
  <a href="/en/osx/airport.html">airport</a> <a href="#airport"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Wireless network configuration utility.

#### Show current wireless status information:
```shell
airport -I
```
#### Sniff wireless traffic on channel 1:
```shell
airport sniff {{1}}
```
#### Scan for available wireless networks:
```shell
airport -s
```
#### Disassociate from current airport network:
```shell
sudo airport -z
```
{% endraw %}{% raw %}
<h2 id="apachectl">
  <a href="/en/osx/apachectl.html">apachectl</a> <a href="#apachectl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Apache HTTP Server control interface for macOS.

#### Start the `org.apache.httpd` launchd job:
```shell
apachectl start
```
#### Stop the launchd job:
```shell
apachectl stop
```
#### Stop, then start launchd job:
```shell
apachectl restart
```
{% endraw %}{% raw %}
<h2 id="arch">
  <a href="/en/osx/arch.html">arch</a> <a href="#arch"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display the name of the system architecture, or run a command under a different architecture.
> See also `uname`.

#### Display the system's architecture:
```shell
arch
```
#### Run a command using x86_64:
```shell
arch -x86_64 {{command}}
```
{% endraw %}{% raw %}
<h2 id="archey">
  <a href="/en/osx/archey.html">archey</a> <a href="#archey"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Simple tool for stylishly displaying system information.

#### Show system information:
```shell
archey
```
#### Show system information without colored output:
```shell
archey --nocolor
```
#### Show system information, using MacPorts instead of Homebrew:
```shell
archey --macports
```
#### Show system information without IP address check:
```shell
archey --offline
```
{% endraw %}{% raw %}
<h2 id="as">
  <a href="/en/osx/as.html">as</a> <a href="#as"><svg class="icon">
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
<h2 id="asr">
  <a href="/en/osx/asr.html">asr</a> <a href="#asr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Restore (copy) a disk image onto a volume.
> The command name stands for Apple Software Restore.

#### Restore a disk image to a target volume:
```shell
sudo asr restore --source {{image_name}}.dmg --target {{path/to/volume}}
```
#### Erase the target volume before restoring:
```shell
sudo asr restore --source {{image_name}}.dmg --target {{path/to/volume}} --erase
```
#### Skip verification after restoring:
```shell
sudo asr restore --source {{image_name}}.dmg --target {{path/to/volume}} --noverify
```
#### Clone volumes without the use of an intermediate disk image:
```shell
sudo asr restore --source {{path/to/volume}} --target {{path/to/cloned_volume}}
```
{% endraw %}{% raw %}
<h2 id="base64">
  <a href="/en/osx/base64.html">base64</a> <a href="#base64"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Encode and decode using Base64 representation.

#### Encode a file:
```shell
base64 --input={{plain_file}}
```
#### Decode a file:
```shell
base64 --decode --input={{base64_file}}
```
#### Encode from stdin:
```shell
echo -n {{plain_text}} | base64
```
#### Decode from stdin:
```shell
echo -n {{base64_text}} | base64 --decode
```
{% endraw %}{% raw %}
<h2 id="bless">
  <a href="/en/osx/bless.html">bless</a> <a href="#bless"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Set volume boot capability and startup disk options.
> More information: <https://ss64.com/osx/bless.html>.

#### Bless a volume with only Mac OS X or Darwin, and create the BootX and `boot.efi` files as needed:
```shell
bless --folder "{{/Volumes/Mac OS X/System/Library/CoreServices}}" --bootinfo --bootefi
```
#### Set a volume containing either Mac OS 9 and Mac OS X to be the active volume:
```shell
bless --mount "{{/Volumes/Mac OS}}" --setBoot
```
#### Set the system to NetBoot and broadcast for an available server:
```shell
bless --netboot --server {{bsdp://255.255.255.255}}
```
#### Gather information about the currently selected volume (as determined by the firmware), suitable for piping to a program capable of parsing Property Lists:
```shell
bless --info --plist
```
{% endraw %}{% raw %}
<h2 id="brew-bundle">
  <a href="/en/osx/brew-bundle.html">brew bundle</a> <a href="#brew-bundle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Bundler for Homebrew, Homebrew Cask and the Mac App Store.
> More information: <https://github.com/Homebrew/homebrew-bundle>.

#### Install packages from a Brewfile at the current path:
```shell
brew bundle
```
#### Install packages from a specific Brewfile at a specific path:
```shell
brew bundle --file={{path/to/file}}
```
#### Create a Brewfile from all installed packages:
```shell
brew bundle dump
```
#### Uninstall all formulae not listed in the Brewfile:
```shell
brew bundle cleanup --force
```
#### Check if there is anything to install or upgrade in the Brewfile:
```shell
brew bundle check
```
#### Output a list of all entries in the Brewfile:
```shell
brew bundle list --all
```
{% endraw %}{% raw %}
<h2 id="brew-cask">
  <a href="/en/osx/brew-cask.html">brew cask</a> <a href="#brew-cask"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Package manager for macOS applications distributed as binaries.
> More information: <https://github.com/Homebrew/homebrew-cask>.

#### Search for formulas and casks:
```shell
brew search {{text}}
```
#### Install a cask:
```shell
brew cask install {{cask_name}}
```
#### List all installed casks:
```shell
brew list --cask
```
#### List installed casks that have newer versions available:
```shell
brew outdated --cask
```
#### Upgrade an installed cask (if no cask name is given, all installed casks are upgraded):
```shell
brew upgrade --cask {{cask_name}}
```
#### Uninstall a cask:
```shell
brew cask uninstall {{cask_name}}
```
#### Uninstall a cask and remove related settings and files:
```shell
brew cask zap {{cask_name}}
```
#### Display information about a given cask:
```shell
brew cask info {{cask_name}}
```
{% endraw %}{% raw %}
<h2 id="brightness">
  <a href="/en/osx/brightness.html">brightness</a> <a href="#brightness"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Get and set the brightness level of all internal and certain external displays.

#### Show current brightness:
```shell
brightness -l
```
#### Set the brightness to 100%::
```shell
brightness {{1}}
```
#### Set the brightness to 50%::
```shell
brightness {{0.5}}
```
{% endraw %}{% raw %}
<h2 id="caffeinate">
  <a href="/en/osx/caffeinate.html">caffeinate</a> <a href="#caffeinate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Prevent mac from sleeping.

#### Prevent from sleeping for 1 hour (3600 seconds):
```shell
caffeinate -u -t {{3600}}
```
#### Prevent from sleeping until a command completes:
```shell
caffeinate -s {{command}}
```
#### Prevent from sleeping until you type Ctrl-C:
```shell
caffeinate -i
```
{% endraw %}{% raw %}
<h2 id="cal">
  <a href="/en/osx/cal.html">cal</a> <a href="#cal"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Prints calendar information.

#### Display a calendar for the current month:
```shell
cal
```
#### Display previous, current and next month:
```shell
cal -3
```
#### Display a calendar for a specific month (1-12 or name):
```shell
cal -m {{month}}
```
#### Display a calendar for the current year:
```shell
cal -y
```
#### Display a calendar for a specific year (4 digits):
```shell
cal {{year}}
```
#### Display a calendar for a specific month and year:
```shell
cal {{month}} {{year}}
```
#### Display date of Easter (Western Christian churches) in a given year:
```shell
ncal -e {{year}}
```
{% endraw %}{% raw %}
<h2 id="carthage">
  <a href="/en/osx/carthage.html">carthage</a> <a href="#carthage"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A dependency management tool for Cocoa applications.

#### Download the latest version of all dependencies mentioned in Cartfile, and build them:
```shell
carthage update
```
#### Update dependencies, but only build for iOS:
```shell
carthage update --platform ios
```
#### Update dependencies, but don't build any of them:
```shell
carthage update --no-build
```
#### Download and rebuild the current version of dependencies (without updating them):
```shell
carthage bootstrap
```
#### Rebuild a specific dependency:
```shell
carthage build {{dependency}}
```
{% endraw %}{% raw %}
<h2 id="chflags">
  <a href="/en/osx/chflags.html">chflags</a> <a href="#chflags"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Change file or directory flags.

#### Set the `hidden` flag for a file:
```shell
chflags {{hidden}} {{path/to/file}}
```
#### Unset the `hidden` flag for a file:
```shell
chflags {{nohidden}} {{path/to/file}}
```
#### Recursively set the `uchg` flag for a directory:
```shell
chflags -R {{uchg}} {{path/to/directory}}
```
#### Recursively unset the `uchg` flag for a directory:
```shell
chflags -R {{nouchg}} {{path/to/directory}}
```
{% endraw %}{% raw %}
<h2 id="codesign">
  <a href="/en/osx/codesign.html">codesign</a> <a href="#codesign"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create and manipulate code signatures for macOS.

#### Sign an application with a certificate:
```shell
codesign -s "{{My Company Name}}" {{path/to/App.app}}
```
#### Verify the certificate of an application:
```shell
codesign -v {{path/to/App.app}}
```
{% endraw %}{% raw %}
<h2 id="compgen">
  <a href="/en/osx/compgen.html">compgen</a> <a href="#compgen"><svg class="icon">
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
<h2 id="csshx">
  <a href="/en/osx/csshx.html">csshX</a> <a href="#csshx"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cluster SSH tool for macOS.
> More information: <https://github.com/brockgr/csshx>.

#### Connect to multiple hosts:
```shell
csshX {{hostname1}} {{hostname2}}
```
#### Connect to multiple hosts with a given SSH key:
```shell
csshX {{user@hostname1}} {{user@hostname2}} '--ssh_args' '-i {{path/to/ssh_key.pem}}'
```
#### Connect to a pre-defined cluster from `/etc/clusters`:
```shell
csshX cluster1
```
{% endraw %}{% raw %}
<h2 id="dark-mode">
  <a href="/en/osx/dark-mode.html">dark-mode</a> <a href="#dark-mode"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Control macOS dark mode from the command-line.
> More information: <https://github.com/sindresorhus/dark-mode>.

#### Toggle dark mode (turn it on if it's currently off, off if it's currently on):
```shell
dark-mode
```
#### Turn dark mode on:
```shell
dark-mode on
```
#### Turn dark mode off:
```shell
dark-mode off
```
#### Check if dark mode is on:
```shell
dark-mode status
```
{% endraw %}{% raw %}
<h2 id="date">
  <a href="/en/osx/date.html">date</a> <a href="#date"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Set or display the system date.

#### Display the current date using the default locale's format:
```shell
date +"%c"
```
#### Display the current date in UTC and ISO 8601 format:
```shell
date -u +"%Y-%m-%dT%H:%M:%SZ"
```
#### Display the current date as a Unix timestamp (seconds since the Unix epoch):
```shell
date +%s
```
#### Display a specific date (represented as a Unix timestamp) using the default format:
```shell
date -r 1473305798
```
{% endraw %}{% raw %}
<h2 id="dd">
  <a href="/en/osx/dd.html">dd</a> <a href="#dd"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Convert and copy a file.

#### Make a bootable usb drive from an isohybrid file (such like `archlinux-xxx.iso`):
```shell
dd if={{file.iso}} of=/dev/{{usb_drive}}
```
#### Clone a drive to another drive with 4MB block and ignore error:
```shell
dd if=/dev/{{source_drive}} of=/dev/{{dest_drive}} bs=4m conv=noerror
```
#### Generate a file of 100 random bytes by using kernel random driver:
```shell
dd if=/dev/urandom of={{random_file}} bs=100 count=1
```
#### Benchmark the write performance of a disk:
```shell
dd if=/dev/zero of={{file_1GB}} bs=1024 count=1000000
```
{% endraw %}{% raw %}
<h2 id="defaults">
  <a href="/en/osx/defaults.html">defaults</a> <a href="#defaults"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Read and write macOS user configuration for applications.
> More information: <https://ss64.com/osx/defaults.html>.

#### Read system defaults for an application option:
```shell
defaults read {{application}} {{option}}
```
#### Read default values for an application option:
```shell
defaults read -app {{application}} {{option}}
```
#### Search for a keyword in domain names, keys, and values:
```shell
defaults find {{keyword}}
```
#### Write the default value of an application option:
```shell
defaults write {{application}} {{option}} {{-type}} {{value}}
```
#### Speed up Mission Control animations:
```shell
defaults write com.apple.Dock expose-animation-duration -float 0.1
```
#### Delete all defaults of an application:
```shell
defaults delete {{application}}
```
{% endraw %}{% raw %}
<h2 id="diskutil">
  <a href="/en/osx/diskutil.html">diskutil</a> <a href="#diskutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility to manage local disks and volumes.

#### List all currently available disks, partitions and mounted volumes:
```shell
diskutil list
```
#### Repair the filesystem data structures of a volume:
```shell
diskutil repairVolume {{/dev/diskX}}
```
#### Unmount a volume:
```shell
diskutil unmountDisk {{/dev/diskX}}
```
#### Eject a CD/DVD (unmount first):
```shell
diskutil eject {{/dev/disk1}}
```
{% endraw %}{% raw %}
<h2 id="ditto">
  <a href="/en/osx/ditto.html">ditto</a> <a href="#ditto"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Copy files and directories.

#### Overwrite contents of destination directory with contents of source directory:
```shell
ditto {{path/to/source}} {{path/to/destination}}
```
#### Print a line to the Terminal window for every file that's being copied:
```shell
ditto -V {{path/to/source}} {{path/to/destination}}
```
#### Copy a given file or directory, while retaining the original file permissions:
```shell
ditto -rsrc {{path/to/source}} {{path/to/destination}}
```
{% endraw %}{% raw %}
<h2 id="dmesg">
  <a href="/en/osx/dmesg.html">dmesg</a> <a href="#dmesg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Write the kernel messages to standard output.

#### Show kernel messages:
```shell
dmesg
```
#### Show how much physical memory is available on this system:
```shell
dmesg | grep -i memory
```
#### Show kernel messages 1 page at a time:
```shell
dmesg | less
```
{% endraw %}{% raw %}
<h2 id="dot_clean">
  <a href="/en/osx/dot_clean.html">dot_clean</a> <a href="#dot_clean"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Merge ._* files with corresponding native files.
> More information: <https://ss64.com/osx/dot_clean.html>.

#### Merge all `._*` files recursively:
```shell
dot_clean {{path/to/directory}}
```
#### Don't recursively merge all `._*` in a directory (flat merge):
```shell
dot_clean -f {{path/to/directory}}
```
#### Merge and delete all `._*` files:
```shell
dot_clean -m {{path/to/directory}}
```
#### Only delete `._*` files if there's a matching native file:
```shell
dot_clean -n {{path/to/directory}}
```
#### Follow symlinks:
```shell
dot_clean -s {{path/to/directory}}
```
#### Print verbose output:
```shell
dot_clean -v {{path/to/directory}}
```
{% endraw %}{% raw %}
<h2 id="drutil">
  <a href="/en/osx/drutil.html">drutil</a> <a href="#drutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Interact with DVD burners.

#### Eject a disk from the drive:
```shell
drutil eject
```
#### Burn a directory as an ISO9660 filesystem onto a DVD. Don't verify and eject when complete:
```shell
drutil burn -noverify -eject -iso9660
```
{% endraw %}{% raw %}
<h2 id="du">
  <a href="/en/osx/du.html">du</a> <a href="#du"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Disk usage: estimate and summarize file and directory space usage.

#### List the sizes of a directory and any subdirectories, in the given unit (KB/MB/GB):
```shell
du -{{k|m|g}} {{path/to/directory}}
```
#### List the sizes of a directory and any subdirectories, in human-readable form (i.e. auto-selecting the appropriate unit for each size):
```shell
du -h {{path/to/directory}}
```
#### Show the size of a single directory, in human readable units:
```shell
du -sh {{path/to/directory}}
```
#### List the human-readable sizes of a directory and of all the files and directories within it:
```shell
du -ah {{path/to/directory}}
```
#### List the human-readable sizes of a directory and any subdirectories, up to N levels deep:
```shell
du -h -d {{N}} {{path/to/directory}}
```
#### List the human-readable size of all `.jpg` files in subdirectories of the current directory, and show a cumulative total at the end:
```shell
du -ch */*.jpg
```
{% endraw %}{% raw %}
<h2 id="duti">
  <a href="/en/osx/duti.html">duti</a> <a href="#duti"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Set default applications for document types and URL schemes on macOS.

#### Set Safari as the default handler for HTML documents:
```shell
duti -s {{com.apple.Safari}} {{public.html}} all
```
#### Set VLC as the default viewer for files with `.m4v` extensions:
```shell
duti -s {{org.videolan.vlc}} {{m4v}} viewer
```
#### Set Finder as the default handler for the ftp:// URL scheme:
```shell
duti -s {{com.apple.Finder}} {{ftp}}
```
#### Display information about the default application for a given extension:
```shell
duti -x {{ext}}
```
#### Display the default handler for a given UTI:
```shell
duti -d {{uti}}
```
#### Display all handlers of a given UTI:
```shell
duti -l {{uti}}
```
{% endraw %}{% raw %}
<h2 id="eval">
  <a href="/en/osx/eval.html">eval</a> <a href="#eval"><svg class="icon">
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
<h2 id="export">
  <a href="/en/osx/export.html">export</a> <a href="#export"><svg class="icon">
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
#### Append something to the PATH variable:
```shell
export PATH=$PATH:{{path/to/append}}
```
{% endraw %}{% raw %}
<h2 id="fc">
  <a href="/en/osx/fc.html">fc</a> <a href="#fc"><svg class="icon">
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
<h2 id="fdesetup">
  <a href="/en/osx/fdesetup.html">fdesetup</a> <a href="#fdesetup"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Set and retrieve FileVault related information.

#### List current FileVault enabled users:
```shell
sudo fdesetup list
```
#### Get current FileVault status:
```shell
fdesetup status
```
#### Add FileVault enabled user:
```shell
sudo fdesetup add -usertoadd user1
```
#### Enable FileVault:
```shell
sudo fdesetup enable
```
#### Disable FileVault:
```shell
sudo fdesetup disable
```
{% endraw %}{% raw %}
<h2 id="feh">
  <a href="/en/osx/feh.html">feh</a> <a href="#feh"><svg class="icon">
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
{% endraw %}{% raw %}
<h2 id="file">
  <a href="/en/osx/file.html">file</a> <a href="#file"><svg class="icon">
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
file -I {{filename}}
```
{% endraw %}{% raw %}
<h2 id="fileicon">
  <a href="/en/osx/fileicon.html">fileicon</a> <a href="#fileicon"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A macOS CLI to manage custom file and folder icons.
> More information: <https://github.com/mklement0/fileicon>.

#### Set a custom icon for a specific file or directory:
```shell
fileicon set {{path/to/file_or_directory}} {{path/to/icon.png}}
```
#### Remove a custom icon from a specific file or directory:
```shell
fileicon rm {{path/to/file_or_directory}}
```
#### Save the custom icon of a file or directory as a `.icns` file into the current directory:
```shell
fileicon get {{path/to/file_or_directory}}
```
#### Test if a specific file or directory has a custom icon:
```shell
fileicon test {{path/to/file_or_directory}}
```
{% endraw %}{% raw %}
<h2 id="fsck">
  <a href="/en/osx/fsck.html">fsck</a> <a href="#fsck"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Check the integrity of a filesystem or repair it. The filesystem should be unmounted at the time the command is run.
> It is a wrapper that calls `fsck_hfs`, `fsck_apfs`, `fsck_msdos`, `fsck_exfat`, and `fsck_udf` as needed.

#### Check filesystem `/dev/sdX`, reporting any damaged blocks:
```shell
fsck {{/dev/sdX}}
```
#### Check filesystem `/dev/sdX` only if it is clean, reporting any damaged blocks and interactively letting the user choose to repair each one:
```shell
fsck -f {{/dev/sdX}}
```
#### Check filesystem `/dev/sdX` only if it is clean, reporting any damaged blocks and automatically repairing them:
```shell
fsck -fy {{/dev/sdX}}
```
#### Check filesystem `/dev/sdX`, reporting whether it has been cleanly unmounted:
```shell
fsck -q {{/dev/sdX}}
```
{% endraw %}{% raw %}
<h2 id="getfileinfo">
  <a href="/en/osx/getfileinfo.html">GetFileInfo</a> <a href="#getfileinfo"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Get information about a file in an HFS+ directory.

#### Display information about a given file:
```shell
GetFileInfo {{path/to/filename}}
```
#### Display the date and time a given file was created:
```shell
GetFileInfo -d {{path/to/filename}}
```
#### Display the date and time a given file was last modified:
```shell
GetFileInfo -m {{path/to/filename}}
```
#### Display the creator of a given file:
```shell
GetFileInfo -c {{path/to/filename}}
```
{% endraw %}{% raw %}
<h2 id="hdiutil">
  <a href="/en/osx/hdiutil.html">hdiutil</a> <a href="#hdiutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility to create and manage disk images.

#### Mount an image:
```shell
hdiutil attach {{path/to/image_file}}
```
#### Unmount an image:
```shell
hdiutil detach /Volumes/{{volume_name}}
```
#### List mounted images:
```shell
hdiutil info
```
#### Create an ISO image from the contents of a directory:
```shell
hdiutil makehybrid -o {{path/to/output_file}} {{path/to/directory}}
```
{% endraw %}{% raw %}
<h2 id="head">
  <a href="/en/osx/head.html">head</a> <a href="#head"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Output the first part of files.

#### Output the first few lines of a file:
```shell
head -n {{count_of_lines}} {{filename}}
```
#### Output the first few bytes of a file:
```shell
head -c {{number_in_bytes}} {{filename}}
```
{% endraw %}{% raw %}
<h2 id="hexdump">
  <a href="/en/osx/hexdump.html">hexdump</a> <a href="#hexdump"><svg class="icon">
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
<h2 id="hostname">
  <a href="/en/osx/hostname.html">hostname</a> <a href="#hostname"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show or set the system's host name.

#### Show current host name:
```shell
hostname
```
#### Set current host name:
```shell
hostname {{new_hostname}}
```
{% endraw %}{% raw %}
<h2 id="icalbuddy">
  <a href="/en/osx/icalbuddy.html">icalBuddy</a> <a href="#icalbuddy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line utility for printing events and tasks from the macOS calendar database.
> More information: <https://hasseg.org/icalBuddy/>.

#### Show events later today:
```shell
icalBuddy -n eventsToday
```
#### Show uncompleted tasks:
```shell
icalBuddy uncompletedTasks
```
#### Show a formatted list separated by calendar for all events today:
```shell
icalBuddy -f -sc eventsToday
```
#### Show tasks for a specified number of days:
```shell
icalBuddy -n tasksDueBefore:today+{{days}}
```
#### Show events in a time range:
```shell
icalBuddy eventsFrom:'{{start_date}}' to:'{{end_date}}'
```
{% endraw %}{% raw %}
<h2 id="imgcat">
  <a href="/en/osx/imgcat.html">imgcat</a> <a href="#imgcat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A utility to display images directly on the command-line.
> Requires a compatible terminal such as iTerm2.

#### Display an image on the command-line:
```shell
imgcat {{filename}}
```
{% endraw %}{% raw %}
<h2 id="indent">
  <a href="/en/osx/indent.html">indent</a> <a href="#indent"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Change the appearance of a C/C++ program by inserting or deleting whitespace.
> More information: <https://www.freebsd.org/cgi/man.cgi?query=indent>.

#### Format C/C++ source according to the Berkeley style:
```shell
indent {{path/to/source.c}} {{path/to/indented_source.c}} -nbad -nbap -bc -br -c33 -cd33 -cdb -ce -ci4 -cli0 -di16 -fc1 -fcb -i4 -ip -l75 -lp -npcs -nprs -psl -sc -nsob -ts8
```
#### Format C/C++ source according to the style of Kernighan & Ritchie (K&R):
```shell
indent {{path/to/source.c}} {{path/to/indented_source.c}} -nbad -bap -nbc -br -c33 -cd33 -ncdb -ce -ci4 -cli0 -cs -d0 -di1 -nfc1 -nfcb -i4 -nip -l75 -lp -npcs -nprs -npsl -nsc -nsob
```
{% endraw %}{% raw %}
<h2 id="istats">
  <a href="/en/osx/istats.html">istats</a> <a href="#istats"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> CLI tool that shows statistics such as CPU temperature, fan speeds and battery status.
> More information: <https://github.com/Chris911/iStats>.

#### Show all the stats:
```shell
istats
```
#### Show all CPU stats:
```shell
istats cpu
```
#### Show all fan stats:
```shell
istats fan
```
#### Scan and print temperatures:
```shell
istats scan
```
{% endraw %}{% raw %}
<h2 id="launchctl">
  <a href="/en/osx/launchctl.html">launchctl</a> <a href="#launchctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line interface to Apple's `launchd` manager for launch daemons (system-wide services) and launch agents (per-user programs).
> `launchd` loads XML-based `*.plist` files placed in the appropriate locations, and runs the corresponding commands according to their defined schedule.

#### Activate a user-specific agent to be loaded into `launchd` whenever the user logs in:
```shell
launchctl load ~/Library/LaunchAgents/{{my_script}}.plist
```
#### Activate an agent which requires root privileges to run and/or should be loaded whenever any user logs in (note the absence of `~` in the path):
```shell
sudo launchctl load /Library/LaunchAgents/{{root_script}}.plist
```
#### Activate a system-wide daemon to be loaded whenever the system boots up (even if no user logs in):
```shell
sudo launchctl load /Library/LaunchDaemons/{{system_daemon}}.plist
```
#### Show all loaded agents/daemons, with the PID if the process they specify is currently running, and the exit code returned the last time they ran:
```shell
launchctl list
```
#### Unload a currently loaded agent, e.g. to make changes (note: the plist file is automatically loaded into `launchd` after a reboot and/or logging in):
```shell
launchctl unload ~/Library/LaunchAgents/{{my_script}}.plist
```
#### Manually run a known (loaded) agent/daemon, even if it is not the right time (note: this command uses the agent's label, rather than the filename):
```shell
launchctl start {{my_script}}
```
#### Manually kill the process associated with a known agent/daemon, if it is running:
```shell
launchctl stop {{my_script}}
```
{% endraw %}{% raw %}
<h2 id="lldb">
  <a href="/en/osx/lldb.html">lldb</a> <a href="#lldb"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> The LLVM Low-Level Debugger.

#### Debug an executable:
```shell
lldb {{executable}}
```
#### Attach `lldb` to a running process with a given PID:
```shell
lldb -p {{pid}}
```
#### Wait for a new process to launch with a given name, and attach to it:
```shell
lldb -w -n {{process_name}}
```
{% endraw %}{% raw %}
<h2 id="locate">
  <a href="/en/osx/locate.html">locate</a> <a href="#locate"><svg class="icon">
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
sudo /usr/libexec/locate.updatedb
```
{% endraw %}{% raw %}
<h2 id="logger">
  <a href="/en/osx/logger.html">logger</a> <a href="#logger"><svg class="icon">
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
echo {{log_entry}} | logger -h {{hostname}} -P {{port}}
```
#### Use a specific tag for every line logged. Default is the name of logged in user:
```shell
echo {{log_entry}} | logger -t {{tag}}
```
#### Log messages with a given priority. Default is `user.notice`. See `man logger` for all priority options:
```shell
echo {{log_entry}} | logger -p {{user.warning}}
```
{% endraw %}{% raw %}
<h2 id="look">
  <a href="/en/osx/look.html">look</a> <a href="#look"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Look for lines in sorted file.

#### Look for lines which begins with the given prefix:
```shell
look {{prefix}} {{file}}
```
#### Look for lines ignoring case:
```shell
look -f {{prefix}} {{file}}
```
{% endraw %}{% raw %}
<h2 id="m">
  <a href="/en/osx/m.html">m</a> <a href="#m"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Swiss Army Knife for macOS.

#### Get the battery status:
```shell
m battery status
```
#### Turn off bluetooth:
```shell
m bluetooth off
```
#### List available filesystems for formatting:
```shell
m disk filesystems
```
#### Enable Dock's auto hide feature:
```shell
m dock autohide YES
```
#### Disable the firewall:
```shell
m firewall disable
```
{% endraw %}{% raw %}
<h2 id="mas">
  <a href="/en/osx/mas.html">mas</a> <a href="#mas"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Command-line interface for the Mac App Store.
> More information: <https://github.com/mas-cli/mas>.

#### Sign into the Mac App Store for the first time:
```shell
mas signin {{user@example.com}}
```
#### Show all installed applications and their product identifiers:
```shell
mas list
```
#### Search for an application, displaying the price alongside the results:
```shell
mas search {{application}} --price
```
#### Install or update an application:
```shell
mas install {{product_identifier}}
```
#### Install all pending updates:
```shell
mas upgrade
```
{% endraw %}{% raw %}
<h2 id="md5">
  <a href="/en/osx/md5.html">md5</a> <a href="#md5"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Calculate MD5 cryptographic checksums.

#### Calculate the MD5 checksum for a file:
```shell
md5 {{filename}}
```
#### Calculate MD5 checksums for multiple files:
```shell
md5 {{filename1}} {{filename2}}
```
#### Output only the md5 checksum (no filename):
```shell
md5 -q {{filename}}
```
#### Print a checksum of the given string:
```shell
md5 -s {{string}}
```
{% endraw %}{% raw %}
<h2 id="mdfind">
  <a href="/en/osx/mdfind.html">mdfind</a> <a href="#mdfind"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List files matching a given query.

#### Find a file by its name:
```shell
mdfind -name {{file}}
```
#### Find a file by its content:
```shell
mdfind {{query}}
```
#### Find a file containing a string, in a given directory:
```shell
mdfind -onlyin {{directory}} {{query}}
```
{% endraw %}{% raw %}
<h2 id="mdls">
  <a href="/en/osx/mdls.html">mdls</a> <a href="#mdls"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display the metadata attributes for a file.

#### Display the list of metadata attributes for file:
```shell
mdls {{path/to/file}}
```
#### Display a specific metadata attribute:
```shell
mdls -name {{attribute}} {{path/to/file}}
```
{% endraw %}{% raw %}
<h2 id="mdutil">
  <a href="/en/osx/mdutil.html">mdutil</a> <a href="#mdutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage the metadata stores used by Spotlight for indexing.

#### Show the indexing status of the startup volume:
```shell
mdutil -s {{/}}
```
#### Turn on/off the Spotlight indexing for a given volume:
```shell
mdutil -i {{on|off}} {{path/to/volume}}
```
#### Turn on/off indexing for all volumes:
```shell
mdutil -a -i {{on|off}}
```
#### Erase the metadata stores and restart the indexing process:
```shell
mdutil -E {{path/to/volume}}
```
{% endraw %}{% raw %}
<h2 id="mkfile">
  <a href="/en/osx/mkfile.html">mkfile</a> <a href="#mkfile"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create one or more empty files of any size.

#### Create an empty file of 15 kilobytes:
```shell
mkfile -n {{15k}} {{filename}}
```
#### Create a file of a given size and unit (bytes, KB, MB, GB):
```shell
mkfile -n {{size}}{{b|k|m|g}} {{filename}}
```
#### Create two files of 4 megabytes each:
```shell
mkfile -n {{4m}} {{first_filename}} {{second_filename}}
```
{% endraw %}{% raw %}
<h2 id="n">
  <a href="/en/osx/n.html">n</a> <a href="#n"><svg class="icon">
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
<h2 id="netstat">
  <a href="/en/osx/netstat.html">netstat</a> <a href="#netstat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Displays network-related information such as open connections, open socket ports, etc.
> More information: <https://www.unix.com/man-page/osx/1/netstat>.

#### List all ports:
```shell
netstat -a
```
#### List all listening ports:
```shell
netstat -l
```
#### List listening TCP ports:
```shell
netstat -t
```
#### Display PID and program names for a specific protocol:
```shell
netstat -p {{protocol}}
```
#### Print the routing table:
```shell
netstat -nr
```
{% endraw %}{% raw %}
<h2 id="networksetup">
  <a href="/en/osx/networksetup.html">networksetup</a> <a href="#networksetup"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Configuration tool for Network System Preferences.

#### List available network service providers (Ethernet, Wi-Fi, Bluetooth, etc):
```shell
networksetup -listallnetworkservices
```
#### Show network settings for a particular networking device:
```shell
networksetup -getinfo "{{Wi-Fi}}"
```
#### Get currently connected Wi-Fi network name (Wi-Fi device usually en0 or en1):
```shell
networksetup -getairportnetwork {{en0}}
```
#### Connect to a particular Wi-Fi network:
```shell
networksetup -setairportnetwork {{en0}} "{{Airport Network SSID}}" {{password}}
```
{% endraw %}{% raw %}
<h2 id="nm">
  <a href="/en/osx/nm.html">nm</a> <a href="#nm"><svg class="icon">
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
nm -demangle {{file.o}}
```
{% endraw %}{% raw %}
<h2 id="oathtool">
  <a href="/en/osx/oathtool.html">oathtool</a> <a href="#oathtool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> OATH one-time password tool.

#### Generate TOTP token (behaves like Google Authenticator):
```shell
oathtool --totp --base32 {{secret}}
```
#### Generate a TOTP token for a specific time:
```shell
oathtool --totp --now {{2004-02-29 16:21:42}} --base32 {{secret}}
```
#### Validate a TOTP token:
```shell
oathtool --totp --base32 {{secret}} {{token}}
```
{% endraw %}{% raw %}
<h2 id="open">
  <a href="/en/osx/open.html">open</a> <a href="#open"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Opens files, directories and applications.

#### Open a file with the associated application:
```shell
open {{file.ext}}
```
#### Run a graphical macOS application:
```shell
open -a {{Application}}
```
#### Run a graphical macOS app based on the bundle identifier (refer to `osascript` for an easy way to get this):
```shell
open -b {{com.domain.application}}
```
#### Open the current directory in Finder:
```shell
open .
```
#### Reveal a file in Finder:
```shell
open -R {{path/to/file}}
```
#### Open all the files of a given extension in the current directory with the associated application:
```shell
open {{*.ext}}
```
{% endraw %}{% raw %}
<h2 id="opensnoop">
  <a href="/en/osx/opensnoop.html">opensnoop</a> <a href="#opensnoop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool that tracks file opens on your system.

#### Print all file opens as they occur:
```shell
sudo opensnoop
```
#### Track all file opens by a process by name:
```shell
sudo opensnoop -n {{process_name}}
```
#### Track all file opens by a process by PID:
```shell
sudo opensnoop -p {{PID}}
```
#### Track which processes open a specified file:
```shell
sudo opensnoop -f {{path/to/file}}
```
{% endraw %}{% raw %}
<h2 id="osascript">
  <a href="/en/osx/osascript.html">osascript</a> <a href="#osascript"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run AppleScript or JavaScript for Automation (JXA) from the command-line.

#### Run an AppleScript command:
```shell
osascript -e '{{say "Hello world"}}'
```
#### Run multiple AppleScript commands:
```shell
osascript -e '{{say "Hello"}}' -e '{{say "world"}}'
```
#### Run a compiled (`*.scpt`), bundled (`*.scptd`), or plaintext (`*.applescript`) AppleScript file:
```shell
osascript {{path/to/apple.scpt}}
```
#### Get the bundle identifier of an application (useful for `open -b`):
```shell
osascript -e 'id of app "{{Application}}"'
```
#### Run a JavaScript command:
```shell
osascript -l JavaScript -e '{{console.log("Hello world");}}'
```
#### Run a JavaScript file:
```shell
osascript -l JavaScript {{path/to/script.js}}
```
{% endraw %}{% raw %}
<h2 id="pbcopy">
  <a href="/en/osx/pbcopy.html">pbcopy</a> <a href="#pbcopy"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Place standard output in the clipboard.

#### Place the contents of a file in the clipboard:
```shell
pbcopy < {{file}}
```
#### Place the results of a command in the clipboard:
```shell
find . -type t -name "*.png" | pbcopy
```
{% endraw %}{% raw %}
<h2 id="pbpaste">
  <a href="/en/osx/pbpaste.html">pbpaste</a> <a href="#pbpaste"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Send the contents of the clipboard to standard output.

#### Write the contents of the clipboard to a file:
```shell
pbpaste > {{file}}
```
#### Use the contents of the clipboard as input to a command:
```shell
pbpaste | grep foo
```
{% endraw %}{% raw %}
<h2 id="pdfgrep">
  <a href="/en/osx/pdfgrep.html">pdfgrep</a> <a href="#pdfgrep"><svg class="icon">
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
<h2 id="ping">
  <a href="/en/osx/ping.html">ping</a> <a href="#ping"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Send ICMP ECHO_REQUEST packets to network hosts.

#### Ping the specified host:
```shell
ping {{host}}
```
#### Ping a host a specific number of times:
```shell
ping -c {{count}} {{host}}
```
#### Ping `host`, specifying the interval in `seconds` between requests (default is 1 second):
```shell
ping -i {{seconds}} {{host}}
```
#### Ping `host` without trying to lookup symbolic names for addresses:
```shell
ping -n {{host}}
```
#### Ping `host` and ring the bell when a packet is received (if your terminal supports it):
```shell
ping -a {{host}}
```
#### Ping `host` and prints the time a packet was received (this option is an Apple addition):
```shell
ping --apple-time {{host}}
```
{% endraw %}{% raw %}
<h2 id="pkgutil">
  <a href="/en/osx/pkgutil.html">pkgutil</a> <a href="#pkgutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Query and manipulate Mac OS X Installer packages and receipts.

#### List package IDs for all installed packages:
```shell
pkgutil --pkgs
```
#### Verify cryptographic signatures of a package file:
```shell
pkgutil --check-signature {{path/to/filename.pkg}}
```
#### List all the files for an installed package given its ID:
```shell
pkgutil --files {{com.microsoft.Word}}
```
#### Extract the contents of a package file into a directory:
```shell
pkgutil --expand-full {{path/to/filename.pkg}} {{path/to/directory}}
```
{% endraw %}{% raw %}
<h2 id="plutil">
  <a href="/en/osx/plutil.html">plutil</a> <a href="#plutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> View, convert, validate, or edit property list ("plist") files.

#### Display the contents of one or more plist files in human-readable format:
```shell
plutil -p {{file1.plist file2.plist ...}}
```
#### Convert one or more plist files to XML format, overwriting the original files in-place:
```shell
plutil -convert xml1 {{file1.plist file2.plist ...}}
```
#### Convert one or more plist files to binary format, overwriting the original files in-place:
```shell
plutil -convert binary1 {{file1.plist file2.plist ...}}
```
#### Convert a plist file to a different format, writing to a new file:
```shell
plutil -convert {{xml1|binary1|json|swift|objc}} {{path/to/file.plist}} -o {{path/to/new_file.plist}}
```
#### Convert a plist file to a different format, writing to stdout:
```shell
plutil -convert {{xml1|binary1|json|swift|objc}} {{path/to/file.plist}} -o -
```
{% endraw %}{% raw %}
<h2 id="pmset">
  <a href="/en/osx/pmset.html">pmset</a> <a href="#pmset"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Configure macOS power management settings, as one might do in System Preferences > Energy Saver.
> Commands that modify settings must begin with `sudo`.

#### Display the current power management settings:
```shell
pmset -g
```
#### Display the current power source and battery levels:
```shell
pmset -g batt
```
#### Put display to sleep immediately:
```shell
pmset displaysleepnow
```
#### Set display to never sleep when on charger power:
```shell
sudo pmset -c displaysleep 0
```
#### Set display to sleep after 15 minutes when on battery power:
```shell
sudo pmset -b displaysleep 15
```
#### Schedule computer to automatically wake up every weekday at 9 AM:
```shell
sudo pmset repeat wake MTWRF 09:00:00
```
#### Restore to system defaults:
```shell
sudo pmset -a displaysleep 10 disksleep 10 sleep 30 womp 1
```
{% endraw %}{% raw %}
<h2 id="pod">
  <a href="/en/osx/pod.html">pod</a> <a href="#pod"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Dependency manager for Swift and Objective-C Cocoa projects.

#### Create a Podfile for the current project with the default contents:
```shell
pod init
```
#### Download and install all pods defined in the Podfile (that haven't been installed before):
```shell
pod install
```
#### List all available pods:
```shell
pod list
```
#### Show the outdated pods (of those currently installed):
```shell
pod outdated
```
#### Update all currently installed pods to their newest version:
```shell
pod update
```
#### Update a specific (previously installed) pod to its newest version:
```shell
pod update {{pod_name}}
```
#### Remove CocoaPods from a Xcode project:
```shell
pod deintegrate {{xcode_project}}
```
{% endraw %}{% raw %}
<h2 id="port">
  <a href="/en/osx/port.html">port</a> <a href="#port"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Package manager for macOS.

#### Search for a package:
```shell
port search {{search_term}}
```
#### Install a package:
```shell
sudo port install {{package_name}}
```
#### List installed packages:
```shell
port installed
```
#### Update port and fetch latest list of available packages:
```shell
sudo port selfupdate
```
#### Upgrade outdated packages:
```shell
sudo port upgrade outdated
```
#### Remove old versions of installed packages:
```shell
sudo port uninstall inactive
```
{% endraw %}{% raw %}
<h2 id="pwgen">
  <a href="/en/osx/pwgen.html">pwgen</a> <a href="#pwgen"><svg class="icon">
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
<h2 id="qlmanage">
  <a href="/en/osx/qlmanage.html">qlmanage</a> <a href="#qlmanage"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> QuickLook server tool.

#### Display QuickLook for one or multiple files:
```shell
qlmanage -p {{filename}} {{filename2}}
```
#### Compute 300px wide PNG thumbnails of all JPEGs in the current directory and put them in a directory:
```shell
qlmanage {{*.jpg}} -t -s {{300}} {{path/to/directory}}
```
#### Reset QuickLook:
```shell
qlmanage -r
```
{% endraw %}{% raw %}
<h2 id="readlink">
  <a href="/en/osx/readlink.html">readlink</a> <a href="#readlink"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Follow symlinks and get symlink information.
> More information: <https://www.gnu.org/software/coreutils/readlink>.

#### Print the absolute path which the symlink points to:
```shell
readlink {{path/to/symlink}}
```
{% endraw %}{% raw %}
<h2 id="reboot">
  <a href="/en/osx/reboot.html">reboot</a> <a href="#reboot"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Reboot the system.

#### Reboot immediately:
```shell
sudo reboot
```
#### Reboot immediately without gracefully shutting down:
```shell
sudo reboot -q
```
{% endraw %}{% raw %}
<h2 id="rename">
  <a href="/en/osx/rename.html">rename</a> <a href="#rename"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Rename a file or group of files with a regular expression.

#### Replace `from` with `to` in the filenames of the specified files:
```shell
rename 's/{{from}}/{{to}}/' {{*.txt}}
```
{% endraw %}{% raw %}
<h2 id="route">
  <a href="/en/osx/route.html">route</a> <a href="#route"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manually manipulate the routing tables.
> Necessitates to be root.

#### Add a route to a destination through a gateway:
```shell
sudo route add {{dest_ip_address}} {{gateway_address}}
```
#### Add a route to a /24 subnet through a gateway:
```shell
sudo route add {{subnet_ip_address}}/24 {{gateway_address}}
```
#### Run in test mode (does not do anything, just print):
```shell
sudo route -t add {{dest_ip_address}}/24 {{gateway_address}}
```
#### Remove all routes:
```shell
sudo route flush
```
#### Delete a specific route:
```shell
sudo route delete {{dest_ip_address}}/24
```
#### Lookup and display the route for a destination (hostname or IP address):
```shell
sudo route get {{destination}}
```
{% endraw %}{% raw %}
<h2 id="rubocop">
  <a href="/en/osx/rubocop.html">rubocop</a> <a href="#rubocop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Lint Ruby files.

#### Check all files in the current directory (including subdirectories):
```shell
rubocop
```
#### Check one or more specific files or directories:
```shell
rubocop {{path/to/file}} {{path/to/directory}}
```
#### Write output to file:
```shell
rubocop --out {{path/to/file}}
```
#### View list of cops (linter rules):
```shell
rubocop --show-cops
```
#### Exclude a cop:
```shell
rubocop --except {{cop_1}} {{cop_2}}
```
#### Run only specified cops:
```shell
rubocop --only {{cop_1}} {{cop_2}}
```
#### Auto-correct files (experimental):
```shell
rubocop --auto-correct
```
{% endraw %}{% raw %}
<h2 id="safeejectgpu">
  <a href="/en/osx/safeejectgpu.html">SafeEjectGPU</a> <a href="#safeejectgpu"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Eject a GPU safely.
> Visit the man page for more info.

#### Eject all GPUs:
```shell
SafeEjectGPU Eject
```
#### List all GPUs attached:
```shell
SafeEjectGPU gpus
```
#### List apps using a GPU:
```shell
SafeEjectGPU gpuid {{GPU_ID}} apps
```
#### Get the status of a GPU:
```shell
SafeEjectGPU gpuid {{GPU_ID}} status
```
#### Eject a GPU:
```shell
SafeEjectGPU gpuid {{GPU_ID}} Eject
```
#### Launch an app on a GPU:
```shell
SafeEjectGPU gpuid {{GPU_ID}} LaunchOnGPU {{path/to/App.app}}
```
{% endraw %}{% raw %}
<h2 id="say">
  <a href="/en/osx/say.html">say</a> <a href="#say"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Converts text to speech.

#### Say a phrase aloud:
```shell
say "{{I like to ride my bike.}}"
```
#### Read a file aloud:
```shell
say -f {{filename.txt}}
```
#### Say a phrase with a custom voice and speech rate:
```shell
say -v {{voice}} -r {{words_per_minute}} "{{I'm sorry Dave, I can't let you do that.}}"
```
#### List the available voices:
```shell
say -v "?"
```
#### Create an audio file of the spoken text:
```shell
say -o {{filename.aiff}} "{{Here's to the Crazy Ones.}}"
```
{% endraw %}{% raw %}
<h2 id="screencapture">
  <a href="/en/osx/screencapture.html">screencapture</a> <a href="#screencapture"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility to take screenshots and screen recordings.

#### Take a screenshot and save it to a file:
```shell
screencapture {{path/to/file.png}}
```
#### Take a screenshot including the mouse cursor:
```shell
screencapture -C {{path/to/file.png}}
```
#### Take a screenshot and open it in Preview, instead of saving:
```shell
screencapture -P
```
#### Take a screenshot of a selected rectangular area:
```shell
screencapture -i {{path/to/file.png}}
```
#### Take a screenshot after a delay:
```shell
screencapture -T {{seconds}} {{path/to/file.png}}
```
#### Make a screen recording and save it to a file:
```shell
screencapture -v {{path/to/file.mp4}}
```
{% endraw %}{% raw %}
<h2 id="scutil">
  <a href="/en/osx/scutil.html">scutil</a> <a href="#scutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage system configuration parameters.
> Necessitates to be root when setting configuration.

#### Display DNS Configuration:
```shell
scutil --dns
```
#### Display proxy configuration:
```shell
scutil --proxy
```
#### Get computer name:
```shell
scutil --get ComputerName
```
#### Set computer name:
```shell
sudo scutil --set ComputerName {{computer_name}}
```
#### Get hostname:
```shell
scutil --get HostName
```
#### Set hostname:
```shell
scutil --set HostName {{hostname}}
```
{% endraw %}{% raw %}
<h2 id="security">
  <a href="/en/osx/security.html">security</a> <a href="#security"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Administer Keychains, keys, certificates and the Security framework.
> More information: <https://ss64.com/osx/security.html>.

#### List the available keychains:
```shell
security list-keychains
```
#### Delete a specific keychain:
```shell
security delete-keychain {{path}}
```
#### Create a keychain:
```shell
security create-keychain -p {{password}} {{name.keychain}}
```
{% endraw %}{% raw %}
<h2 id="sed">
  <a href="/en/osx/sed.html">sed</a> <a href="#sed"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Edit text in a scriptable manner.
> More information: <https://ss64.com/osx/sed.html>.

#### Replace the first occurrence of a string in a file, and print the result:
```shell
sed 's/{{find}}/{{replace}}/' {{filename}}
```
#### Replace all occurrences of an extended regular expression in a file:
```shell
sed -E 's/{{regular_expression}}/{{replace}}/g' {{filename}}
```
#### Replace all occurrences of a string [i]n a file, overwriting the file (i.e. in-place):
```shell
sed -i '' 's/{{find}}/{{replace}}/g' {{filename}}
```
#### Replace only on lines matching the line pattern:
```shell
sed '/{{line_pattern}}/s/{{find}}/{{replace}}/' {{filename}}
```
#### Print only text between n-th line till the next empty line:
```shell
sed -n '{{line_number}},/^$/p' {{filename}}
```
#### Apply multiple find-replace expressions to a file:
```shell
sed -e 's/{{find}}/{{replace}}/' -e 's/{{find}}/{{replace}}/' {{filename}}
```
#### Replace separator / by any other character not used in the find or replace patterns, e.g., #:
```shell
sed 's#{{find}}#{{replace}}#' {{filename}}
```
#### [d]elete the line at the specific line number [i]n a file, overwriting the file:
```shell
sed -i '' '{{line_number}}d' {{filename}}
```
{% endraw %}{% raw %}
<h2 id="shuf">
  <a href="/en/osx/shuf.html">shuf</a> <a href="#shuf"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate random permutations.

#### Randomize the order of lines in a file and output the result:
```shell
shuf {{filename}}
```
#### Only output the first 5 entries of the result:
```shell
shuf -n {{5}} {{filename}}
```
#### Write output to another file:
```shell
shuf {{filename}} -o {{output_filename}}
```
#### Generate random numbers in range 1-10:
```shell
shuf -i {{1-10}}
```
{% endraw %}{% raw %}
<h2 id="shutdown">
  <a href="/en/osx/shutdown.html">shutdown</a> <a href="#shutdown"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Shutdown and reboot the system.

#### Power off (halt) immediately:
```shell
shutdown -h now
```
#### Sleep immediately:
```shell
shutdown -s now
```
#### Reboot immediately:
```shell
shutdown -r now
```
#### Reboot in 5 minutes:
```shell
shutdown -r +{{5}}
```
#### Power off (halt) at 1:00 pm (Uses 24h clock):
```shell
shutdown -h {{1300}}
```
#### Reboot on May 10th 2042 at 11:30 am (Input format: YYMMDDHHMM):
```shell
shutdown -r {{4205101130}}
```
{% endraw %}{% raw %}
<h2 id="sips">
  <a href="/en/osx/sips.html">sips</a> <a href="#sips"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Apple Scriptable Image Processing System.
> Raster/Query images and ColorSync ICC Profiles.

#### Specify an output directory so that originals do not get modified:
```shell
sips --out {{path/to/out_dir}}
```
#### Resample image at specified size, Image aspect ratio may be altered:
```shell
sips -z {{1920}} {{300}} {{image.ext}}
```
#### Resample image so height and width aren't greater than specified size (notice the capital Z):
```shell
sips -Z {{1920}} {{300}} {{image.ext}}
```
#### Resample all images in a directory to fit a width of 960px (honoring aspect ratio):
```shell
sips --resampleWidth {{960}} {{path/to/images}}
```
#### Convert an image from CMYK to RGB:
```shell
sips --matchTo '/System/Library/ColorSync/Profiles/Generic RGB Profile.icc' {{path/to/image.ext}} {{path/to/out_dir}}
```
#### Remove ColorSync ICC profile from an image:
```shell
sips -d profile --deleteColorManagementProperties {{path/to/image.ext}}
```
{% endraw %}{% raw %}
<h2 id="softwareupdate">
  <a href="/en/osx/softwareupdate.html">softwareupdate</a> <a href="#softwareupdate"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tool for updating macOS App Store apps via the command-line.

#### List all available updates:
```shell
softwareupdate -l
```
#### Download and install all updates:
```shell
softwareupdate -ia
```
#### Download and install all recommended updates:
```shell
softwareupdate -ir
```
#### Download and install a specific app:
```shell
softwareupdate -i {{update_name}}
```
{% endraw %}{% raw %}
<h2 id="split">
  <a href="/en/osx/split.html">split</a> <a href="#split"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Split a file into pieces.

#### Split a file, each split having 10 lines (except the last split):
```shell
split -l {{10}} {{filename}}
```
#### Split a file by a regular expression. The matching line will be the first line of the next output file:
```shell
split -p {{cat|^[dh]og}} {{filename}}
```
#### Split a file with 512 bytes in each split (except the last split; use 512k for kilobytes and 512m for megabytes):
```shell
split -b {{512}} {{filename}}
```
{% endraw %}{% raw %}
<h2 id="spotify">
  <a href="/en/osx/spotify.html">spotify</a> <a href="#spotify"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A command-line interface to Spotify.
> More information: <https://github.com/hnarayanan/shpotify>.

#### Find a song by name and play it:
```shell
spotify play {{song_name}}
```
#### Find a playlist by name and play it:
```shell
spotify play list {{playlist_name}}
```
#### Pause (or resume) playback:
```shell
spotify pause
```
#### Skip to the next song in a playlist:
```shell
spotify next
```
#### Change volume:
```shell
spotify vol {{up|down|value}}
```
#### Show the playback status and song details:
```shell
spotify status
```
{% endraw %}{% raw %}
<h2 id="ssh-add">
  <a href="/en/osx/ssh-add.html">ssh-add</a> <a href="#ssh-add"><svg class="icon">
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
#### Add a key to the ssh-agent and the keychain:
```shell
ssh-add -K {{path/to/private_key}}
```
{% endraw %}{% raw %}
<h2 id="sshuttle">
  <a href="/en/osx/sshuttle.html">sshuttle</a> <a href="#sshuttle"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Transparent proxy server that tunnels traffic over an SSH connection.
> Doesn't require admin, or any special setup on the remote SSH server.
> More information: <https://github.com/sshuttle/sshuttle>.

#### Forward all IPv4 TCP traffic via a remote SSH server:
```shell
sshuttle --remote={{username}}@{{sshserver}} {{0.0.0.0/0}}
```
#### Forward all IPv4 TCP and DNS traffic:
```shell
sshuttle --dns --remote={{username}}@{{sshserver}} {{0.0.0.0/0}}
```
#### Use the tproxy method to forward all IPv4 and IPv6 traffic:
```shell
sudo sshuttle --method=tproxy --remote={{username}}@{{sshserver}} {{0.0.0.0/0}} {{::/0}} --exclude={{your_local_ip_address}} --exclude={{ssh_server_ip_address}}
```
{% endraw %}{% raw %}
<h2 id="stat">
  <a href="/en/osx/stat.html">stat</a> <a href="#stat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display file status.

#### Show file properties such as size, permissions, creation and access dates among others:
```shell
stat {{file}}
```
#### Same as above but verbose (more similar to linux's `stat`):
```shell
stat -x {{file}}
```
#### Show only octal file permissions:
```shell
stat -f %Mp%Lp {{file}}
```
#### Show owner and group of the file:
```shell
stat -f "%Su %Sg" {{file}}
```
#### Show the size of the file in bytes:
```shell
stat -f "%z %N" {{file}}
```
{% endraw %}{% raw %}
<h2 id="sw_vers">
  <a href="/en/osx/sw_vers.html">sw_vers</a> <a href="#sw_vers"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print macOS operating system version information.

#### Print all available information (OS name, version number, and build):
```shell
sw_vers
```
#### Print only the version number of the operating system:
```shell
sw_vers -productVersion
```
#### Print only the build identifier:
```shell
sw_vers -buildVersion
```
{% endraw %}{% raw %}
<h2 id="sysctl">
  <a href="/en/osx/sysctl.html">sysctl</a> <a href="#sysctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Access kernel state information.

#### Show all available variables and their values:
```shell
sysctl -a
```
#### Show Apple model identifier:
```shell
sysctl -n hw.model
```
#### Show CPU model:
```shell
sysctl -n machdep.cpu.brand_string
```
#### Show available CPU features (MMX, SSE, SSE2, SSE3, AES, etc):
```shell
sysctl -n machdep.cpu.features
```
#### Set a changeable kernel state variable:
```shell
sysctl -w {{section.tunable}}={{value}}
```
{% endraw %}{% raw %}
<h2 id="system_profiler">
  <a href="/en/osx/system_profiler.html">system_profiler</a> <a href="#system_profiler"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Report system hardware and software configuration.

#### Display a full system profiler report which can be opened by System Profiler.app:
```shell
system_profiler -xml > MyReport.spx
```
#### Display a hardware overview (Model, CPU, Memory, Serial, etc):
```shell
system_profiler SPHardwareDataType
```
#### Print the system serial number:
```shell
system_profiler SPHardwareDataType|grep "Serial Number (system)" |awk '{print $4}'
```
{% endraw %}{% raw %}
<h2 id="systemsetup">
  <a href="/en/osx/systemsetup.html">systemsetup</a> <a href="#systemsetup"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Configure System Preferences machine settings.

#### Enable remote login (SSH):
```shell
systemsetup -setremotelogin on
```
#### Specify TimeZone, NTP Server and enable network time:
```shell
systemsetup -settimezone {{US/Pacific}} -setnetworktimeserver {{us.pool.ntp.org}} -setusingnetworktime on
```
#### Make the machine never sleep and automatically restart on power failure or kernel panic:
```shell
systemsetup -setsleep off -setrestartpowerfailure on -setrestartfreeze on
```
#### List valid startup disks:
```shell
systemsetup -liststartupdisks
```
#### Specify a new startup disk:
```shell
systemsetup -setstartupdisk {{path}}
```
{% endraw %}{% raw %}
<h2 id="textutil">
  <a href="/en/osx/textutil.html">textutil</a> <a href="#textutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Used to manipulate text files of various formats.

#### Display information about `foo.rtf`:
```shell
textutil -info {{foo.rtf}}
```
#### Convert `foo.rtf` into `foo.html`:
```shell
textutil -convert {{html}} {{foo.rtf}}
```
#### Convert rich text to normal text:
```shell
textutil {{foo.rtf}} -convert {{txt}}
```
#### Convert `foo.txt` into `foo.rtf`, using Times 10 for the font:
```shell
textutil -convert {{rtf}} -font {{Times}} -fontsize {{10}} {{foo.txt}}
```
#### Load all RTF files in the current directory, concatenates their contents, and writes the result out as `index.html` with the HTML title set to "Several Files":
```shell
textutil -cat {{html}} -title "Several Files" -output {{index.html}} *.rtf
```
{% endraw %}{% raw %}
<h2 id="tmutil">
  <a href="/en/osx/tmutil.html">tmutil</a> <a href="#tmutil"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility for managing Time Machine backups. Most verbs require root privileges.
> More information: <https://ss64.com/osx/tmutil.html>.

#### Set a HFS+ drive as the backup destination:
```shell
sudo tmutil setdestination {{path/to/disk_mount_point}}
```
#### Set a APF share or SMB share as the backup destination:
```shell
sudo tmutil setdestination {{protocol://user[:password]@host/share}}
```
#### Append the given destination to the list of destinations:
```shell
sudo tmutil setdestination -a {{destination}}
```
#### Enable automatic backups:
```shell
sudo tmutil enable
```
#### Disable automatic backups:
```shell
sudo tmutil disable
```
#### Start a backup, if one is not running already, and release control of the shell:
```shell
sudo tmutil startbackup
```
#### Start a backup and block until the backup is finished:
```shell
sudo tmutil startbackup -b
```
#### Stop a backup:
```shell
sudo tmutil stopbackup
```
{% endraw %}{% raw %}
<h2 id="top">
  <a href="/en/osx/top.html">top</a> <a href="#top"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Display dynamic real-time information about running processes.

#### Start top, all options are available in the interface:
```shell
top
```
#### Start top sorting processes by internal memory size (default order - process ID):
```shell
top -o mem
```
#### Start top sorting processes first by CPU, then by running time:
```shell
top -o cpu -O time
```
#### Start top displaying only processes owned by given user:
```shell
top -user {{user_name}}
```
#### Get help about interactive commands:
```shell
?
```
{% endraw %}{% raw %}
<h2 id="trap">
  <a href="/en/osx/trap.html">trap</a> <a href="#trap"><svg class="icon">
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
<h2 id="tree">
  <a href="/en/osx/tree.html">tree</a> <a href="#tree"><svg class="icon">
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
#### Print the tree without indentation lines, showing the full path instead (use `-N` to not escape whitespace and special characters):
```shell
tree -i -f
```
#### Print the size of each node next to it, in human-readable format, with directories displaying their cumulative size (as in the `du` command):
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
<h2 id="uname">
  <a href="/en/osx/uname.html">uname</a> <a href="#uname"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Print details about the current machine and the operating system running on it.
> Note: for additional information about the operating system, try the `sw_vers` command.

#### Print hardware-related information: machine and processor:
```shell
uname -mp
```
#### Print software-related information: operating system, release number, and version:
```shell
uname -srv
```
#### Print the nodename (hostname) of the system:
```shell
uname -n
```
#### Print all available system information (hardware, software, nodename):
```shell
uname -a
```
{% endraw %}{% raw %}
<h2 id="uptime">
  <a href="/en/osx/uptime.html">uptime</a> <a href="#uptime"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tell how long the system has been running and other information.

#### Print current time, uptime, number of logged-in users and other information:
```shell
uptime
```
{% endraw %}{% raw %}
<h2 id="uuidgen">
  <a href="/en/osx/uuidgen.html">uuidgen</a> <a href="#uuidgen"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Generate new UUID (Universally Unique IDentifier) strings.
> More information: <https://www.ss64.com/osx/uuidgen.html>.

#### Generate a UUID string:
```shell
uuidgen
```
{% endraw %}{% raw %}
<h2 id="valet">
  <a href="/en/osx/valet.html">valet</a> <a href="#valet"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A Laravel development environment that allows hosting sites via local tunnels on `http://<example>.test`.
> More information: <https://laravel.com/docs/8.x/valet>.

#### Start the valet daemon:
```shell
valet start
```
#### Register the current working directory as a path that Valet should search for sites:
```shell
valet park
```
#### View 'parked' paths:
```shell
valet paths
```
#### Serve a single site instead of an entire directory:
```shell
valet link app-name
```
#### Share a project via an Ngrok tunnel:
```shell
valet share
```
{% endraw %}{% raw %}
<h2 id="w">
  <a href="/en/osx/w.html">w</a> <a href="#w"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Show who is logged on and what they are doing.
> Print user login, TTY, remote host, login time, idle time, current process.

#### Show logged-in users info:
```shell
w
```
#### Show logged-in users info without a header:
```shell
w -h
```
#### Show info about logged-in users, sorted by their idle time:
```shell
w -i
```
{% endraw %}{% raw %}
<h2 id="wacaw">
  <a href="/en/osx/wacaw.html">wacaw</a> <a href="#wacaw"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A little command-line tool for macOS that allows you to capture both still pictures and video from an attached camera.
> More information: <http://webcam-tools.sourceforge.net>.

#### Take a picture from webcam:
```shell
wacaw {{filename}}
```
#### Record a video:
```shell
wacaw --video {{filename}} -D {{duration_in_seconds}}
```
#### Take a picture with custom resolution:
```shell
wacaw -x {{width}} -y {{height}} {{filename}}
```
#### Copy image just taken to clipboard:
```shell
wacaw --to-clipboard
```
#### List the devices available:
```shell
wacaw -L
```
{% endraw %}{% raw %}
<h2 id="whatis">
  <a href="/en/osx/whatis.html">whatis</a> <a href="#whatis"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool that searches a set of database files containing short descriptions of system commands for keywords.
> More information: <http://www.linfo.org/whatis.html>.

#### Search for information about keyword:
```shell
whatis {{keyword}}
```
#### Search for information about multiple keywords:
```shell
whatis {{first_keyword}} {{second_keyword}}
```
{% endraw %}{% raw %}
<h2 id="whence">
  <a href="/en/osx/whence.html">whence</a> <a href="#whence"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A zsh builtin to indicate how a given command would be interpreted.

#### Interpret {{command}}, with expansion if defined as an `alias` (similar to the `command -v` builtin):
```shell
whence {{command}}
```
#### Display type of {{command}}, with location if defined as a function, or binary (equivalent to the `type` and `command -V` builtins):
```shell
whence -v {{command}}
```
#### Same as above, except display content of shell functions instead of location (equivalent to `which` builtin):
```shell
whence -c {{command}}
```
#### Same as above, but show all occurrences on command path (equivalent to the `where` builtin):
```shell
whence -ca {{command}}
```
#### Search only the `PATH` for {{command}}, ignoring builtins, aliases or shell functions (equivalent to the `where` command):
```shell
whence -p {{command}}
```
{% endraw %}{% raw %}
<h2 id="whereis">
  <a href="/en/osx/whereis.html">whereis</a> <a href="#whereis"><svg class="icon">
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
{% endraw %}{% raw %}
<h2 id="wifi-password">
  <a href="/en/osx/wifi-password.html">wifi-password</a> <a href="#wifi-password"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Get the password of the wifi.
> More information: <https://github.com/rauchg/wifi-password>.

#### Get the password for the wifi you are currently logged onto:
```shell
wifi-password
```
#### Get the password for the wifi with a specific SSID:
```shell
wifi-password {{ssid}}
```
#### Print only the password as output:
```shell
wifi-password -q
```
{% endraw %}{% raw %}
<h2 id="xar">
  <a href="/en/osx/xar.html">xar</a> <a href="#xar"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manage .xar archives.
> More information: <https://manned.org/xar>.

#### Create a xar archive of all files in a given directory:
```shell
xar -cf {{archive.xar}} {{path/to/directory}}
```
#### Lis[t] the contents of a given xar archive:
```shell
xar -tf {{archive.xar}}
```
#### Extract the contents of a given xar archive to the current directory:
```shell
xar -xf {{archive.xar}}
```
{% endraw %}{% raw %}
<h2 id="xattr">
  <a href="/en/osx/xattr.html">xattr</a> <a href="#xattr"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Utility to work with extended filesystem attributes.

#### List key:value extended attributes for a given file:
```shell
xattr -l {{file}}
```
#### Write an attribute for a given file:
```shell
xattr -w {{attribute_key}} {{attribute_value}} {{file}}
```
#### Delete an attribute from a given file:
```shell
xattr -d {{com.apple.quarantine}} {{file}}
```
#### Delete all extended attributes from a given file:
```shell
xattr -c {{file}}
```
#### Recursively delete an attribute in a given directory:
```shell
xattr -rd {{attribute_key}} {{directory}}
```
{% endraw %}{% raw %}
<h2 id="xcode-select">
  <a href="/en/osx/xcode-select.html">xcode-select</a> <a href="#xcode-select"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Switch between different versions of Xcode and the included developer tools.
> Also used to update the path to Xcode if it is moved after installation.

#### Install Xcode's command-line tools:
```shell
xcode-select --install
```
#### Select a given path as the active developer directory:
```shell
xcode-select -s {{path/to/Xcode.app/Contents/Developer}}
```
#### Select a given Xcode instance and use its developer directory as the active one:
```shell
xcode-select -s {{path/to/Xcode.app}}
```
#### Print the currently selected developer directory:
```shell
xcode-select -p
```
#### Discard any user-specified developer directory so that it will be found via the default search mechanism:
```shell
sudo xcode-select -r
```
{% endraw %}{% raw %}
<h2 id="xcodebuild">
  <a href="/en/osx/xcodebuild.html">xcodebuild</a> <a href="#xcodebuild"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Build Xcode projects.

#### Build workspace:
```shell
xcodebuild -workspace {{workspace_name.workspace}} -scheme {{scheme_name}} -configuration {{configuration_name}} clean build SYMROOT={{SYMROOT_path}}
```
#### Build project:
```shell
xcodebuild -target {{target_name}} -configuration {{configuration_name}} clean build SYMROOT={{SYMROOT_path}}
```
#### Show SDKs:
```shell
xcodebuild -showsdks
```
{% endraw %}{% raw %}
<h2 id="xctool">
  <a href="/en/osx/xctool.html">xctool</a> <a href="#xctool"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tool for building Xcode projects.
> More information: <https://github.com/facebook/xctool>.

#### Build a single project without any workspace:
```shell
xctool -project {{YourProject.xcodeproj}} -scheme {{YourScheme}} build
```
#### Build a project that is part of a workspace:
```shell
xctool -workspace {{YourWorkspace.xcworkspace}} -scheme {{YourScheme}} build
```
#### Clean, build and execute all the tests:
```shell
xctool -workspace {{YourWorkspace.xcworkspace}} -scheme {{YourScheme}} clean build test
```
{% endraw %}{% raw %}
<h2 id="xed">
  <a href="/en/osx/xed.html">xed</a> <a href="#xed"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Opens files for editing in Xcode.

#### Open file in Xcode:
```shell
xed {{file1}}
```
#### Open file(s) in Xcode, create if it doesn't exist:
```shell
xed -c {{filename1}}
```
#### Open a file in Xcode and jump to line number 75:
```shell
xed -l 75 {{filename}}
```
{% endraw %}{% raw %}
<h2 id="xip">
  <a href="/en/osx/xip.html">xip</a> <a href="#xip"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create or expand compressed files in a secure xip archive.
> Only archives signed by Apple are trusted, so this tool should not be used to create archives.

#### Expand the archive into the current working directory:
```shell
xip --expand {{path/to/file.xip}}
```
{% endraw %}{% raw %}
<h2 id="xsltproc">
  <a href="/en/osx/xsltproc.html">xsltproc</a> <a href="#xsltproc"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Transform XML with XSLT to produce output (usually HTML or XML).

#### Transform an XML file with a specific XSLT stylesheet:
```shell
xsltproc --output {{output.html}} {{stylesheet.xslt}} {{xmlfile.xml}}
```
#### Pass a value to a parameter in the stylesheet:
```shell
xsltproc --output {{output.html}} --stringparam {{name}} {{value}} {{stylesheet.xslt}} {{xmlfile.xml}}
```
{% endraw %}{% raw %}
<h2 id="yaa">
  <a href="/en/osx/yaa.html">yaa</a> <a href="#yaa"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Create and manipulate YAA archives.

#### Create an archive from a directory:
```shell
yaa archive -d {{path/to/directory}} -o {{path/to/output.yaa}}
```
#### Create an archive from a file:
```shell
yaa archive -i {{path/to/file}} -o {{path/to/output.yaa}}
```
#### Extract an archive to the current directory:
```shell
yaa extract -i {{path/to/archive.yaa}}
```
#### List the contents of an archive:
```shell
yaa list -i {{path/to/archive.yaa}}
```
#### Create an archive with a specific compression algorithm:
```shell
yaa archive -a {{algorithm}} -d {{path/to/directory}} -o {{path/to/output.yaa}}
```
#### Create an archive with an 8MB block size:
```shell
yaa archive -b {{8m}} -d {{path/to/directory}} -o {{path/to/output.yaa}}
```
{% endraw %}{% raw %}
<h2 id="yabai">
  <a href="/en/osx/yabai.html">yabai</a> <a href="#yabai"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A tiling window manager for macOS based on binary space partitioning.
> More information: <https://github.com/koekeishiya/yabai>.

#### Set the layout to bsp:
```shell
yabai -m config layout {{bsp}}
```
#### Set the window gap to 10pt:
```shell
yabai -m config window_gap {{10}}
```
#### Enable opacity:
```shell
yabai -m config window_opacity on
```
#### Disable window shadow:
```shell
yabai -m config window_shadow off
```
#### Enable status bar:
```shell
yabai -m config status_bar on
```
{% endraw %}{% raw %}
<h2 id="yank">
  <a href="/en/osx/yank.html">yank</a> <a href="#yank"><svg class="icon">
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
{% endraw %}