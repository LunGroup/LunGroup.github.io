---
layout: archive
title: "研究成果"
permalink: /publications/
author_profile: true
---

{% include base_path %}

<div class="pub-intro">
  课题组累计发表论文 <strong>{{ site.publications | size }}</strong> 篇。完整列表也可在 <a href="{{ author.googlescholar }}">Google Scholar</a> 个人主页查看。
</div>

{% assign pubs = site.publications | sort: "date" | reverse %}
{% assign groups = pubs | group_by: "section" %}
{% for group in groups %}
  <h2 class="pub-year-head">{{ group.name }}</h2>
  {% for pub in group.items %}
    {% include pub-item.html pub=pub %}
  {% endfor %}
{% endfor %}
