---
layout: default
title: "sunos"
date: 2021-06-25 18:12:13 +02:00
---
## Table of contents
* <a href="#devfsadm">devfsadm</a>
* <a href="#dmesg">dmesg</a>
* <a href="#prctl">prctl</a>
* <a href="#prstat">prstat</a>
* <a href="#snoop">snoop</a>
* <a href="#svcadm">svcadm</a>
* <a href="#svccfg">svccfg</a>
* <a href="#svcs">svcs</a>
* <a href="#truss">truss</a>

{% raw %}
<h2 id="devfsadm">
  <a href="/en/sunos/devfsadm.html">devfsadm</a> <a href="#devfsadm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Administration command for `/dev`. Maintains the `/dev` namespace.
> More information: <https://www.unix.com/man-page/sunos/1m/devfsadm>.

#### Scan for new disks:
```shell
devfsadm -c disk
```
#### Cleanup any dangling /dev links and scan for new device:
```shell
devfsadm -C -v
```
#### Dry-run - output what would be changed but make no modifications:
```shell
devfsadm -C -v -n
```
{% endraw %}{% raw %}
<h2 id="dmesg">
  <a href="/en/sunos/dmesg.html">dmesg</a> <a href="#dmesg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Write the kernel messages to standard output.
> More information: <https://www.unix.com/man-page/sunos/1m/dmesg>.

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
<h2 id="prctl">
  <a href="/en/sunos/prctl.html">prctl</a> <a href="#prctl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Get or set the resource controls of running processes,.
> Tasks, and projects.
> More information: <https://www.unix.com/man-page/sunos/1/prctl>.

#### Examine process limits and permissions:
```shell
prctl {{PID}}
```
#### Examine process limits and permissions in machine parseable format:
```shell
prctl -P {{PID}}
```
#### Get specific limit for a running process:
```shell
prctl -n process.max-file-descriptor {{PID}}
```
{% endraw %}{% raw %}
<h2 id="prstat">
  <a href="/en/sunos/prstat.html">prstat</a> <a href="#prstat"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Report active process statistics.
> More information: <https://www.unix.com/man-page/sunos/1m/prstat>.

#### Examine all processes and reports statistics sorted by CPU usage:
```shell
prstat
```
#### Examine all processes and reports statistics sorted by memory usage:
```shell
prstat -s rss
```
#### Report total usage summary for each user:
```shell
prstat -t
```
#### Report microstate process accounting information:
```shell
prstat -m
```
#### Print out a list of top 5 CPU using processes every second:
```shell
prstat -c -n 5 -s cpu 1
```
{% endraw %}{% raw %}
<h2 id="snoop">
  <a href="/en/sunos/snoop.html">snoop</a> <a href="#snoop"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Network packet sniffer.
> SunOS equivalent of tcpdump.
> More information: <https://www.unix.com/man-page/sunos/1m/snoop>.

#### Capture packets on a specific network interface:
```shell
snoop -d {{e1000g0}}
```
#### Save captured packets in a file instead of displaying them:
```shell
snoop -o {{filename}}
```
#### Display verbose protocol layer summary of packets from a file:
```shell
snoop -V -i {{filename}}
```
#### Capture network packets that come from a hostname and go to a given port:
```shell
snoop to port {{port}} from host {{hostname}}
```
#### Capture and show an hex-dump of network packets exchanged between two IP addresses:
```shell
snoop -x0 -p4 {{ip_address_1}} {{ip_address_2}}
```
{% endraw %}{% raw %}
<h2 id="svcadm">
  <a href="/en/sunos/svcadm.html">svcadm</a> <a href="#svcadm"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Manipulate service instances.
> More information: <https://www.unix.com/man-page/linux/1m/svcadm>.

#### Enable a service in the service database:
```shell
svcadm enable {{service_name}}
```
#### Disable service:
```shell
svcadm disable {{service_name}}
```
#### Restart a running service:
```shell
svcadm restart {{service_name}}
```
#### Command service to re-read configuration files:
```shell
svcadm refresh {{service_name}}
```
#### Clear a service from maintenance state and command it to start:
```shell
svcadm clear {{service_name}}
```
{% endraw %}{% raw %}
<h2 id="svccfg">
  <a href="/en/sunos/svccfg.html">svccfg</a> <a href="#svccfg"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Import, export, and modify service configurations.
> More information: <https://www.unix.com/man-page/linux/1m/svccfg>.

#### Validate configuration file:
```shell
svccfg validate {{smf.xml}}
```
#### Export service configurations to file:
```shell
svccfg export {{servicename}} > {{smf.xml}}
```
#### Import/update service configurations from file:
```shell
svccfg import {{smf.xml}}
```
{% endraw %}{% raw %}
<h2 id="svcs">
  <a href="/en/sunos/svcs.html">svcs</a> <a href="#svcs"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> List information about running services.
> More information: <https://www.unix.com/man-page/linux/1/svcs>.

#### List all running services:
```shell
svcs
```
#### List services that are not running:
```shell
svcs -vx
```
#### List information about a service:
```shell
svcs apache
```
#### Show location of service log file:
```shell
svcs -L apache
```
#### Display end of a service log file:
```shell
tail $(svcs -L apache)
```
{% endraw %}{% raw %}
<h2 id="truss">
  <a href="/en/sunos/truss.html">truss</a> <a href="#truss"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Troubleshooting tool for tracing system calls.
> SunOS equivalent of strace.
> More information: <https://www.unix.com/man-page/linux/1/truss>.

#### Start tracing a program by executing it, following all child processes:
```shell
truss -f {{program}}
```
#### Start tracing a specific process by its PID:
```shell
truss -p {{pid}}
```
#### Start tracing a program by executing it, showing arguments and environment variables:
```shell
truss -a -e {{program}}
```
#### Count time, calls, and errors for each system call and report a summary on program exit:
```shell
truss -c -p {{pid}}
```
#### Trace a process filtering output by system call:
```shell
truss -p {{pid}} -t {{system_call_name}}
```
{% endraw %}