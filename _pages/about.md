---
layout: single
permalink: /
title: "Wishzone"
description: "Wishzone 的学术主页：无线时间同步、嵌入式感知与边缘智能。"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<div class="academic-home">
  <p class="academic-home__affiliation">Beihang University · China</p>
  <p class="academic-home__lead">关注无线时间同步、嵌入式感知与边缘智能。</p>
  <p>我的工作跨越硬件、FPGA、嵌入式固件与算法实现，重点是让时间测量、传感器采集和边缘推理在真实系统中可靠运行。这里整理研究方向与代表项目，并标明各项目目前的验证阶段。</p>

  <div class="academic-links" aria-label="学术与联系链接">
    <a href="mailto:{{ site.author.email }}">电子邮件</a>
    {% if site.author.orcid %}<a href="{{ site.author.orcid }}">ORCID</a>{% endif %}
    <a href="https://github.com/{{ site.author.github }}">GitHub</a>
    {% if site.author.uri %}<a href="{{ site.author.uri }}">个人网站</a>{% endif %}
  </div>

  <h2 id="research">研究方向</h2>
  <div class="academic-research">
    <section>
      <h3>无线时间同步</h3>
      <p>研究基于 FPGA SDR 的硬件时间戳、突发信号到达时间估计，以及双向链路中的时钟校准。</p>
      <p class="academic-research__related">相关项目：<a href="{{ '/portfolio/pwts/' | relative_url }}">PWTS</a></p>
    </section>
    <section>
      <h3>网络化传感与嵌入式系统</h3>
      <p>关注低功耗惯性传感、多节点无线采集、设备固件与上位机之间的系统协同。</p>
      <p class="academic-research__related">相关项目：<a href="{{ '/portfolio/wtsimu/' | relative_url }}">WTSIMU</a>、<a href="{{ '/portfolio/hider/' | relative_url }}">Hider</a></p>
    </section>
    <section>
      <h3>边缘智能</h3>
      <p>探索目标检测模型的边缘部署，以及大语言模型端云协同推测解码的实现与评测。</p>
      <p class="academic-research__related">相关项目：<a href="{{ '/portfolio/yolo/' | relative_url }}">YOLO</a>、<a href="{{ '/portfolio/mssp/' | relative_url }}">MSSP</a></p>
    </section>
  </div>

  <div class="academic-section-heading">
    <h2 id="projects">代表项目</h2>
    <a href="{{ '/portfolio/' | relative_url }}">查看全部项目 →</a>
  </div>
  <ol class="academic-project-list">
    {% for project in site.data.projects %}
    <li>
      <span class="academic-project-list__number">{{ project.number }}</span>
      <div>
        <h3><a href="{{ '/portfolio/' | append: project.slug | append: '/' | relative_url }}">{{ project.name }}</a></h3>
        <p>{{ project.summary }}</p>
        <span class="academic-project-list__meta">{{ project.field }} · {{ project.status }}</span>
      </div>
    </li>
    {% endfor %}
  </ol>

  <h2 id="contact">联系</h2>
  <p>学术交流或项目合作请发送邮件至 <a href="mailto:{{ site.author.email }}">{{ site.author.email }}</a>。</p>
</div>
