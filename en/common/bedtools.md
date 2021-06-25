---
layout: default
title: "bedtools"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="bedtools">
  <a href="/en/common/bedtools.html">bedtools</a> <a href="#bedtools"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> A swiss-army knife of tools for genomic-analysis tasks.
> Used to intersect, group, convert and count data in BAM, BED, GFF/GTF, VCF format.
> More information: <https://bedtools.readthedocs.io/en/latest/>.

#### Intersect two files with respect to the sequences' strand and save the result to {{`path/to/output_file`}}:
```shell
bedtools intersect -a {{path/to/file_1}} -b {{path/to/file_2}} -s > {{path/to/output_file}}
```
#### Intersect two files with a left outer join, i.e. report each feature from {{file_1}} and NULL if no overlap with {{file_2}}:
```shell
bedtools intersect -a {{path/to/file_1}} -b {{path/to/file_2}} -lof > {{path/to/output_file}}
```
#### Using more efficient algorithm to intersect two pre-sorted files:
```shell
bedtools intersect -a {{path/to/file_1}} -b {{path/to/file_2}} -sorted > {{path/to/output_file}}
```
#### Group file {{`path/to/file`}} based on the first three and the fifth column and summarize the sixth column by summing it up:
```shell
bedtools groupby -i {{path/to/file}} -c 1-3,5 -g 6 -o sum
```
#### Convert bam-formatted file to a bed-formatted one:
```shell
bedtools bamtobed -i {{path/to/file}}.bam > {{path/to/file}}.bed
```
#### Find for all features in {{file_1}}.bed the closest one in {{file_2}}.bed and write their distance in an extra column (input files must be sorted):
```shell
bedtools closest -a {{path/to/file_1}}.bed -b {{path/to/file_2}}.bed -d
```
{% endraw %}