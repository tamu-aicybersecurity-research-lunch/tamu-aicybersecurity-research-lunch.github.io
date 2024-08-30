---
title: "Past AI for Cybersecurity Research Lunches"
layout: default
---

# Past AI for Cybersecurity Research Lunches

---

This page contains all previous AI for Cybersecurity Research Lunch events.

**Return to Main Page**: [Go Back](/)

# History Schedule

{% assign past_events = site.schedule | sort: "date" | reverse %}
{% assign today = site.time | date: "%Y-%m-%d" %}

{% for event in past_events %}
  {% if event.date < today %}
    <blockquote class="schedule-post">
      <h3><strong>{{ event.title }}</strong></h3>
      <p><strong>Date:</strong> {{ event.date | date: "%m/%d/%Y" }}</p>
      <p><strong>Speakers:</strong> {{ event.speakers }}</p>
      <p><strong>Abstract:</strong></p>
      <p>{{ event.content | markdownify }}</p>
    </blockquote>
    <hr>
    <br><br>
  {% endif %}
{% endfor %}
