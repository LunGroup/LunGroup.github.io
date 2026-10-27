---
permalink: /
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<div class="lab-hero">
  <p class="lab-eyebrow">电化学储能实验室 · 中国科学院大学</p>
  <div class="lab-hero-banner">
    <img src="/images/activity/Retreat2025-web.jpg" alt="课题组合影">
  </div>
</div>

<h2 class="lab-section-title">课题组简介</h2>
<div class="lab-hero-text">
  <p>电化学储能实验室依托中国科学院大学化学科学学院建设，并与魏桥国科高等技术研究院高端化学材料中心（高化中心）有密切合作。课题组研究主要围绕新型储能材料的设计、合成、表征及其回收与再生等相关方向展开，同时依托中科院、中国科学院大学、魏桥国科高化中心等仪器表征平台发展新型材料（原位）表征技术。</p>
  <p>团队负责人伦正言，中国科学院大学化学科学学院副教授，博士生导师。2016 年毕业于中国科学技术大学，获材料物理专业学士学位；2020 年毕业于美国加州大学伯克利分校，获材料科学与工程博士学位，导师 Gerbrand Ceder 教授；2021–2022 年于英国剑桥大学进行博后研究，合作导师化学系 Clare P. Grey 教授和物理系 Akshay Rao 教授；2022 年 6 月通过海外高层次人才计划全职加入中国科学院大学化学科学学院，2023 年起兼任魏桥国科高化中心研究员。</p>
</div>

<h2 class="lab-section-title">依托单位</h2>
<div class="lab-org">
  <p><b>中国科学院大学化学科学学院</b>是学校主要基础学院之一，2017 年入选国家首批一流学科建设计划。近年来，学院校部教师科研成绩显著，在国际重要学术刊物（如 Science, J. Am. Chem. Soc., Angew. Chem. Int. Ed., Adv. Mater.）上发表论文数百篇，出版学术专著多部，获国家专利多项，完成和正在承担国家科技重大专项、“973”、“863”和国家自然科学基金委各类基金项目。</p>
  <p><b>魏桥国科高等技术研究院</b>由世界 500 强山东魏桥创业集团发起创办，在中国科学院大学与山东魏桥创业集团战略合作大背景下，由滨州市人民政府设立的直属事业单位和面向未来新建新型理工类大学的研究平台。高等研究院重点围绕优势主导产业布局学科和专业方向，聚焦国家重大战略需求和地方产业振兴所需要的“高精特尖”学科专业，致力于打造汇聚国内外高水平人才的创新高地和促进产学研用协同的创新阵地。高端化学材料中心是魏桥国科高研院高尖端化学材料研究的分部，配备有顶尖的合成、表征等实验平台。</p>
</div>

<h2 class="lab-section-title">研究方向</h2>
<div class="lab-directions">
  <div class="lab-direction">
    <span class="lab-direction-num">01</span>
    <div>
      <p class="lab-direction-title">新型储能材料的设计与合成</p>
      <p class="lab-direction-desc">锂/钠离子电池正极与固态电解质等</p>
    </div>
  </div>
  <div class="lab-direction">
    <span class="lab-direction-num">02</span>
    <div>
      <p class="lab-direction-title">先进（原位）表征技术及其应用</p>
      <p class="lab-direction-desc">同步辐射、固体核磁 ssNMR、干涉散射光学成像 iSCAT 等</p>
    </div>
  </div>
  <div class="lab-direction">
    <span class="lab-direction-num">03</span>
    <div>
      <p class="lab-direction-title">固体材料合成科学</p>
      <p class="lab-direction-desc">固态反应机理研究与合成方案优化</p>
    </div>
  </div>
  <div class="lab-direction">
    <span class="lab-direction-num">04</span>
    <div>
      <p class="lab-direction-title">锂电池的回收与再生</p>
      <p class="lab-direction-desc">关键金属回收与材料修复再生</p>
    </div>
  </div>
</div>

<div class="lab-stats">
  <div class="lab-stat-total">
    <span class="lab-stat-num">{{ site.publications | size }}</span>
    <span class="lab-stat-label">累计发表论文</span>
  </div>
  <div class="lab-stat-years">
    {% assign pubs = site.publications | sort: "date" | reverse %}
    {% assign groups = pubs | group_by: "section" %}
    {% for group in groups %}
    <span class="lab-year-chip"><b>{{ group.name }}</b>{{ group.items | size }} 篇</span>
    {% endfor %}
  </div>
</div>

<h2 class="lab-section-title">最新动态 <a class="lab-more" href="/year-archive/">查看全部</a></h2>
<ul class="lab-news">
  {% for post in site.posts limit:3 %}
  <li>
    <span class="lab-news-date">{{ post.date | date: "%Y.%m" }}</span>
    <a href="{{ post.url | relative_url }}">{{ post.title }}</a>
  </li>
  {% endfor %}
</ul>

<h2 class="lab-section-title">相关链接</h2>

- [中国科学院大学](https://www.ucas.ac.cn/)
- [化学科学学院](https://chem.ucas.ac.cn)
- [导师学院主页](https://people.ucas.ac.cn/~zylun)
