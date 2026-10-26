---
title: ''
date: 2026-10-20
type: landing
sections:
  - block: resume-biography-3
    content:
      username: me
      text: ''
      headings:
        about: "About"
        education: "Education"
        interests: "Research interests"
    design:
      css_class: hb-hero dark
      background:
        gradient_mesh:
          enable: true
      name:
        size: md
      avatar:
        size: medium
        shape: circle
  - block: collection
    id: reflexions
    content:
      title: "Latest reflections"
      count: 5
      filters:
        folders:
          - reflexions
      archive:
        enable: true
        text: "All reflections"
        link: reflexions/
    design:
      view: date-title-summary
      css_class: hb-refl
  - block: stats
    content:
      title: "At a glance"
      items:
        - statistic: "4"
          description: "Articles in scientific journals"
          sub_metric: "2014 – 2025"
          icon: hero/document-text
        - statistic: "6"
          description: "Conference and seminar contributions"
          sub_metric: "including 1 international conference"
          icon: hero/presentation-chart-bar
        - statistic: "5"
          description: "Institutional projects and responsibilities"
          sub_metric: "CDC, TAWDIF, Entrepreneurship House…"
          icon: hero/building-library
        - statistic: "HDR"
          description: "Habilitation to supervise research"
          sub_metric: "University of Algiers 3"
          icon: hero/academic-cap
    design:
      layout: cards
      css_class: hb-stats dark
  - block: markdown
    content:
      title: "My research"
      text: |-
        My research focuses on economic development and North–South regional integration policies. My doctoral thesis analysed the partnership between Algeria and the European Union and the Algerian economy's transition to a market economy; I then studied the effects of the Association Agreement on Algeria's foreign trade and the country's policy for attracting foreign direct investment.

        I also work on employment and the labour-market integration of higher-education graduates, on entrepreneurship and SMEs, and on the links between the digital economy and sustainable development.

        I am open to scientific collaboration: please do not hesitate to contact me.
    design:
      columns: '1'
  - block: collection
    id: publications
    content:
      title: "Recent publications"
      count: 4
      filters:
        folders:
          - publications
      archive:
        enable: true
        text: "All publications"
        link: publications/
    design:
      view: citation
  - block: collection
    id: projets
    content:
      title: "Projects and responsibilities"
      count: 4
      filters:
        folders:
          - projets
    design:
      view: article-grid
      columns: 2
      show_date: false
      show_read_time: false
---
