---
permalink: /team/
title: # ""
excerpt: # ""
author_profile: true

---

{% for staff_member in site.team_members %}
  <h2>{{ staff_member.name }} - {{ staff_member.position }}</h2>
  <img src="{{ staff_member.image }}" width="250">
  <p>{{ staff_member.content | markdownify }}</p>
{% endfor %}


