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

## Google Teaching Assistants (TAs)
{% assign teaching_assistants = site.staffers | where: 'role', 'Teaching Assistant' %}
{% for staffer in teaching_assistants %}
{{ staffer }}
{% endfor %}

## Google University Program Specialist
{% assign u_program_specialist = site.staffers | where: 'role', 'University Program Specialist' %}
{% for staffer in u_program_specialist %}
{{ staffer }}
{% endfor %}