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

I am Tianyang Zhou (周天阳 in Chinese), a first-year PhD student in **Information Systems and Management** at the [Heinz College](https://www.heinz.cmu.edu/) of [Carnegie Mellon University](https://www.cmu.edu/), advised by Prof. [Leman Akoglu](https://www.andrew.cmu.edu/user/lakoglu/).

My research centers on the **safety, interpretability, and reliability of large language models (LLMs)**, with a focus on prompt optimization, structured rule learning, and reinforcement learning for trustworthy LLM behavior. I am also interested in deploying LLMs in **high-stakes domains** such as finance.

Before CMU, I completed my B.A. in Economics and Finance (with Distinction) at [Tsinghua University](https://www.tsinghua.edu.cn/en/).

<hr />

<a id="news"></a>

## News

- **May 2026** — Released a first-author preprint, [*Structured Prompt Optimization Meets Reinforcement Learning for Global and Local Interpretability over Complex Text*](https://arxiv.org/abs/2605.29076).
- **Apr 2026** — Co-authored a survey, *"Confidence as Control: A Survey of Confidence Utilization in Large Language Models."*
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

<hr />

<a id="contact"></a>

## Contact

- Email: [tzhou3@andrew.cmu.edu](mailto:tzhou3@andrew.cmu.edu)
- GitHub: [@tyzhou42](https://github.com/tyzhou42)
- Google Scholar: [Tianyang Zhou](https://scholar.google.com/citations?user=dmgL6coAAAAJ&hl=en)
- ORCID: [0009-0006-6122-7745](https://orcid.org/0009-0006-6122-7745)
- LinkedIn: [tianyang-zhou](https://www.linkedin.com/in/tianyang-zhou/)
<!-- TODO: add Twitter/X if desired -->
