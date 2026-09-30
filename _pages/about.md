---
layout: default
permalink: /
title: "工程与研究"
description: "Wishzone 的个人网站，记录嵌入式系统、无线时间同步、计算机视觉与边缘智能项目。"
redirect_from:
  - /about/
  - /about.html
---

<main class="portfolio-site" id="main">
  <section class="site-hero" aria-labelledby="hero-title">
    <div class="site-hero__copy">
      <p class="site-kicker"><span class="site-kicker__line"></span> WISHZONE / PORTFOLIO</p>
      <h1 id="hero-title">把想法做成<br><span>可以运行的系统。</span></h1>
      <p class="site-hero__lead">我关注嵌入式系统、无线时间同步与边缘智能，工作跨越硬件、固件、算法和上位机。这里记录正在推进的项目，以及从实验走向可用系统的过程。</p>
      <div class="site-actions">
        <a class="site-button site-button--primary" href="{{ '/portfolio/' | relative_url }}">查看项目 <span aria-hidden="true">↗</span></a>
        <a class="site-button site-button--text" href="mailto:{{ site.author.email }}">联系我 <span aria-hidden="true">↗</span></a>
      </div>
    </div>
    <div class="site-hero__visual" aria-hidden="true">
      <div class="site-hero__orbit site-hero__orbit--outer"></div>
      <div class="site-hero__orbit site-hero__orbit--inner"></div>
      <div class="site-hero__signal"><i></i><i></i><i></i><i></i><i></i><i></i><i></i></div>
      <span class="site-hero__dot site-hero__dot--one"></span>
      <span class="site-hero__dot site-hero__dot--two"></span>
      <span class="site-hero__visual-label">BUILD · MEASURE · ITERATE</span>
    </div>
  </section>

  <section class="site-section" id="projects" aria-labelledby="projects-title">
    <div class="site-section__heading">
      <div>
        <p class="site-eyebrow">SELECTED WORK / 01—05</p>
        <h2 id="projects-title">项目实践</h2>
      </div>
      <a class="site-inline-link" href="{{ '/portfolio/' | relative_url }}">浏览全部项目 <span aria-hidden="true">↗</span></a>
    </div>
    <div class="project-grid">
      {% for project in site.data.projects %}
        <a class="project-card project-card--{{ project.slug }}" href="{{ '/portfolio/' | append: project.slug | append: '/' | relative_url }}" aria-label="查看 {{ project.name }} 项目详情">
          <span class="project-card__top"><span>{{ project.number }} / {{ project.field }}</span><span aria-hidden="true">↗</span></span>
          <span class="project-card__graphic" aria-hidden="true"><span></span><span></span><span></span></span>
          <span class="project-card__body">
            <strong>{{ project.name }}</strong>
            <span class="project-card__summary">{{ project.summary }}</span>
            <span class="project-card__tags">{% for tag in project.tags limit:3 %}<em>{{ tag }}</em>{% endfor %}</span>
          </span>
        </a>
      {% endfor %}
    </div>
  </section>

  <section class="site-about" id="about" aria-labelledby="about-title">
    <div><p class="site-eyebrow">ABOUT / WISHZONE</p><h2 id="about-title">关于我</h2></div>
    <div class="site-about__copy">
      <p>目前在北京航空航天大学开展学习与研究。我喜欢把系统中的关键环节亲手打通：从板级调试与时序测量，到嵌入式固件、服务端和可视化工具。</p>
      <p>项目记录会区分已经完成的软件验证与仍待开展的真实场景测试。对技术交流或合作感兴趣，欢迎来信。</p>
      <a class="site-inline-link" href="mailto:{{ site.author.email }}">{{ site.author.email }} <span aria-hidden="true">↗</span></a>
    </div>
  </section>

  <section class="site-contact" id="contact" aria-labelledby="contact-title">
    <p class="site-eyebrow">LET'S CONNECT</p>
    <h2 id="contact-title">聊聊你的想法。</h2>
    <p>无线同步、传感器系统、边缘计算，或者一个值得动手解决的问题。</p>
    <div class="site-actions">
      <a class="site-button site-button--light" href="mailto:{{ site.author.email }}">发送邮件 <span aria-hidden="true">↗</span></a>
      <a class="site-button site-button--outline" href="https://github.com/{{ site.author.github }}" rel="me">GitHub <span aria-hidden="true">↗</span></a>
    </div>
  </section>
</main>
