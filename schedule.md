---
layout: page
title: Schedule
description: The weekly event schedule.
nav_order: 5
---

# Weekly Schedule

## Key Dates
- Self-scheduled midterm (see schedule for the week noted).
- Final project presentations (see schedule).
- Final project write-up due Friday, May 1, 2026 at 11:59 PM.

{% for schedule in site.schedules %}
{{ schedule }}
{% endfor %}
