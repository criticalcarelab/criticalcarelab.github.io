---
title: Team
nav:
  order: 3
  tooltip: About our team
---

# {% include icon.html icon="fa-solid fa-users" %} Team

Welcome to our team page! Meet the people who make our research possible.

{% include section.html title="Principal Investigators" %}
{% include list.html data="members" component="portrait" filter="role == 'pi'" %}

{% include section.html title="Students / Post-Docs" %}
{% include list.html data="members" component="portrait" filter="role == 'student' or role == 'postdoc'" %}

{% include section.html title="Visiting Researchers" %}
{% include list.html data="members" component="portrait" filter="role == 'visiting'" %}

{% include section.html title="Staff" %}
{% include list.html data="members" component="portrait" filter="role == 'staff'" %}

{% include section.html %}

{% include list.html data="members" component="portrait" filter="role == 'pi'" %}
{% include list.html data="members" component="portrait" filter="role != 'pi'" %}

{% include section.html background="images/background.jpg" dark=true %}

Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor
incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis
nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.

{% include section.html %}

{% capture content %}

{% include figure.html image="images/photo.jpg" %}
{% include figure.html image="images/photo.jpg" %}
{% include figure.html image="images/photo.jpg" %}

{% endcapture %}

{% include grid.html style="square" content=content %}
