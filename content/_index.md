---
layout: list
title: Biomedical Data Management
subtitle: Workshop at VLDB 2026
thumbnail: images/logo.png
summary: |
  Community of biomedical informatics and data management researchers and practitioners who engage in
  collaborative efforts to identify emerging problem areas, develop novel solutions and help accelerate
  the pace of innovation in healthcare.
sections:
    - title: Speakers
      partial: list
      content:
        page: people
        param: pages
        where:
          key: Params.groups
          operator: intersect
          match:
            - invited
      params:
        preventTitleLinks: true
        small: false
        sortBy:
          param: order
    - partial: content
      content:
        page: workshop/program.md
    - partial: content
      content:
        page: workshop/contribute.md
    - partial: content
      content:
        page: workshop/about.md
    - title: Organizers
      partial: list
      content:
        page: people
        param: pages
        where:
          key: Params.groups
          operator: intersect
          match:
            - organizer
      params:
        preventTitleLinks: true
        small: true
        sortBy:
          param: order

links:
  - icon: fa-brands fa-discord
    href: https://discord.gg/mR7Fmh9JtG
    large: true
    label: Chat
  # - icon: fa-solid fa-person-chalkboard
  #   href: '#invited-speakers'
  #   large: true
  #   label: Speakers
  - icon: fa-solid fa-location-dot
    href: https://vldb.org/2026/
    large: true
    label: Attend
---
