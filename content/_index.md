---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # The user's folder name in `content/authors/`
      username: admin_bio
      # Show a call-to-action button under your biography? (optional)
      # To link to a file, upload it to your `static/uploads/` folder
      button:
        text: Résumé
        url: uploads/resume.pdf

  - block: resume-experience
    id: experience
    content:
      username: admin_spec
    design:
      # Hugo date format
      date_format: '2006 January'
      # Education or Experience section first?
      is_education_first: true

  # - block: resume-skills
  #   content:
  #     title: Skills & Hobbies
  #     username: admin
  #   design:
  #     show_skill_percentage: true

  - block: resume-languages
    content:
      title: Languages
      username: admin_spec
---
