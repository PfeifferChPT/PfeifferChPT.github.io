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

Vor for
{% for file in site.static_files %}
Vor If 1:
 {% if file.path contains "/demo" %}
Vor If 2:
  {% if file.extname == '.md' %}
In der If2:

    {% assign filenameparts = file.path | split: "/" %}
    {% assign filename = filenameparts | last | replace: file.extname,"" %}
    <a href="{{ file.path | relative_url }}">{{ site.url | replace: '.md','.html'}} - {{ filename }}</a>  

  {% endif %}
 {% endif %}
{% endfor %}
