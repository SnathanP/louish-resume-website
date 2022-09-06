---
# An instance of the Experience widget.
# Documentation: https://wowchemy.com/docs/page-builder/
widget: experience

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 40

title: Experience
subtitle:

# Date format for experience
#   Refer to https://wowchemy.com/docs/customization/#date-format
date_format: Jan 2006

# Experiences.
#   Add/remove as many `experience` items below as you like.
#   Required fields are `title`, `company`, and `date_start`.
#   Leave `date_end` empty if it's your current employer.
#   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
experience:
  - title: Site Reliability Engineer
    company: WeMaintain
    company_url: 'https://wemaintain.com/'
    company_logo: wemaintain
    location: Paris, France
    date_start: '2022-01-01'
    date_end: ''
    description: |2-
      It is going pretty well :)
  - title: DevOps Engineer
    company: ViaSema
    company_url: 'https://www.viasema.com/'
    company_logo: viasema
    location: Paris, France
    date_start: '2021-02-01'
    date_end: '2022-01-01'
    description: |2-
      Rationalization of business and internal processes of VIASEMA:
      - implementation of the industrial approach and DevSecOps transformation.
      - team and structural evangelism
      - infrastructure architecture, negotiations with cloud partners and deployment of hybrid fleet (Azure).
      - implementation of delivery chain and continuous deployment (Gitlab-CI, kubernetes, Docker, Helm).
      - network architecture, flow security policy and access control.
      - introduction of metrology and alerting strategies (prometheus, grafana, logstash, datadog). Also at the origin of organizational and managerial change, team cohesion, agile approach and openness to knowledge.
  - title: Teaching Assistant
    company: EPITA
    company_url: 'https://www.groupe-pomona.fr/en'
    company_logo: epita
    location: Paris, France
    date_start: '2020-02-01'
    date_end: '2020-12-01'
    description: |2-
      As a teaching assistant, I was in charge, with the team, to ensure programmation lectures to first years students in C, Java and C++
  - title: DevOps Intern
    company: Groupe POMONA
    company_url: 'https://www.groupe-pomona.fr/en'
    company_logo: pomona
    location: Antony, France
    date_start: '2019-09-01'
    date_end: '2020-01-15'
    description: |2-
      Participation in the IT industrialization process:
      - Implementation of the CI/CD/CT chain of the Pomona Group (GitLab, Jenkins, Ansible, Terraform, SonarQube)
      - Definition, evangelization and reference point of good DevOps practices for the group's IT department
      - Definition and implementation of architectural standards and technical rules of the delivery chain
      - Participation in the definition of the environment management strategy
      - Implementation and support of the first Azure-based solutions and chains
      - Participate in the organizational transition and the evolution of working methods [Agile/Scrum]
      - Participation in the design and construction of the internal CaaS platform (Rancher/Kubernetes)
      - Implementation of the first metrology solution (E.L.K, Prometheus & Grafana) infrastructure

design:
  columns: '2'
---
