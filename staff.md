---
layout: page
title: Staff
description: A listing of all the course staff members.
---

# Staff

For a quicker response on homework or project help, please ask on EdStem rather than emailing staff members individually. On EdStem, all staff members can see your question and answer it.

## Instructors

{% assign instructors = site.staffers | where: 'role', 'Instructor' %}
{% for staffer in instructors %}
{{ staffer }}
{% endfor %}

{% assign teaching_assistants = site.staffers | where: 'role', 'Teaching Assistant' %}
{% assign num_teaching_assistants = teaching_assistants | size %}
{% if num_teaching_assistants != 0 %}
## Google Teaching Assistants (TAs)

{% for staffer in teaching_assistants %}
{{ staffer }}
{% endfor %}
{% endif %}
