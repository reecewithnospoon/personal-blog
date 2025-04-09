---
title: "Tokyo Software Engineer"
layout: splash
date: 2025-02-23 21:21:00 +0900
# header:
# # TODO make this the latest post?
#   overlay_color: "#000"
#   overlay_filter: "0.5"
#   overlay_image: /assets/images/squirrel-3.jpg
#   actions:
#     - label: "Read the latest post"
#       url: "https://lalala"
excerpt: "Articles about philosophy, software, and hobbies from a British engineer in Tokyo."
intro: 
  - excerpt: 'This is a Jekyll blog I built to exercise my brain through writing. I like to discuss philosophy, programming, self-improvement, and life in Japan.'
# TODO make these tags and/or posts
feature_row:
  - image_path: assets/images/diogenes.jpg
    title: "Philosophy"
    excerpt: "Philosophy teaches me how to navigate the world."
    alt: "Diogenes the Cynic"
    url: "/categories/philosophy"
    btn_label: "Read more"
    btn_class: "btn--primary"
  - image_path: assets/images/commodore.jpg
    alt: "Commodore 64"
    title: "Software Engineering"
    excerpt: "Curiosity is important."
    url: "/categories/engineering"
    btn_label: "Read more"
    btn_class: "btn--primary"
  - image_path: /assets/images/sakura.jpg
    alt: "Sakura and mount Fuji"
    title: "Life in Japan"
    excerpt: "The country that I'm glad to call home."
    url: "/categories/japan"
    btn_label: "Read more"
    btn_class: "btn--primary"
feature_row2:
  - image_path: /assets/images/portfolio.png
    alt: "Portfolio"
    title: "My personal site"
    excerpt: "Learn more about me and check my CV at dev.reecehayward.com"
    url: "https://dev.reecehayward.com"
    btn_label: "Read More"
    btn_class: "btn--primary"
---
<div class="page__hero--overlay"
  style="background-color: #000;background-image: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('{{ site.posts.first.header.overlay_image }}');"
>
    <div class="wrapper">
      <h1 id="page-title" class="page__title" itemprop="headline">
        {{ site.posts.first.title | default: site.title | markdownify | remove: "<p>" | remove: "</p>" }}
      </h1>
        <p class="page__lead">{{ site.posts.first.excerpt | markdownify | truncatewords: 25 | remove: "<p>" | remove: "</p>" }}</p>
      {% include page__meta.html %}
        <p>
          <a href="{{ site.posts.first.url | relative_url }}" class="btn btn--light-outline btn--large">{{ action.label | default: site.data.ui-text[site.locale].more_label | default: "Read the full post" }}</a>
        </p>
    </div>
  {% if page.header.caption %}
    <span class="page__hero-caption">{{ page.header.caption | markdownify | remove: "<p>" | remove: "</p>" }}</span>
  {% endif %}
</div>


{% include feature_row id="intro" type="center" %}

{% include feature_row %}

{% include feature_row id="feature_row2" type="left" %}

{% include video id="PZ7lDrwYdZc" provider="youtube" %}