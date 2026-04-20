---
layout: archive
title: "CV"
permalink: /cv/
author_profile: true
redirect_from:
  - /resume
---

{% include base_path %}

## Education

* **Ph.D. in Computer Science**, Purdue University, 2022–2027 (expected)
  * Advisor: [Steve Hanneke](https://stevehanneke.com/)
* **B.S. in Mathematics**, Tsinghua University, 2017–2022

## Research

My research focuses on machine learning theory, reinforcement learning, and large language models. I am interested in the theoretical foundations of learning, including statistical learning theory, online learning, and algorithms with provable guarantees.

## Publications

<small>* Equal contribution &nbsp;&nbsp; † Alphabetical author order</small>

<ul>{% for post in site.publications reversed %}
  {% include archive-single-cv.html %}
{% endfor %}</ul>

## Teaching

<ul>{% for post in site.teaching reversed %}
  {% include archive-single-cv.html %}
{% endfor %}</ul>
