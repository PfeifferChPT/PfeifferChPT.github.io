⁹---
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
A:  
{% for file in '/demo' %}
<a href="{{ file.url }}">{{ file.url }}</a>  
{{ file.path }}  
{{ file.extname }}  

{% endfor %}
