---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
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
      title: Interests
      filters:
        folders:
          - hobbies
    design:
      view: community/main-grid
      columns: 3
      background:
        image:
          # filename: icon.png
          filters:
            # Darken the image? Range 0-1 where 1 is transparent and 0 is opaque.
            brightness: 0.5

  - block: markdown
    content:
      title: Location
      text: <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d306141.380212437!2d126.3453416664724!3d33.3711157139061!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x350ce3544cc84045%3A0x66bc36d2981ebf31!2sJeju-do%2C+South+Korea!5e0!3m2!1sen!2sus!4v1473136714592" width="600" height="450" frameborder="0" style="border:0" allowfullscreen></iframe>

  - block: resume-languages
    content:
      title: Languages
      username: admin

  - block: collection
    content:
      title: Etc.
      filters:
        folders:
          - hobbies_copy
    design:
      view: community/main-grid
      columns: 3
      background:
        image:
          filename: icon.png
          filters:
            # Darken the image? Range 0-1 where 1 is transparent and 0 is opaque.
            brightness: 0.5
---
