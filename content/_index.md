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
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      # button:
      #  text: Download CV
      #  url: uploads/resume.pdf
    design:
      css_class: "dark"
      # Customize the section spacing. Order is top, right, bottom, left.
      spacing:
         padding: ['0', '0', '0', '0']
      background:
         gradient_start: '#0d3e61'
         gradient_end: '#125b8f'
         gradient_angle: 45
#        color: black
#        image:
#          # Add your image background to `assets/media/`.
#          filename: stacked-peaks.svg
#          filters:
#            brightness: 1.0
#          size: cover
#          position: center
#          parallax: true
  - block: markdown
    id: research
    content:
      title: 'My Research'
      subtitle: ''
      text: |-
        <p class="text-justify">My research blends methodologies from computer science, design, and decision theory to address challenges that arise in a variety of application areas such as engineering or life sciences.
        These include decision-making under conflicting objectives, parameter space exploration, domain knowledge exploitation, feature engineering for computational support, or analysis of cause-effect relationships.
        I am also interested in how reflections on the practice of crafting visualizations for real-world problems inform the refinement of methods for visualization research.<p>

        <p class="text-justify">If you would like to work with me, please reach out! 
        I am particularly interested in multidisciplinary discussions on human factors, methodological aspects of visualization research, and real-world applications.</p>
    design:
      css_class: "dark:dark"
      columns: '1'
      spacing:
        padding: ['6rem', '2rem', '6rem', '2rem']
  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publications
        featured_only: true
    design:
      css_class: "dark:dark"
      spacing:
        padding: ['6rem', '2rem', '6rem', '2rem']
      view: card
  - block: collection
    content:
      title: Recent Publications
      filters:
        folders:
          - publications
        exclude_featured: false
      archive:
        text: See all publications
    design:
      css_class: "dark:dark"
      view: citation
  - block: collection
    id: talks
    content:
      title: Invited Talks
      filters:
        folders:
          - talks
    design:
      css_class: "dark:dark"
      view: date-title-summary
  - block: collection
    id: teaching
    content:
      title: Teaching
      count: 2
      filters:
        folders:
          - teaching
      archive:
        text: See all courses
    design:
      view: article-grid
      columns: 2
      css_class: "dark:dark"
---
