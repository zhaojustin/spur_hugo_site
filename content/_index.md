---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

sections:
  # About Us section
  - block: about.biography
    id: about
    design:
      spacing:
        padding: ["50px", "0", "50px", "0"]
    content:
      title: Biography
      username: admin

  # Affiliates section
  - block: experience
    id: affiliates
    content:
      title: Affiliates
      subtitle: subtitle?
      text: |-
        {{< teamSection >}}
      count: 1
    design:
      columns: "2"

  # Talks section
  - block: collection
    id: talks
    content:
      title: Upcoming and Past Talks
      subtitle: ""
      text: ""
      # Choose how many pages you would like to display (0 = all pages)
      count: 0
      # Filter on criteria
      filters:
        folders:
          - event
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: compact
      columns: "2"

  # Publications - COMMENTED OUT FOR NOW
  - block: collection
    id: publications
    content:
      title: Publications
      filters:
        folders:
          - publication
        featured_only: false
        count: 0
    design:
      columns: "2"
      view: card

  # Working Papers - COMMENTED OUT FOR NOW
  - block: collection
    id: papers
    content:
      title: Working Papers
      filters:
        folders:
          - post
        featured_only: false
        count: 0
    design:
      columns: "2"
      view: card

  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam mi diam, venenatis ut magna et, vehicula efficitur enim.
      # Contact (add or remove contact options as necessary)
      email: test@example.org
      phone: 888 888 88 88
      appointment_url: "https://calendly.com"
      address:
        street: 450 Serra Mall
        city: Stanford
        region: CA
        postcode: "94305"
        country: United States
        country_code: US
      directions: Enter Building 1 and take the stairs to Office 200 on Floor 2
      office_hours:
        - "Monday 10:00 to 13:00"
        - "Wednesday 09:00 to 10:00"
      # Choose a map provider in `params.yaml` to show a map from these coordinates
      coordinates:
        latitude: "37.4275"
        longitude: "-122.1697"
      contact_links:
        - icon: twitter
          icon_pack: fab
          name: DM Me
          link: "https://twitter.com/Twitter"
        - icon: skype
          icon_pack: fab
          name: Skype Me
          link: "skype:echo123?call"
        - icon: video
          icon_pack: fas
          name: Zoom Me
          link: "https://zoom.com"
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
      columns: "2"
---
