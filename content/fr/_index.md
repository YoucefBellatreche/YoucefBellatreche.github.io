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
        about: "Présentation"
        education: "Formation"
        interests: "Domaines de recherche"
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
      title: "Dernières réflexions"
      count: 5
      filters:
        folders:
          - reflexions
      archive:
        enable: true
        text: "Toutes les réflexions"
        link: reflexions/
    design:
      view: date-title-summary
      css_class: hb-refl
  - block: stats
    content:
      title: "En quelques chiffres"
      items:
        - statistic: "4"
          description: "Articles publiés dans des revues scientifiques"
          sub_metric: "2014 – 2025"
          icon: hero/document-text
        - statistic: "6"
          description: "Communications en colloques et séminaires"
          sub_metric: "dont 1 colloque international"
          icon: hero/presentation-chart-bar
        - statistic: "5"
          description: "Projets et responsabilités institutionnelles"
          sub_metric: "CDC, TAWDIF, Maison de l'entrepreneuriat…"
          icon: hero/building-library
        - statistic: "HDR"
          description: "Habilitation à diriger des recherches"
          sub_metric: "Université Alger 3"
          icon: hero/academic-cap
    design:
      layout: cards
      css_class: hb-stats dark
  - block: markdown
    content:
      title: "Mes recherches"
      text: |-
        Mes travaux portent sur le développement économique et les politiques d'intégration régionale Nord-Sud. Ma thèse de doctorat a analysé le partenariat entre l'Algérie et l'Union européenne et la transition de l'économie algérienne vers l'économie de marché ; j'ai ensuite étudié les effets de l'accord d'association sur le commerce extérieur algérien et la politique d'attraction des investissements directs étrangers.

        Je m'intéresse aussi à l'emploi et à l'insertion professionnelle des diplômés de l'enseignement supérieur, à l'entrepreneuriat et aux PME, ainsi qu'aux liens entre économie numérique et développement durable.

        Je suis ouvert aux collaborations scientifiques : n'hésitez pas à me contacter.
    design:
      columns: '1'
  - block: collection
    id: publications
    content:
      title: "Publications récentes"
      count: 4
      filters:
        folders:
          - publications
      archive:
        enable: true
        text: "Toutes les publications"
        link: publications/
    design:
      view: citation
  - block: collection
    id: projets
    content:
      title: "Projets et responsabilités"
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
