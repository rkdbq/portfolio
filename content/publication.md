---
title: Publications
type: landing

# cascade:
#   - _target:
#       kind: page
#     params:
#       show_breadcrumb: true
# cms_exclude: true

# # View.
# view: citation

# # Optional header image (relative to `static/media/` folder).
# banner:
#   caption: ''
#   image: ''

sections:
  - block: collection
    content:
      title: International Journal
      text: ""
      filters:
        folders:
          - journals-international
        exclude_featured: false
    design:
      view: citation
  
  - block: collection
    content:
      title: Domestic Journal
      text: ""
      filters:
        folders:
          - journals-domestic
        exclude_featured: false
    design:
      view: citation
---
