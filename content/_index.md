---
# Leave the homepage title empty to use the site title
title:
date: 2023-04-13
type: landing

sections:
  - block: about.avatar
    id: about
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      # Override your bio text from `authors/admin/_index.md`?
      text:
  #- block: features
  #  content:
  #    title: Skills
  #    items:
  #      - name: R
  #        description: 90%
  #        icon: r-project
  #        icon_pack: fab
  #      - name: Statistics
  #        description: 100%
  #        icon: chart-line
  #        icon_pack: fas
  #      - name: Photography
  #        description: 10%
  #        icon: camera-retro
  #        icon_pack: fas
  - block: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: PhD student in Computer sciences
          company: University of Clermont-Auvergne
          company_url: 'https://www.uca.fr/'
          company_logo: logo_uca.png
          location: Aurillac
          date_start: '2022-10-01'
          date_end: '2025-10-01'
          description: |2-
              * Research in network security and cryptography
              * Teaching
        - title: Intern in cryptology
          company: Harmonic
          company_url: 'https://www.harmonicinc.com/'
          company_logo: org-x
          location: Cesson Sévigné (France)
          date_start: '2022-03'
          date_end: '2022-08'
          description: Implementation of a cryptographic toolkit to protect the sensitive data of the products in the video chain.   
        - title: Intern in data engineering
          company: Veolia Nordics
          company_url: 'https://www.veolia.com'
          company_logo: org-x
          location: Stockholm (Sweden)
          date_start: '2020-06'
          date_end: '2020-08'
          description: Data studies of unpaid invoices and profit and loss in order to produce reports that meet customer needs.
        - title: Intern in data science
          company: Veolia S.A.
          company_url: 'https://www.veolia.com'
          company_logo: org-x
          location: Paris (France)
          date_start: '2019-06'
          date_end: '2019-07'
          description: Study of time series on water data in order to forecast water consumption and detect leaks in the drinkable water network.
        - title: Intern in computer science applied to neuroscience
          company: Paris Descartes University
          company_url: 'https://u-paris.fr/en/'
          company_logo: org-x
          location: Paris (France)
          date_start: '2017-06'
          date_end: '2017-07'
          description: |2-
              Angle calculation and motion recording with Codamotion software.
              Training workshop on virtual reality to study and heal the brain.
        - title: Intern in netwrok
          company: Paris Diderot University
          company_url: 'https://u-paris.fr/en/'
          company_logo: org-x
          location: Paris (France)
          date_start: '2016-06'
          date_end: '2016-06'
          description: |2-
              Installation and administration of experimental routers using Babel and HNCP (Home Networking Control Protocol) protocols.
              (presentation during the IETF 96 in Berlin in July 2016 by Juliusz Chroboczek)
              
              
    design:
      columns: '2'
  - block: accomplishments
    content:
      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
      title: 'Accomplish&shy;ments'
      subtitle:
      # Date format: https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Accomplishments.
      #   Add/remove as many `item` blocks below as you like.
      #   `title`, `organization`, and `date_start` are the required parameters.
      #   Leave other parameters empty if not required.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - certificate_url: https://www.coursera.org
          date_end: ''
          date_start: '2021-01-25'
          description: ''
          organization: Coursera
          organization_url: https://www.coursera.org
          title: Neural Networks and Deep Learning
          url: ''
        - certificate_url: https://www.edx.org
          date_end: ''
          date_start: '2021-01-01'
          description: Formulated informed blockchain models, hypotheses, and use cases.
          organization: edX
          organization_url: https://www.edx.org
          title: Blockchain Fundamentals
          url: https://www.edx.org/professional-certificate/uc-berkeleyx-blockchain-fundamentals
        - certificate_url: https://www.datacamp.com
          date_end: '2020-12-21'
          date_start: '2020-07-01'
          description: ''
          organization: DataCamp
          organization_url: https://www.datacamp.com
          title: 'Object-Oriented Programming in R'
          url: ''
    design:
      columns: '2'
  - block: collection
    id: posts
    content:
      title: Recent Posts
      subtitle: ''
      text: ''
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        folders:
          - post
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: compact
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
  - block: markdown
    content:
      title: Gallery
      subtitle: ''
      text: |-
        {{< gallery album="demo" >}}
    design:
      columns: '1'
  - block: collection
    id: featured
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: collection
    content:
      title: Recent Publications
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
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
  - block: tag_cloud
    content:
      title: Popular Topics
    design:
      columns: '2'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        If you want more information or have questions you can contact through the follwing form:
      # Contact (add or remove contact options as necessary)
      email: dorine.chagnon@doctorant.uca.fr
      #phone: 888 888 88 88
      appointment_url: 'https://calendly.com'
      address:
        street: 100 rue de l'Egalité
        city: Aurillac
        region: Cantal
        postcode: '15000'
        country: France
        country_code: FR
      directions: Departement of data science and cybersecurity, Phd student office
      #office_hours:
      #  - 'Monday 10:00 to 13:00'
      #  - 'Wednesday 09:00 to 10:00'
      #contact_links:
        #- icon: twitter
        #  icon_pack: fab
        #  name: DM Me
        #  link: 'https://twitter.com/Twitter'
        #- icon: skype
        #  icon_pack: fab
        #  name: Skype Me
        #  link: 'skype:echo123?call'
        #- icon: video
        #  icon_pack: fas
        #  name: Zoom Me
        #  link: 'https://zoom.com'
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
