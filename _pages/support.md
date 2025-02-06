---
layout: page
title: Support
permalink: /support/
nav: true
nav_order: 2
#dropdown: true
#children:
#  - title: Getting Help
#    permalink: get_help
#  - title: Preliminaries
#    permalink: preliminaries
#  - title: Introduction to using a compute cluster
#    permalink: cluster_tutorial
#  - title: Open OnDemand(OOD)
#    permalink: ood_tutorial
#  - title: Globus
#    permalink: globus_tutorial
#  - title: Introduction to the Linux command-line
#    permalink: linux_tutorial
---

## Research Computing Support

Need help getting access to the compute cluster? Having issues with scheduling a job on the cluster? Want a refresher on Linux or high-performance computing? The research computing team is here to help! You can sign up for a consultation with one of our team members, attend a training course, or browse our documentation.

<div class="projects">

<!-- Display projects without categories -->

{% assign sorted_projects = site.support | sort: "importance" %}

  <!-- Generate cards for each project -->

{% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-1 row-cols-md-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.liquid %}
    {% endfor %}
    </div>
  </div>
{% else %}
  <div class="row row-cols-1 row-cols-md-3">
    {% for project in sorted_projects %}
      {% include projects.liquid %}
    {% endfor %}
  </div>
{% endif %}
</div>
