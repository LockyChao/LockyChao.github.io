---
layout: archive
title: "Publications"
permalink: /publications/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

{% for post in site.publications reversed %}
  {% include archive-single.html %}
{% endfor %}

* W. B. Xu, X. D. Li, W. D. Xu, L. Gong*, et al., "Human-robot Interaction Oriented Human-in-the-loop Real-time Motion Imitation on a Humanoid Tri-Co Robot," 3rd International Conference on Advanced Robotics and Mechatronics (ICARM), NUS, Singapore, 2018.
