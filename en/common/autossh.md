---
layout: default
title: "autossh"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="autossh">
  <a href="/en/common/autossh.html">autossh</a> <a href="#autossh"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Run, monitor and restart SSH connections.
> Auto-reconnects to keep port forwarding tunnels up. Accepts all `ssh` flags.
> More information: <https://www.harding.motd.ca/autossh>.

#### Start an SSH session, restarting when a monitoring port fails to return data:
```shell
autossh -M {{monitor_port}} "{{ssh_command}}"
```
#### Forward a local port to a remote one, restarting when necessary:
```shell
autossh -M {{monitor_port}} -L {{local_port}}:localhost:{{remote_port}} {{user}}@{{host}}
```
#### Fork `autossh` into the background before executing `ssh` and don't open a remote shell:
```shell
autossh -f -M {{monitor_port}} -N "{{ssh_command}}"
```
#### Run in the background, with no monitoring port, and instead send SSH keep-alive packets every 10 seconds to detect failure:
```shell
autossh -f -M 0 -N -o "ServerAliveInterval 10" -o "ServerAliveCountMax 3" "{{ssh_command}}"
```
#### Run in the background, with no monitoring port and no remote shell, exiting if the port forward fails:
```shell
autossh -f -M 0 -N -o "ServerAliveInterval 10" -o "ServerAliveCountMax 3" -o ExitOnForwardFailure=yes -L {{local_port}}:localhost:{{remote_port}} {{user}}@{{host}}
```
#### Run in the background, logging `autossh` debug output and `ssh` verbose output to files:
```shell
AUTOSSH_DEBUG=1 AUTOSSH_LOGFILE={{path/to/autossh_log_file.log}} autossh -f -M {{monitor_port}} -v -E {{path/to/ssh_log_file.log}} {{ssh_command}}
```
{% endraw %}