---
layout: page
title: About
description: 创造从单片机开始
keywords: xiangxu, 许嘉鑫
comments: true
menu: 关于
permalink: /about/
---

我是Xiangxu，XX者说，追求卓越，成就非凡。

仰慕「优雅编码的艺术」。

坚信熟能生巧，努力改变人生。

## 联系

<ul>
{% for website in site.data.social %}
<li>{{website.sitename }}：<a href="{{ website.url }}" target="_blank">@{{ website.name }}</a></li>
{% endfor %}
</ul>


## Skill Keywords

{% for skill in site.data.skills %}
### {{ skill.name }}
<div class="btn-inline">
{% for keyword in skill.keywords %}
<button class="btn btn-outline" type="button">{{ keyword }}</button>
{% endfor %}
</div>
{% endfor %}
