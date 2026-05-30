---
permalink: /
title: "About"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

I am a postdoctoral researcher at the [ELLIS Institute Tübingen](https://institute-tue.ellis.eu/compass) (co-affiliated with the [Max Planck Institute for Intelligent Systems](https://is.mpg.de/compass)). I am part of the Cooperative Machine Intelligence for People-Aligned Safe Systems (COMPASS) group, led by [Sahar Abdelnabi](https://s-abdelnabi.github.io/). My research focuses on enhancing [trustworthy](/publications/#trustworthy-ai), [safe](/publications/#ai-safety), and effective [reasoning](/publications/#reasoning) in language models and agentic systems.

I did my Ph.D. in Machine Learning & Natural Language Processing at [UKP Lab](https://www.informatik.tu-darmstadt.de/ukp/ukp_home/index.en.jsp) in [TU Darmstadt](https://www.tu-darmstadt.de/index.en.jsp), supervised by [Prof. Iryna Gurevych](https://www.informatik.tu-darmstadt.de/ukp/ukp_home/head_ukp/index.en.jsp). During my Ph.D., I interned at [Parameter Lab](https://www.parameterlab.de), where we worked with [Naver AI](https://clova.ai/en/ai-research) on trustworthy AI.

Before my Ph.D., I worked at the Coleridge Initiative, where we organized the Kaggle Competition [*Show US the Data*](https://www.kaggle.com/c/coleridgeinitiative-show-us-the-data/overview). I got my master's degree from the [School of Computing](https://cs.kaist.ac.kr/) at [KAIST](https://www.kaist.ac.kr/en/), where I was a research assistant at IR&NLP Lab and advised by [Professor Sung-Hyon Myaeng](http://ir.kaist.ac.kr/member/professor/).

Education
======
* Ph.D. in Computer Science, TU Darmstadt, 2026
* M.S. in Computer Science, KAIST, 2021
* B.Sc. in Computer Science & Engineering (*Summa Cum Laude*), University of Malaga, 2017

News
======

<style>
  .news-table { width: 100%; border-collapse: collapse; margin-top: 0.3em; border: none !important; box-shadow: none !important; }
  .news-table td { padding: 0.35em 0.75em 0.35em 0; vertical-align: top; border: none !important; background: none !important; }
  .news-date {
    white-space: nowrap;
    font-size: 0.82em;
    color: #fff;
    background: #52adc8;
    border-radius: 0.3em;
    padding: 0.1em 0.5em;
    font-weight: bold;
  }
  .news-text { font-size: 0.92em; line-height: 1.45; }
  .news-icon { color: #52adc8; margin-right: 0.45em; width: 1.1em; text-align: center; }
</style>

<table class="news-table">
  <tr>
    <td><span class="news-date">May 2026</span></td>
    <td class="news-text"><i class="fas fa-file-lines news-icon" aria-hidden="true"></i>New preprint: <a href="https://arxiv.org/abs/2605.28591">Models That Know How Evaluations Are Designed Score Safer</a>.</td>
  </tr>
  <tr>
    <td><span class="news-date">Mar 2026</span></td>
    <td class="news-text"><i class="fas fa-building-columns news-icon" aria-hidden="true"></i>Started as a postdoctoral researcher at the <a href="https://institute-tue.ellis.eu/compass">ELLIS Institute Tübingen</a> (COMPASS group).</td>
  </tr>
  <tr>
    <td><span class="news-date">Feb 2026</span></td>
    <td class="news-text"><i class="fas fa-file-lines news-icon" aria-hidden="true"></i>New preprint: <a href="https://arxiv.org/abs/2602.24210">Controllable Reasoning Models are Private Thinkers</a>.</td>
  </tr>
  <tr>
    <td><span class="news-date">Dec 2025</span></td>
    <td class="news-text"><i class="fas fa-person-chalkboard news-icon" aria-hidden="true"></i><a href="https://arxiv.org/abs/2506.11097">C-SEO Bench</a> presented at NeurIPS 2025 Datasets &amp; Benchmarks.</td>
  </tr>
  <tr>
    <td><span class="news-date">Nov 2025</span></td>
    <td class="news-text"><i class="fas fa-person-chalkboard news-icon" aria-hidden="true"></i><a href="https://arxiv.org/abs/2506.15674">Leaky Thoughts</a> presented at EMNLP 2025.</td>
  </tr>
  <tr>
    <td><span class="news-date">Jul 2025</span></td>
    <td class="news-text"><i class="fas fa-person-chalkboard news-icon" aria-hidden="true"></i><a href="https://aclanthology.org/2025.acl-long.191/">Fine-Tuning on Diverse Reasoning Chains</a> presented at ACL 2025.</td>
  </tr>
</table>

Selected Publications
======

<style>
  .home-pub-entry { margin-bottom: 1.2em; }
  .home-pub-entry div, .home-pub-entry p { margin: 0; padding: 0; line-height: 1.4; }
  .home-pub-title { font-weight: bold; margin-bottom: 0.2em !important; }
  .home-pub-authors { margin-bottom: 0.1em !important; }
  .home-pub-venue { opacity: 0.8; margin-bottom: 0.3em !important; }
  .home-pub-categories { margin: 0.3em 0 0.3em !important; }
  .home-pub-badge {
    display: inline-block;
    margin: 0 0.25em 0.2em 0;
    padding: 0.1em 0.5em;
    border-radius: 1em;
    background: #eef4f6;
    color: #2a6f86;
    font-size: 0.7em;
    border: 1px solid #cfe2e9;
  }
  .home-pub-links a {
    display: inline-block;
    margin: 0 0.3em 0.2em 0;
    padding: 0.1em 0.5em;
    border: 1px solid #52adc8;
    border-radius: 0.3em;
    font-size: 0.72em;
    color: #52adc8;
    text-decoration: none;
  }
  .home-pub-links a:hover { background: #52adc8; color: #fff; }
</style>

{% assign selected_pubs = site.publications | where: "selected", "y" | sort: "date" | reverse %}
{% for pub in selected_pubs %}
<div class="home-pub-entry">
  <div class="home-pub-title">
    {% if pub.paperurl %}<a href="{{ pub.paperurl }}">{{ pub.title }}</a>{% else %}{{ pub.title }}{% endif %}
  </div>
  <div class="home-pub-authors">{{ pub.authors }}</div>
  <div class="home-pub-venue"><i>{{ pub.venue }}</i></div>
  {% if pub.categories.size > 0 %}
  <div class="home-pub-categories">
    {% for c in pub.categories %}<span class="home-pub-badge">{{ c }}</span>{% endfor %}
  </div>
  {% endif %}
  <div class="home-pub-links">
    {% if pub.paperurl %}<a href="{{ pub.paperurl }}" target="_blank">Paper</a>{% endif %}
    {% if pub.slides %}<a href="{{ pub.slides | prepend: site.baseurl }}" target="_blank">Slides</a>{% endif %}
    {% if pub.poster %}<a href="{{ pub.poster | prepend: site.baseurl }}" target="_blank">Poster</a>{% endif %}
    {% if pub.video %}<a href="{{ pub.video }}" target="_blank">Video</a>{% endif %}
    {% if pub.website %}<a href="{{ pub.website }}" target="_blank">Website</a>{% endif %}
    {% if pub.code %}<a href="{{ pub.code }}" target="_blank">Code</a>{% endif %}
    {% if pub.data %}<a href="{{ pub.data }}" target="_blank">Data</a>{% endif %}
  </div>
</div>
{% endfor %}

<p><a href="/publications/">→ Full publication list</a></p>
