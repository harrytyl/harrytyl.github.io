---
layout: cv
permalink: /cv/
title: CV
nav: true
nav_order: 8
cv_pdf: /assets/pdf/website_CV.pdf # you can also use external links here
cv_format: jsonresume # options: rendercv, jsonresume
description: Click the CV icon below to download my full CV. Please feel free to contact me via email or LinkedIn.
# toc:
# sidebar: left
---

{% if site.visitor_map.tracker_id %}

  <div class="infobox visitorbox">
    <p class="infobox-lead">
        Thanks for stopping by. The map shows how many people have visited this site and where they are reading from, courtesy of
      <a href="https://mapmyvisitors.com/" target="_blank" rel="noopener">MapMyVisitors</a>.
    </p>
    <div class="visitor-widget">
      {% if site.visitor_map.widget == 'image' %}
        <a href="https://mapmyvisitors.com/web/{{ site.visitor_map.web_id }}" title="Visit tracker" target="_blank" rel="noopener">
          <img src="https://mapmyvisitors.com/map.png?d={{ site.visitor_map.tracker_id }}&cl=ffffff" alt="Map of visitors to this site" loading="lazy" />
        </a>
      {% else %}
        <script type="text/javascript" id="mapmyvisitors" src="//mapmyvisitors.com/map.js?d={{ site.visitor_map.tracker_id }}&cl=ffffff&w=a"></script>
      {% endif %}
    </div>
  </div>
{% endif %}

<style>
  /* Capitalize the first letter of the About page section headings */
  /* About page section headings ("selected publications" is the only one
     while announcements and latest_posts are disabled): render as
     "Selected Publications" and give it room above. */
  /* Visitor info box, styled to match the info boxes on the other pages. */
  .infobox {
    display: flex;
    flex-wrap: wrap;
    align-items: center;
    gap: 1.25rem 2rem;
    justify-content: space-between;
    padding: 1.25rem 1.5rem;
    margin-top: 3rem;
    border: 1px solid var(--global-divider-color, #e8e8e8);
    border-radius: 0.6rem;
    background-color: var(--global-card-bg-color, #fafafa);
  }

  .infobox-lead {
    flex: 1 1 320px;
    margin: 0;
    font-size: 0.95rem;
    line-height: 1.55;
    color: var(--global-text-color, #1c1c1c);
  }

  .visitor-widget {
    flex: 0 1 auto;
    max-width: 100%;
  }

  .visitor-widget img {
    max-width: 100%;
    height: auto;
  }
</style>
