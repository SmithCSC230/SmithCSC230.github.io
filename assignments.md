---
layout: page
title: Assignments
nav_order: 1
parent: Deliverables
description: Assignment handouts and starter files.
has_children: true
---

# Assignments
Assignments for this class take on a number of different flavors: reflections, problems sets, and reading quizzes. These will be managed through Gradescope and Gradiance, both linked below. Please see Moodle for this semester's Gradiance key (which you can use to register for free).

## Important Links
- [Course Gradescope hub](https://www.gradescope.com/courses/1239414)
- [Request a 72-hour extension here](https://docs.google.com/forms/d/e/1FAIpQLSdYfhC5fb3JWVF95fV02CaynFACyYjjUsCVjxDGlU9ZbEbaaQ/viewform?usp=header)
- [Gradiance](https://www.newgradiance.com/services/servlet/COTC)

## Weekly Assignments

{% assign weekly_pages = site.pages | where_exp: "p", "p.parent == 'Assignments'" | where_exp: "p", "p.grand_parent == 'Deliverables'" | sort: "nav_order" %}
{% for p in weekly_pages %}
- [{{ p.title }}]({{ p.url }})
{% endfor %}
