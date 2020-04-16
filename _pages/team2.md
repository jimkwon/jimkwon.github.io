---
permalink: /team2/
title: "Team2"
excerpt: # ""
author_profile: false

---

{% for staff_member in site.portfolio %}
  <h2>{{ staff_member.name }} - {{ staff_member.position }}</h2>
  <img src={{ staff_member.image }} width="150">
  <p>{{ staff_member.content | markdownify }}</p>
{% endfor %}


