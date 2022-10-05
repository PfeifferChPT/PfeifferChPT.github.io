---
themelogo: https://template.pc-cdn.eu/assets/img/logo/transparent_logo.png
---
[..](https://pc-cdn-template.pc-tests.cf/demo/)  
[blue](blue.html)  
[blue2](blue2.html)  
[dlt](dlt.html)  
[dltr](dltr.html)  
[green](green.html)  
[grey](grey.html)  
[orange](orange.html)  
[orange2](orange2.html)  
[purple](purple.html)  
[red](red.html)  
[sweet dreams](sweetdreams.html)  
[sweet dreams frosted](sweetdreamsfrosted.html)  
[yellow](yellow.html)  

[test](test.html)
[test](test.html)
[test](test.html)  
[test](test.html)
[test](test.html)
[test](test.html)

[test](test.html)


---

{% for post in site.posts %}
  {% if page.path contains '/demo/writr-color/' %} 
   {{ file.name }} - ({{ file.path }} - {{ file.name }}
  {% endif %}
{% endfor %}
