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

I am a first-year PhD student at the [Heinz College](https://www.heinz.cmu.edu/) of [Carnegie Mellon University](https://www.cmu.edu/), advised by Prof. [Leman Akoglu](https://www.andrew.cmu.edu/user/lakoglu/) and Prof. [Pedro Ferreira](https://www.heinz.cmu.edu/faculty-research/profiles/ferreira-pedro). <!-- TODO: confirm Pedro Ferreira profile URL -->

My research centers on the **safety, interpretability, and reliability of large language models (LLMs)**, with a particular focus on their deployment in **high-stakes domains** such as finance and human mobility modeling. I approach these problems across multiple levels of model access:

- **Black-box** — output monitoring with diverse metrics and anomaly detectors; optimization-based pipelines that let LLMs identify and self-correct errors.
- **White-box** — probing internal activations to detect anomalous representations, and developing steering mechanisms that intervene on model behavior at inference time.
- **Training-time** — supervised fine-tuning and reinforcement learning to more fundamentally reshape model behavior for domain-specific safety and reliability requirements.

I currently collaborate with faculty at CMU [Tepper School of Business](https://www.cmu.edu/tepper/) on using LLMs to extract interpretable insights from financial analyst reports.

<!-- TODO: add a sentence about pre-PhD background once you tell me your undergrad school + years -->

<hr />

<a id="news"></a>

## News

<!-- TODO: replace with real dated items as things happen -->

- **May 2026** — Submitted my first-author paper *"From Rules to Reasoning: Scalable and Interpretable Complex Text Classification with LLMs"*.
- **Apr 2026** — Our co-authored survey *"Confidence as Control: A Survey of Confidence Utilization in Large Language Models"* is under review at TMLR.
- **Aug 2025** — Started my PhD at CMU Heinz, advised by Prof. Leman Akoglu and Prof. Pedro Ferreira.

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

- **Ph.D. in [TODO: program name]**, Carnegie Mellon University — Heinz College, 2025 –
  - Advisors: Prof. Leman Akoglu, Prof. Pedro Ferreira
- **B.[TODO: degree, e.g. Eng / Sc]**, [TODO: undergraduate institution], [TODO: years]

<hr />

<a id="contact"></a>

## Contact

- Email: [tzhou3@andrew.cmu.edu](mailto:tzhou3@andrew.cmu.edu)
- GitHub: [@tyzhou42](https://github.com/tyzhou42)
- Google Scholar: [Tianyang Zhou](https://scholar.google.com/citations?user=dmgL6coAAAAJ&hl=en)
- ORCID: [0009-0006-6122-7745](https://orcid.org/0009-0006-6122-7745)
<!-- TODO: add Twitter / LinkedIn if desired -->
