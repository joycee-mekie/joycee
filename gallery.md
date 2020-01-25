---
---

# Photo Gallery

![](/images/img1.jpg){:width="500px"}
![](/images/img2.jpg){:width="500px"}
<br />
![](/images/img3.jpg){:width="500px"}
![](/images/img4.jpg){:width="500px"}

images:
  - image_path: /images/img1.jpg
    title: A
  - image_path: /images/img2.jpg
    title: B
  - image_path: /images/img3.jpg
    title: C
  - image_path: /images/img4.jpg
    title: D
---
<ul class="photo-gallery">
  {% for image in page.images %}
    <li><img src="{{ image.image_path }}" alt="{{ image.title}}"/></li>
  {% endfor %}
</ul>
