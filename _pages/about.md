---
permalink: /
title: ""
excerpt: "Tianyang Zhou — PhD student at CMU Heinz College. LLM safety, interpretability, and reliability."
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<a id="about"></a>

I am a first-year PhD student in **Information Systems and Management** at the [Heinz College](https://www.heinz.cmu.edu/) of [Carnegie Mellon University](https://www.cmu.edu/), advised by Prof. [Leman Akoglu](https://www.andrew.cmu.edu/user/lakoglu/).

My research centers on the **safety, interpretability, and reliability of large language models (LLMs)**, with a focus on prompt optimization, structured rule learning, and reinforcement learning for trustworthy LLM behavior. I am also interested in deploying LLMs in **high-stakes domains** such as finance.

Before CMU, I completed my B.A. in Economics and Finance (with Distinction) at [Tsinghua University](https://www.tsinghua.edu.cn/en/), and was an international guest student at the [University of Pennsylvania](https://www.upenn.edu/). I previously worked with Prof. [Yao Xie](https://www2.isye.gatech.edu/~yxie77/) (Georgia Tech) on non-stationary bandit algorithms and Prof. [Weijie Su](https://statistics.wharton.upenn.edu/profile/suw/) (Penn) on calibrated LLM long-form QA.

<hr />

<a id="news"></a>

## News

- **Apr 2026** — Our co-authored survey *"Confidence as Control: A Survey of Confidence Utilization in Large Language Models"* is under review at TMLR.
- **Aug 2025** — Started my PhD at CMU Heinz, advised by Prof. Leman Akoglu.

<hr />

<a id="publications"></a>

## Publications

{% if site.publication_category %}
  {% for category in site.publication_category %}
    {% assign title_shown = false %}
    {% for post in site.publications reversed %}
      {% if post.category != category[0] %}{% continue %}{% endif %}
      {% unless title_shown %}
### {{ category[1].title }}
        {% assign title_shown = true %}
      {% endunless %}
{% include archive-single.html %}
    {% endfor %}
  {% endfor %}
{% else %}
  {% for post in site.publications reversed %}
{% include archive-single.html %}
  {% endfor %}
{% endif %}

<hr />

<a id="education"></a>

## Education

- **Ph.D. in Information Systems and Management**, Carnegie Mellon University — Heinz College, 2025 – present
  - Advisor: Prof. Leman Akoglu
- **B.A. in Economics and Finance (with Distinction)**, Tsinghua University, 2021 – 2025
  - Minor in Statistics
- **International Guest Student**, University of Pennsylvania, Fall 2023

<hr />

<a id="contact"></a>

## Contact

- Email: [tzhou3@andrew.cmu.edu](mailto:tzhou3@andrew.cmu.edu)
- GitHub: [@tyzhou42](https://github.com/tyzhou42)
- Google Scholar: [Tianyang Zhou](https://scholar.google.com/citations?user=dmgL6coAAAAJ&hl=en)
- ORCID: [0009-0006-6122-7745](https://orcid.org/0009-0006-6122-7745)
<!-- TODO: add LinkedIn once URL provided; Twitter optional -->
