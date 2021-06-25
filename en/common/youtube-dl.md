---
layout: default
title: "youtube-dl"
date: 2021-06-25 18:12:13 +02:00
---
{% raw %}
<h2 id="youtube-dl">
  <a href="/en/common/youtube-dl.html">youtube-dl</a> <a href="#youtube-dl"><svg class="icon">
    <use href="/assets/images/unicode_sprite.svg#link" />
  </svg></a>
</h2>
> Download videos from YouTube and other websites.
> More information: <http://rg3.github.io/youtube-dl/>.

#### Download a video or playlist:
```shell
youtube-dl '{{https://www.youtube.com/watch?v=oHg5SJYRHA0}}'
```
#### List all formats that a video or playlist is available in:
```shell
youtube-dl --list-formats '{{https://www.youtube.com/watch?v=Mwa0_nE9H7A}}'
```
#### Download a video or playlist at a specific quality:
```shell
youtube-dl --format "{{best[height<=480]}}" '{{https://www.youtube.com/watch?v=oHg5SJYRHA0}}'
```
#### Download the audio from a video and convert it to an MP3:
```shell
youtube-dl -x --audio-format {{mp3}} '{{url}}'
```
#### Download the best quality audio and video and merge them:
```shell
youtube-dl -f bestvideo+bestaudio '{{url}}'
```
#### Download video(s) as MP4 files with custom filenames:
```shell
youtube-dl --format {{mp4}} -o "{{%(title)s by %(uploader)s on %(upload_date)s in %(playlist)s.%(ext)s}}" '{{url}}'
```
#### Download a particular language's subtitles along with the video:
```shell
youtube-dl --sub-lang {{en}} --write-sub '{{https://www.youtube.com/watch?v=Mwa0_nE9H7A}}'
```
#### Download a playlist and extract mp3 from it:
```shell
youtube-dl -f "bestaudio" --continue --no-overwrites --ignore-errors --extract-audio --audio-format mp3 -o "%(title)s.%(ext)s" {{url_to_playlist}}
```
{% endraw %}