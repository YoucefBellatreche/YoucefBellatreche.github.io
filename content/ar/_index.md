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
        about: "نبذة"
        education: "التكوين الجامعي"
        interests: "مجالات البحث"
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
      title: "أحدث التأملات"
      count: 5
      filters:
        folders:
          - reflexions
      archive:
        enable: true
        text: "جميع التأملات"
        link: reflexions/
    design:
      view: date-title-summary
      css_class: hb-refl
  - block: stats
    content:
      title: "في أرقام"
      items:
        - statistic: "4"
          description: "مقالات منشورة في مجلات علمية"
          sub_metric: "2014 – 2025"
          icon: hero/document-text
        - statistic: "6"
          description: "مداخلات في ملتقيات وأيام دراسية"
          sub_metric: "منها ملتقى دولي واحد"
          icon: hero/presentation-chart-bar
        - statistic: "5"
          description: "مشاريع ومسؤوليات مؤسساتية"
          sub_metric: "CDC، TAWDIF، دار المقاولاتية…"
          icon: hero/building-library
        - statistic: "HDR"
          description: "التأهيل الجامعي"
          sub_metric: "جامعة الجزائر 3"
          icon: hero/academic-cap
    design:
      layout: cards
      css_class: hb-stats dark
  - block: markdown
    content:
      title: "أبحاثي"
      text: |-
        تتمحور أبحاثي حول التنمية الاقتصادية وسياسات التكامل الإقليمي بين الشمال والجنوب. تناولت أطروحتي للدكتوراه الشراكة بين الجزائر والاتحاد الأوروبي وانتقال الاقتصاد الجزائري نحو اقتصاد السوق، ثم درستُ آثار اتفاق الشراكة على التجارة الخارجية الجزائرية وسياسة جذب الاستثمارات الأجنبية المباشرة.

        كما أهتم بالتشغيل والإدماج المهني لخريجي التعليم العالي، وبالمقاولاتية والمؤسسات الصغيرة والمتوسطة، وبالعلاقة بين الاقتصاد الرقمي والتنمية المستدامة.

        أنا منفتح على التعاون العلمي: لا تترددوا في التواصل معي.
    design:
      columns: '1'
  - block: collection
    id: publications
    content:
      title: "أحدث المنشورات"
      count: 4
      filters:
        folders:
          - publications
      archive:
        enable: true
        text: "جميع المنشورات"
        link: publications/
    design:
      view: citation
  - block: collection
    id: projets
    content:
      title: "المشاريع والمسؤوليات"
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
