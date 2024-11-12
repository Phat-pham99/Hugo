+++
date = '2024-11-12T15:56:21+07:00'
draft = true
title = 'My First Post'
+++
# Hello bro
## This my first post using Hugo

{{ $image := .Resources.Get "El_Gato_Original.webp" }}
{{/* Convert the image from JPG to PNG. */}}
{{ $image := $image.Process "png" }}
<img src="{{ $image.RelPermalink }}" width="{{ $image.Width }}" height="{{ $image.Height }}">