---
title: Team
nav:
  order: 3
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %} Team

# Welcome to our team page! Meet the people who make our research possible.

{% include section.html %}

## Principal Investigator

{% include list.html data="members" component="portrait" filter="role == 'principal-investigator'" %}

## Visiting Scientists

{% include list.html data="members" component="portrait" filter="role == 'visiting-scientist'" %}

## Postdoctoral Fellows and Students

{% include list.html data="members" component="portrait" filter="role == 'student' or role == 'postdoc'" %}

## Staff

{% include list.html data="members" component="portrait" filter="role == 'staff'" %}

## Alumni

{% include list.html data="members" component="portrait" filter="role == 'alumni'" %}

{% include section.html %}
