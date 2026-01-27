---
layout: page
title: Schedule
description: The weekly event schedule.
nav_order: 3
parent: Course Info
---

# Weekly Schedule

## Key Dates
- Self-scheduled midterm (see schedule for the week noted).
- Final project presentations (see schedule).
- Final project write-up due Friday, May 1, 2026 at 11:59 PM.

## Office Hours
- Start Friday, January 30, 2026.
- Monday 3:30 – 4:30 (Bass 109)
- Wednesday 10:00 – 11:00 (Bass 109)
- Friday 2:00 – 3:00 (Bass 109)

{% for schedule in site.schedules %}
{{ schedule }}
{% endfor %}
