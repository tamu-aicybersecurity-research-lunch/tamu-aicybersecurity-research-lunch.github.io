---
title: "AI for Cybersecurity Research Lunch"
layout: default
---

# AI for Cybersecurity Research Lunch

---

<aside>
💡 The TAMU Cybersecurity Research Lunch is a weekly event on Tuesday where students and researchers present their latest work to peers. Talks are open to anybody, but regular attendees are expected to give a presentation on their work.
</aside>

**Format:** The lunch is held **every Tuesday** during Fall 2024 in **PETR 214 from 12:00 PM to 1:00 PM**. If you'd like to give a talk, please contact Ze Sheng with an abstract (zesheng@tamu.edu).


**Mailing List:** [aicybersecurity-research-lunch@lists.tamu.edu](mailto:aicybersecurity-research-lunch@lists.tamu.edu)

**Previous Meetings:**: [View All Past Events](/history.html)

**🍔Ordering Food🍔:** Coming Soon

# Upcoming Schedule

{% assign sorted_events = site.schedule | sort: "date" | reverse | limit: 10 %}

{% for event in sorted_events %}
<blockquote>
    <h3><strong>{{ event.title }}</strong></h3>

    <p><strong>Date:</strong> {{ event.date | date: "%m/%d/%Y" }}</p>

    <p><strong>Speakers:</strong> {{ event.speakers }}</p>

    <p><strong>Abstract:</strong></p>
    <p>{{ event.content | markdownify }}</p>
</blockquote>
<br>
<hr>
<br>
{% endfor %}