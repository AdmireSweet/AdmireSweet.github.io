---
layout: page
title: 不良人
tagline: 一天是不良人，一生都是不良人……
permalink: /links.html
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
