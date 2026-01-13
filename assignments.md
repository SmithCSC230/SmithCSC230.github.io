---
layout: page
title: Assignments
nav_order: 6
description: Assignment handouts and starter files.
---

# Assignments

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
