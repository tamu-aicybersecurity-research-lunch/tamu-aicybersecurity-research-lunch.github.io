---
title: "Past AI for Cybersecurity Research Lunches"
layout: default
---

# Past AI for Cybersecurity Research Lunches

---

This page has all previews schedule AI for Cybersecurity Research Lunch.

**Return to Main Page**: [Go Back](/)

# History Schedule

{% assign past_events = site.schedule | sort: "date" %} 

{% for event in past_events %}
<blockquote class="schedule-post">
    <h3><strong>{{ event.title }}</strong></h3>

    <p><strong>Date:</strong> {{ event.date | date: "%m/%d/%Y" }}</p>

    <p><strong>Speakers:</strong> {{ event.speakers }}</p>

    <p><strong>Abstract:</strong></p>
    <p>{{ event.content | markdownify }}</p>
</blockquote>
<hr>
<br><br>
{% endfor %}
