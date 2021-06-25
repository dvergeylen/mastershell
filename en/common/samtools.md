---
layout: default
title: "samtools"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="samtools">
  <a href="/en/common/samtools.html">samtools</a> <a href="#samtools"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Tools for handling high-throughput sequencing (genomics) data.
> Used for reading/writing/editing/indexing/viewing of data in SAM/BAM/CRAM format.

#### Convert a SAM input file to BAM stream and save to file:
```shell
samtools view -S -b {{input.sam}} > {{output.bam}}
```
#### Take input from stdin (-) and print the SAM header and any reads overlapping a specific region to stdout:
```shell
{{other_command}} | samtools view -h - chromosome:start-end
```
#### Sort file and save to BAM (the output format is automatically determined from the output file's extension):
```shell
samtools sort {{input}} -o {{output.bam}}
```
#### Index a sorted BAM file (creates {{sorted_input.bam.bai}}):
```shell
samtools index {{sorted_input.bam}}
```
#### Print alignment statistics about a file:
```shell
samtools flagstat {{sorted_input}}
```
#### Count alignments to each index (chromosome / contig):
```shell
samtools idxstats {{sorted_indexed_input}}
```
#### Merge multiple files:
```shell
samtools merge {{output}} {{input1 input2 …}}
```
#### Split input file according to read groups:
```shell
samtools split {{merged_input}}
```
{% endraw %}