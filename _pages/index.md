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

***What is RWOT?*** It's a new take on the classic model of a web of trust that was first suggested by PGP. Our goal is to support our community in creating decentralized models of identity and information, to ensure that we can remain in control of our assets, our accounts, and ourselves online!

***What Does RWOT Do?*** RWOT consists of virtual salons and in-person design workshops. They allow us to germinate new ideas and produce finalized content that present those ideas to the larger community. Virtual salons crowdsource inspiration and deliver statements, while design workshops produce at least five white papers on topics decided by the group to have the greatest impact on the future.

_Please consider joining us for the next RWOT event!_

{% capture notice-2 %}

 {% for post in site.posts limit: 2 %}
 
  <b>{{ post.date | date: "%Y-%m-%d" }}: <a href="{{ post.url }}">{{ post.title }}</a></b><br>

{% endfor %}
  
{% endcapture%}

<div class="notice--info">{{ notice-2 | markdownify }}</div>


