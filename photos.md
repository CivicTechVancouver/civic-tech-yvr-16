---
title: Photos
---

{% assign image_files = site.static_files | where: "image", true %}
{% for image in image_files %}
  ![{{ image.name }}]({{ image.path }})
{% endfor %}
