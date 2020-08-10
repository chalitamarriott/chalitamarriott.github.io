---
layout: default
title: "Home Page"
fulltitle: "The Darker Arts | Art Portfolio" 
excerpt: This website is my art portfolio feel free to browse and use the contact us page to drop me a mail if you like anything!
---
<!-- fulltitle: This overrides the default page title, which is "{{page.tite}} | {{site.title}}" -->
<!-- excerpt: If this isn't set, it'll pull your {{site.tagline}} for meta description-->
<div class="container-fluid">
<div class="row">
{% for post in site.posts %}
  <div class="col-xs-12 col-sm-6 col-md-4">
    <center>
      <a href="img/{{post.imageUrl}}.jpg" data-lightbox="image-{{post.imageUrl}}" data-title="{{post.imageUrl}}">
      <img class="art animate__animated animate__flipInX" style="border-radius: 20px; width:100%;" src="img/{{post.imageUrl}}.jpg"></a>
    </center>
  </div>
{% endfor %}
</div>
</div>