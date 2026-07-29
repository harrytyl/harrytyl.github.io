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

  <!--
    Visitor tracking only: requesting this image registers the visit with
    MapMyVisitors, and nothing is drawn on the page. Read the numbers at
    https://mapmyvisitors.com/web/{{ site.visitor_map.web_id }}. Set
    visitor_map.show_box to true in _config.yml to also display the visible
    map box on the CV page.
  -->

<img
    class="visitor-tracker"
    src="https://mapmyvisitors.com/map.png?cl=080808&w=500&t=tt&d={{ site.visitor_map.tracker_id }}&co=ffffff&ct=808080"
    alt=""
    aria-hidden="true"
    width="1"
    height="1"
  />
{% endif %}

<style>
  /* Tracking pixel: kept off-screen rather than display:none so the browser
     reliably still requests it. */
  .visitor-tracker {
    position: absolute;
    left: -9999px;
    width: 1px;
    height: 1px;
    opacity: 0;
    pointer-events: none;
  }

  /* Capitalize the first letter of the About page section headings */
  /* About page section headings ("selected publications" is the only one
     while announcements and latest_posts are disabled): render as
     "Selected Publications" and give it room above. */
  .post h2 {
    text-transform: uppercase;
    text-transform: capitalize;
    margin-top: 3.5rem;
  }
</style>
