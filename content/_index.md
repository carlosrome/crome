---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: experience
    content:
      title: Work Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Physics Lab Assistant
          company: Elmhurst University
          company_url: 'https://www.elmhurst.edu/academics/departments/physics/'
          company_logo: elmhurst
          location: Illinois
          date_start: '2023-08-28'
          date_end: ''
          description: |2-
              Responsibilities include:

              * Setting up the experiments
              * Overseeing student's progress
        - title: Mathematics Teacher Assistant ELSA Program
          company: Elmhurst University
          company_url: 'https://www.elmhurst.edu/academics/elmhurst-learning-success-academy/'
          company_logo: elmhurst
          location: Illinois
          date_start: '2022-08-29'
          date_end: ''
          description: |2-
              Responsibilities include:

              * Grading
              * Guiding students
    
        - title: Physics and Mathematics tutor
          company: Elmhurst University
          company_url: 'https://www.elmhurst.edu/academics/academic-centers/the-learning-center/'
          company_logo: elmhurst
          location: Illinois
          date_start: '2021-08-30'
          date_end: ''
          description: Provided tutoring for advanced physics and mathematics courses at the university's Learning Center.
    design:
      columns: '2'
    
  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: All
          tag: '*'
        - name: Deep Learning
          tag: Deep Learning
        - name: Other
          tag: Demo
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: collection
    id: featured
    content:
      title: Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: collection
    content:
      title: Conferences
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation

  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
      email: carlos.romerome@outlook.com
      phone: 331 243 38 66
      address:
        street: 190 S Prospect Avenue 
        city: Elmhurst
        region: IL
        postcode: '60126'
        country: United States
        country_code: US


      # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '2'
---
