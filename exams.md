---
layout: page
title: Exams
nav_order: 2
parent: Deliverables
description: Past exams and answer keys.
---

# Exams

The take-home exam is due Thursday, March 12, 2026.

## Past exams

{% assign exam_files = site.static_files | where_exp: "file", "file.path contains '/content/Exams/'" %}
{% assign exam_pdfs = exam_files | where_exp: "file", "file.extname == '.pdf'" %}

{% if exam_pdfs.size > 0 %}
{% for file in exam_pdfs %}
- [{{ file.name }}]({{ file.path }})
{% endfor %}
{% else %}
Exams will be posted here.
{% endif %}
