---
layout: default
title: "scancel"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="scancel">
  <a href="/en/linux/scancel.html">scancel</a> <a href="#scancel"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Cancel a Slurm job.
> More information: <https://slurm.schedmd.com/scancel.html>.

#### Cancel a job using its ID:
```shell
scancel {{job_id}}
```
#### Cancel all jobs from a user:
```shell
scancel {{user_name}}
```
{% endraw %}