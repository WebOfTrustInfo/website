---
permalink: /
title: "Welcome to the Web of Trust"
layout: single
classes:
  - wide
author_profile: true
header:
  overlay_color: "#000"
  overlay_filter: "0.25"
  overlay_image: /assets/images/splash-image-1.jpg
  og_image: /assets/images/rwot-logo.png

---

{% capture notice-1 %}
{% include nextevent.md %}
{% endcapture%}

<div class="notice--info">{{ notice-1 | markdownify }}</div>

<!-- TODO: Automatically draw this out of a folder of photos -->

<figure class="half">
    <a href="{{ site.url }}{{ site.baseurl }}/assets/images/rwot-fp1.jpeg"><img src="{{ site.url }}{{ site.baseurl }}/assets/images/rwot-fp1.jpeg"></a>
    <a href="{{ site.url }}{{ site.baseurl }}/assets/images/rwot-fp2.jpeg"><img src="{{ site.url }}{{ site.baseurl }}/assets/images/rwot-fp2.jpeg"></a>
</figure>

***What is RWOT?*** Rebooting the Web of Trust (RWOT) is a unique event that brings together professionals, researchers, and enthusiasts to collaborate on decentralized identity and trust solutions. Our goal is to support our community in generating and developing ideas that allow us to better remain in control of our assets, our accounts, and ourselves online!

***What Does RWOT Do?*** RWOT consists of virtual salons and in-person design workshops. They help us to germinate new ideas, establish new connections, and produce finalized content that present those ideas to the larger community. Virtual salons crowdsource inspiration and deliver statements, while design workshops produce at least five white papers on topics decided by the group to have the greatest impact on the future.

{% include nextevent-cta.md %}

## Recent News

{% capture notice-2 %}

 {% for post in site.posts limit: 3 %}
 
  <b>{{ post.date | date: "%Y-%m-%d" }}: <a href="{{ post.url }}">{{ post.title }}</a></b><br>

{% endfor %}
  
{% endcapture%}

<div class="notice--info">{{ notice-2 | markdownify }}</div>


