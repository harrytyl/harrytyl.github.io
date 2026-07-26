---
layout: about
title: About
permalink: /
subtitle:

profile:
  align: right
  image: prof_pic.jpg
  image_circular: false # crops the image to make it circular
  # more_info: >
  #   <p>Stanford University School of Medicine</p>
  #   <p>Palo Alto, CA</p>

selected_papers: true # includes a list of papers marked as "selected={true}"
social: true # includes social icons at the bottom of the page

announcements:
  enabled: false # includes a list of news items
  scrollable: true # adds a vertical scroll bar if there are more than 3 news items
  limit: 5 # leave blank to include all the news in the `_news` folder

latest_posts:
  enabled: false
  scrollable: true # adds a vertical scroll bar if there are more than 3 new posts items
  limit: 3 # leave blank to include all the blog posts
---

I am a [Banting Postdoctoral Fellow](https://banting.fellowships-bourses.gc.ca/en/home-accueil.html) in the [Quantitative Sciences Unit](https://med.stanford.edu/qsu.html) at [Stanford University School of Medicine](https://med.stanford.edu/), where I work with [Dr. Summer Han](https://med.stanford.edu/summerhanlab.html) on lung cancer research. My work leverages large-scale electronic health record data and methods from data science, decision science, and health policy. My research interests include real-world data analysis, clinical prediction modeling, and decision-analytic modeling. Across these areas, my methodological research is driven by real-world applications.

My path here has been non-linear. I am Korean-Canadian and grew up in Vancouver, Canada, where I began my BSc Honours in Chemistry at the University of British Columbia. After working as an intern at a chemicals company thad had once made Old Spice shampoo, I switched into Statistics and went on to complete an MSc in Statistics under the supervision of Drs. [James V. Zidek](https://www.stat.ubc.ca/users/james-v-zidek-frsc-oc) and [Matias Salibian-Barrera](https://www.stat.ubc.ca/users/matias-salibian-barrera) at the same institution. During my MSc, two work experiences proved pivotal: a Big Data Analytics internship at the [United Nations Capital Development Fund](https://www.uncdf.org/) and a fellowship in Data Science for Social Good at the [UBC Data Science Institute](https://dsi.ubc.ca/). These experiences drew me toward the interdisciplinary work at the intersection of statistics and health. Subsequently, I pursued a PhD in health economics and outcomes research in the [Respiratory Evaluation Sciences Program](https://resp.core.ubc.ca/), Faculty of Pharmaceutical Sciences, under the supervision of Drs. [Mohsen Sadatsafavi](https://pharmsci.ubc.ca/directory/mohsen-sadatsafavi) and [John Petkau](https://www.stat.ubc.ca/users/john-petkau).

{% if site.visitor_map.tracker_id %}

  <div class="infobox visitorbox">
    <p class="infobox-lead">
      <b>Visitors.</b> Thanks for stopping by. The map shows how many people have visited this
      site and where they are reading from, courtesy of
      <a href="https://mapmyvisitors.com/" target="_blank" rel="noopener">MapMyVisitors</a>.
      Counting starts from the day the tracker was installed, not from the site's whole history.
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
  .post h2 {
    text-transform: uppercase;
    text-transform: capitalize;
    margin-top: 3.5rem;
  }

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
