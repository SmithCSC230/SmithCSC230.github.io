---
layout: page
title: Schedule
description: The weekly event schedule.
nav_order: 5
---

# Weekly Schedule

## Midterm Dates and Coverage
Students take midterms asynchronously over the weekend.
- Midterm 1 (Feb 20–22): ADT, Arrays, Loops, Search (linear & binary), Lists, Iterators.
- Midterm 2 (Mar 27–29): Stacks/Queues, Copy Depth, Recursion, Sorting, Binary Tree.
- Midterm 3 (Apr 24–26): Traversal, BST, Heaps, HashMaps, Graphs.

{% for schedule in site.schedules %}
{{ schedule }}
{% endfor %}
