---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: markdown
    id: about
    content:
      text: "![img](https://plus.unsplash.com/premium_photo-1667126444822-94fb21279436?q=80&w=2940&auto=format&fit=crop&ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D)"
  - block: community/resume-biography-3-custom
    content:
      # The user's folder name in `content/authors/`
      username: admin
      # Show a call-to-action button under your biography? (optional)
      # To link to a file, upload it to your `static/uploads/` folder
      button:
        text: Résumé
        url: uploads/resume.pdf

  - block: resume-experience
    id: experience
    content:
      username: admin
    design:
      # Hugo date format
      date_format: '2006년 January'
      # Education or Experience section first?
      is_education_first: true

  # - block: resume-skills
  #   content:
  #     title: Skills & Hobbies
  #     username: admin
  #   design:
  #     show_skill_percentage: true

  - block: collection
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - projects
    design:
      view: community/project-grid
      columns: 3 
      
  - block: collection
    content:
      title: Activities
      filters:
        folders:
          - activities
    design:
      view: community/project-grid
      columns: 3
      background:
        image:
          # filename: icon.png
          filters:
            # Darken the image? Range 0-1 where 1 is transparent and 0 is opaque.
            brightness: 0.5

  - block: collection
    content:
      title: 🎶
      filters:
        folders:
          - etc
    design:
      view: community/main-grid
      columns: 3

  - block: markdown
    content:
      title: Location
      text: <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d3234.3010662434363!2d128.56395901107965!3d35.84162057242138!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x3565e49dd28209e7%3A0x83734ac8a26bd9f1!2z64yA7ZWc66-86rWtIOuMgOq1rOq0keyXreyLnCDrgqjqtawg64yA66qF67O16rCc66GcIDE0NC0y!5e0!3m2!1sko!2sus!4v1727252752562!5m2!1sko!2sus" width="600" height="450" style="border:0;" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade"></iframe>

  - block: resume-languages
    content:
      title: Languages
      username: admin

      # Image Slider with upsplash images at least 3
      # Text overlay also
      
  # - block: slider
  #   content:
  #     slides:
  #     - title: 👋 Welcome to the group
  #       content: Take a look at what we're working on...
  #       align: center
  #       background:
  #         image:
  #           filename: contact.jpg
  #           filters:
  #             brightness: 0.7
  #         position: right
  #         color: '#666'
  #     - title: Lunch & Learn ☕️
  #       content: 'Share your knowledge with the group and explore exciting new topics together!'
  #       align: left
  #       background:
  #         image:
  #           filename: contact.jpg
  #           filters:
  #             brightness: 0.7
  #         position: center
  #         color: '#555'
  #     - title: World-Class Semiconductor Lab
  #       content: 'Just opened last month!'
  #       align: right
  #       background:
  #         image:
  #           filename: contact.jpg
  #           filters:
  #             brightness: 0.5
  #         position: center
  #         color: '#333'
  #   design:
  #     # Slide height is automatic unless you force a specific height (e.g. '400px')
  #     slide_height: ''
  #     is_fullscreen: true
  #     # Automatically transition through slides?
  #     loop: false
  #     # Duration of transition between slides (in ms)
  #     interval: 2000
  - block: community/slider
---
