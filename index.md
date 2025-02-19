---
title: "Here is a squirrel"
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
excerpt: "He wanna be your friend."
intro: 
  - excerpt: 'A place to gather my thoughts, no matter their value.'
# TODO make these tags and/or posts
feature_row:
  - image_path: assets/images/squirrel-3.jpg
    alt: "placeholder image 1"
    title: "New York"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
    alt: "placeholder image 2"
  - image_path: assets/images/squirrel-3.jpg
    title: "Another bit"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
  - image_path: /assets/images/unsplash-2.jpg
    title: "Placeholder 3"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
feature_row2:
  - image_path: /assets/images/unsplash-3.jpg
    alt: "placeholder image 2"
    title: "Placeholder Image Left Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Left aligned with `type="left"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
feature_row3:
  - image_path: /assets/images/unsplash-3.jpg
    alt: "placeholder image 2"
    title: "Placeholder Image Right Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Right aligned with `type="right"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
feature_row4:
  - image_path: /assets/images/unsplash-3.jpg
    alt: "placeholder image 2"
    title: "Placeholder Image Center Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Centered with `type="center"`'
    url: "#test-link"
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
        <p class="page__lead">{{ site.posts.first.excerpt | markdownify | remove: "<p>" | remove: "</p>" }}</p>
      {% include page__meta.html %}
        <p>
          <a href="{{ site.posts.first.url | relative_url }}" class="btn btn--light-outline btn--large">{{ action.label | default: site.data.ui-text[site.locale].more_label | default: "Learn More" }}</a>
        </p>
    </div>
  {% if page.header.caption %}
    <span class="page__hero-caption">{{ page.header.caption | markdownify | remove: "<p>" | remove: "</p>" }}</span>
  {% endif %}
</div>


{% include feature_row id="intro" type="center" %}

{% include feature_row %}

{% include feature_row id="feature_row2" type="left" %}

{% include feature_row id="feature_row3" type="right" %}

{% include feature_row id="feature_row4" type="center" %}