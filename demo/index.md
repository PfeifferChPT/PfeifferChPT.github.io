---
title: Hallo Welt
layout: default
permalink: /demo/index.html
---
<!--
<a href="creativeily.html">creativeily</a>  
<a href="lighthouse.html">lighthouse</a>  
<a href="none.html">none</a>  
<a href="print.html">print</a>  
<a href="ProSidebar.html">ProSidebar</a>  
<a href="thflat.html">thflat</a>  
<a href="writr.html">writr</a>  
-->

<style>
    .image-gallery {overflow: auto; margin-left: -1%!important;}
    .image-gallery li {float: left; display: block; margin: 0 0 1% 1%; width: 19%;}
    .image-gallery li a {text-align: center; text-decoration: none!important; color: #777;}
    .image-gallery li a span {display: block; text-overflow: ellipsis; overflow: hidden; white-space: nowrap; padding: 3px 0;}
    .image-gallery li a img {width: 100%; display: block;}
</style>

{% for file in site.static_files %}{% if file.path contains "/demo" %}{% if file.extname == '.md' %}{% assign filenameparts = file.path | split: "/" %}{% assign filename = filenameparts | last | replace: file.extname,"" %}
<a href="{{ file.path | relative_url }}" data-lightbox="{{ filename }}" title="{{ filename }}">{{ site.url | replace: '.md','.html'}} - {{ filename }}</a>  {% endif %}{% endif %}{% endfor %}
