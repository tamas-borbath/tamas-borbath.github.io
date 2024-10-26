---
# Leave the homepage title empty to use the site title
title: ''
date: 2023-10-30
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  # - block: skills
  #   content:
  #     title: Skills
  #     text: ''
  #     # Choose a user to display skills from (a folder name within `content/authors/`)
  #     username: admin
  #   design:
  #     columns: '1'
  #- block: markdown
  #  content:
  #    title: Recent News
  #    subtitle: My subtitle
  #    text: |2-
  #      Add any **markdown** formatted content here - text, images, videos, galleries - and even HTML code!
  #        Responsibilities include:
#
#            * Analysing
#            * Modelling
#            * Deploying
#    design:
#      # See Page Builder docs for all section customization options.
#      # Choose how many columns the section has. Valid values: '1' or '2'.
#      columns: '2'
  - block: markdown
    id: news
    content:
      title: Recent News
      subtitle: '[Archived news](news/)'
      text: |-
        {{< readfromfile "/content/newslist.dat" 3 >}} 
    design:
      columns: '2'
  - block: experience
    content:
      title: Experience
      id: experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Senior Service Engineer
          company: Coreso
          company_url: 'https://www.coreso.eu'
          company_logo: org-coreso
          location: Brussels, BE
          date_start: '2024-10-01'
          date_end: ''
          description: I am working on developing coordination services for European Transmission System Operators.
        - title: Researcher
          company: KU Leuven and EnergyVille
          company_url: 'https://www.esat.kuleuven.be/electa'
          company_logo: org-kuleuven
          location: Leuven, BE
          date_start: '2019-09-01'
          date_end: '2024-09-30'
          description: I am researching Transmission Grids and Resource Adequacy at the [Electrical Energy & Computer Architectures (ELECTA)](https://www.esat.kuleuven.be/electa') research group of KU Leuven and the [Decision Support for Transmission Networks team of ETCH Energyville](https://www.energyville.be/en/research/electrical-networks).
        - title: Application Lead
          company: ENTSO-E Digital Section
          company_url: 'https://www.entsoe.eu'
          company_logo: org-entsoe
          location: Brussels, BE
          date_start: '2018-07-01'
          date_end: '2019-08-31'
          description: I coordinated the operation and development of shared big data platforms for [market](https://transparency.entsoe.eu) and [statistical data](https://www.entsoe.eu/publications/statistics-and-data/) of European power system actors.
        - title: Subject Matter Expert (multiple positions)
          company: GE Digital Energy
          company_url: 'https://www.ge.com/digital/applications/transmission/'
          company_logo: org-ge
          location: Bucharest, RO & Redmond, WA
          date_start: '2014-11-01'
          date_end: '2018-07-01'
          description: I specialized in data-intensive digital solutions for power system operators. Worked with 20+ utilities from 5 continents and contributed code and design to [GE's Advanced EMS Platform](https://www.ge.com/digital/applications/transmission/advanced-energy-management-system-aems) and Network Model Manager.
    design:
      columns: '2'
  # - block: accomplishments
  #   content:
  #     # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
  #     title: 'Accomplish&shy;ments'
  #     subtitle:
  #     # Date format: https://wowchemy.com/docs/customization/#date-format
  #     date_format: Jan 2006
  #     # Accomplishments.
  #     #   Add/remove as many `item` blocks below as you like.
  #     #   `title`, `organization`, and `date_start` are the required parameters.
  #     #   Leave other parameters empty if not required.
  #     #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
  #     items:
  #       - certificate_url: https://www.coursera.org
  #         date_end: ''
  #         date_start: '2021-01-25'
  #         description: ''
  #         organization: Coursera
  #         organization_url: https://www.coursera.org
  #         title: Neural Networks and Deep Learning
  #         url: ''
  #       - certificate_url: https://www.edx.org
  #         date_end: ''
  #         date_start: '2021-01-01'
  #         description: Formulated informed blockchain models, hypotheses, and use cases.
  #         organization: edX
  #         organization_url: https://www.edx.org
  #         title: Blockchain Fundamentals
  #         url: https://www.edx.org/professional-certificate/uc-berkeleyx-blockchain-fundamentals
  #       - certificate_url: https://www.datacamp.com
  #         date_end: '2020-12-21'
  #         date_start: '2020-07-01'
  #         description: ''
  #         organization: DataCamp
  #         organization_url: https://www.datacamp.com
  #         title: 'Object-Oriented Programming in R'
  #         url: ''
  #   design:
  #     columns: '2'
  # - block: portfolio
  #   id: projects
  #   content:
  #     title: Projects
  #     filters:
  #       folders:
  #         - project
  #     # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
  #     default_button_index: 0
  #     # Filter toolbar (optional).
  #     # Add or remove as many filters (`filter_button` instances) as you like.
  #     # To show all items, set `tag` to "*".
  #     # To filter by a specific tag, set `tag` to an existing tag name.
  #     # To remove the toolbar, delete the entire `filter_button` block.
  #     buttons:
  #       - name: All
  #         tag: '*'
  #       - name: Deep Learning
  #         tag: Deep Learning
  #       - name: Other
  #         tag: Demo
  #   design:
  #     # Choose how many columns the section has. Valid values: '1' or '2'.
  #     columns: '1'
  #     view: showcase
  #     # For Showcase view, flip alternate rows?
  #     flip_alt_rows: false
  # - block: collection
  #   id: featured
  #   content:
  #     title: Featured Publications
  #     filters:
  #       folders:
  #         - publication
  #       featured_only: true
  #   design:
  #     columns: '2'
  #     view: card
  - block: collection
    id: publications
    content:
      title: Recent Publications
      # text: |-
      #   {{% callout note %}}
      #   Quickly discover relevant content by [filtering publications](./publication/).
      #   {{% /callout %}}
      #count: 3
      filters:
        folders:
          - publication
        exclude_featured: false
      # archive:
      #   enable: true
      #   text: See all my publications
      #   link: publication/
    design:
      columns: '2'
      view: citation
  # - block: collection
  #   id: talks
  #   content:
  #     title: Recent & Upcoming Talks
  #     filters:
  #       folders:
  #         - event
  #   design:
  #     columns: '2'
  #     view: compact
  # # - block: tag_cloud
  #   content:
  #     title: Popular Topics
  #   design:
  #     columns: '2'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: ''
      # Contact (add or remove contact options as necessary)
      email: me@tamas-borbath.eu
      phone: 
      appointment_url: 
      address:
        street: 
        city: Leuven
        region: 
        postcode: '3001'
        country: Belgium
        country_code: BE
      directions:
      office_hours:
      contact_links:
        - icon: twitter
          icon_pack: fab
          name: DM Me
          link: 'https://twitter.com/tamasborbath'
        # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      # form:
      #   provider: netlify
      #   formspree:
      #     id:
      #   netlify:
      #     # Enable CAPTCHA challenge to reduce spam?
      #     captcha: false
    design:
      columns: '2'
---
