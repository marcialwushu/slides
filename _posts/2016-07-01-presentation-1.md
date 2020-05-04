---
title: Presentation 1
layout: post
permalink: /presentation-1/
background: '#0a5'
slides:
 - title: Slide 1
   slide-data: This is first slide
     
 - title: Slide 2
   slide-data: This is second slide

 - title: Slide 3
   slide-data: ![](https://trello-attachments.s3.amazonaws.com/5d7e8031eaec3e42c24aade0/5e94f88f99a48502ea68509f/2a7a7738dad49a782d209a565f62d4fa/roadsec_93116306_852328841924250_6000492837628222912_n.jpg)
  
---

{% for slide in page.slides %}
                    
<section data-background="{% if slide.background %}{{slide.background}}{% else %}{{page.background}}{% endif %}"><h1>{{slide.title}}</h1>{{ slide.slide-data }}</section>
                    
{% endfor %}
    
