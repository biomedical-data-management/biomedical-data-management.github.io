---
layout: list
title: Biomedical Data Management
subtitle: Workshop at VLDB 2026
thumbnail: images/logo.png
summary: |
sections:
    - partial: content
      content:
        page: workshop/background.md
    - title: Invited Speakers
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
    - title: Organizing Team
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
        small: false
        sortBy:
          param: order

links:
  - icon: fa-brands fa-discord
    href: https://discord.gg/mR7Fmh9JtG
    large: true
    label: Chat
  - icon: fa-solid fa-person-chalkboard
    href: '#invited-speakers'
    large: true
    label: Speakers
  - icon: fa-solid fa-location-dot
    href: https://vldb.org/2026/
    large: true
    label: Attend
---
