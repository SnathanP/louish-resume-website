---
# An instance of the Contact widget.
widget: contact

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 130

title: Contact
subtitle: Restons en contact!

content:
  # Automatically link email and phone or display as text?
  autolink: true

  # Email form provider
  form:
    provider: formspree
    formspree:
      id: xqkjeeab
      captcha: true
      captcha_key: 6LchL9EhAAAAAM92GH24-tGC5xTaST5E-DyvG-1-

  # Contact details (edit or remove options as required)
  email: contact@louis-holleville.fr
  address:
    city: Paris
    region: France
    country: France
    country_code: FR
  contact_links:
    - icon: linkedin
      icon_pack: fab
      name: Démarrez la conversation!
      link: 'https://twitter.com/LouisHolleville'
    - icon: twitter
      icon_pack: fab
      name: Envoyez moi un MP!
      link: 'https://twitter.com/LouisHolleville'
design:
  columns: '2'
---
