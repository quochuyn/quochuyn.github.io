---
layout: page
permalink: /coding-projects/
title: coding projects
description: " "
nav: true
nav_order: 2
---

**Youtube Recommendation Website** [Article](https://medium.com/@gabrielalon257/youtube-filtering-capstone-67f755fb6dca) | [Code](https://github.com/quochuyn/youtube_nlp_recommender) | [Video](https://www.youtube.com/watch?v=T_uKgvzt8M0) | [Website](https://youtube-capstone.streamlit.app/) 
This is an end-to-end product for a Youtube video recommender system with a NLP-based filter using LLMs like BERT and Chat-GPT to provide a personalized browsing experience and filter offensive/addictive content.

**NHL Draft Predictions** [Article](https://deepnote.com/@nhl-draft-predictions/NHL-Draft-Predictions-09d8dc5c-d54b-4729-bd12-f4067dd931f4) | [Code](https://github.com/quochuyn/nhl-draft-predictions) 
We leveraged Natural Language Processing (NLP) techniques to predict player outcomes in the National Hockey League (NHL) draft. We outline our journey through various NLP methodologies, starting from the baseline NLTK approach and progressing to state-of-the-art Language Models (LLMs) like Google's BERT and OpenAI's Chat-GPT.

**This Website** [Code](https://github.com/quochuyn/quochuyn.github.io)
I crafted this portfolio website within 3 days by immersing myself in front-end technologies (HTML, Javascript, and CSS) despite having no prior knowledge. Notably, this project is built upon the [al-folio](https://github.com/alshedivat/al-folio) template, incorporating Jekyll and Github Actions for CI/CD, showcasing my rapid learning for web development.

**Pytorch Graph-Based CNN** [Code](https://github.com/quochuyn/DGCN-torch)
This is a PyTorch implementation of a (Dual Graph) Convolutional Neural Network (CNN) for semi-supervised classification from a highly cited research article to find insights in skin cancer single-cell data. I created customized Pytorch classes and functions to match the algorithms proposed in the research paper.

***

{% if site.data.repositories.github_users %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for user in site.data.repositories.github_users %}
    {% include repository/repo_user.html username=user %}
  {% endfor %}
</div>

---

{% if site.repo_trophies.enabled %}
{% for user in site.data.repositories.github_users %}
  {% if site.data.repositories.github_users.size > 1 %}
  <h4>{{ user }}</h4>
  {% endif %}
  <div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% include repository/repo_trophies.html username=user %}
  </div>

  ---

{% endfor %}
{% endif %}
{% endif %}

## GitHub Repositories

{% if site.data.repositories.github_repos %}
<div class="repositories d-flex flex-wrap flex-md-row flex-column justify-content-between align-items-center">
  {% for repo in site.data.repositories.github_repos %}
    {% include repository/repo.html repository=repo %}
  {% endfor %}
</div>
{% endif %}
