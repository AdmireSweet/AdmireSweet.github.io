---
layout: page
title: Hello world
tagline: 我是一只合格的程序猿
---


{% for f in site.data.friends %}
<div class="link-chip">
 <img alt="{{f.describe}}" src="{{f.image}}" class="link-chip-icon">
 <a title="{{f.describe}}" target="_blank" class="link-chip-title" href="{{f.url}}">{{f.name}}</a>
</div>
{% endfor %}


<hr/>

  {% if site.data.social.valine_comment.enable  == true %}
  <script src="/comment/av-min.js"></script>
  <script src="/comment/Valine.min.js"></script>
  <div id="comments"></div>
  {% include comments.html %}
  {% endif %}
  {% include scripts.html %}

## 程序猿的全世界

> Hello, world!<br>
> This is the whole world of programmer!<br>


## 走进新世界的大门

> Computer has opened the door of the new world for me.<br>
> So, go for it!
