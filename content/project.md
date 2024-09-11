---
title: Projects
type: landing

cascade:
  - _target:
      kind: page
    params:
      show_breadcrumb: true

sections:
  - block: collection
    content:
      title: Projects
      filters:
        folders:
          - projects
    design:
      view: article-grid
      columns: 2

  - block: collection
    content:
      title: Research
      filters:
        folders:
          - research
    design:
      view: article-grid
      columns: 2
---
