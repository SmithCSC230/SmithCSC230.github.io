---
layout: page
title: Assignments
nav_order: 7
description: Assignment handouts and starter files.
---

# Assignments

## Important Links
- [Course Gradescope hub] (https://www.gradescope.com/courses/1225360)
- [Request a 72-hour extension here](https://docs.google.com/forms/d/e/1FAIpQLSc3QMRpoOr5WqiYz2cQlBssQPz4uA9wtlrXh5H2VrlfYfsfrg/viewform?usp=header)

## Assignment bundles

{% assign assignment_files = site.static_files | where_exp: "file", "file.path contains '/content/Assignments/'" %}
{% assign assignment_zips = assignment_files | where_exp: "file", "file.extname == '.zip'" %}

{% if assignment_zips.size > 0 %}
{% for file in assignment_zips %}
- [{{ file.name }}]({{ file.path }})
{% endfor %}
{% else %}
Assignments will be posted here.
{% endif %}

## Assignment summaries

- [Assignment summaries](content/Assignments/summaries/)
