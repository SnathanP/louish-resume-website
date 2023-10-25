---
# An instance of the Experience widget.
# Documentation: https://wowchemy.com/docs/page-builder/
widget: experience

# This file represents a page section.
headless: true

# Order that this section appears on the page.
weight: 40

title: Expérience
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
  - title: Ingénieur Cloud
    company: Docaposte
    company_url: 'https://www.docaposte.com/'
    company_logo: docaposte
    location: Ivry-sur-Seine, France
    date_start: '2023-05-01'
    #date_end: 'on going'
    description: |2-
      Création depuis une feuille blanche jusqu'à la réalisation et maintient en condition opérationnel d'une plateforme interne de cloud privé. Intervention sur des secteurs:
      - infrastructure: architecture et configuration des équipements physiques en datacenter
      - réseau: architecture et configuration des équipements physiques en datacenter
      - undercloud: mise en place d'un écosystème underlay nécessaire à l'exploitation d'un cloud privé
      - hypervision: exploitation de suite d'outils orienté hypervision: OpenStack et VMware suite.
      - CMP: déploiement et développement de solution d'interfacage client et d'exploitation des services proposés.
  - title: Site Reliability Engineer
    company: WeMaintain
    company_url: 'https://wemaintain.com/'
    company_logo: wemaintain
    location: Paris, France
    date_start: '2022-01-01'
    date_end: '2023-04-30'
    description: |2-
      Mise en place de l'état de l'art de l'industrie à WeMaintain:
      - création de standard de développement et d'opérationel
      - implémentation du pattern GitOps et évangélisation
      - intégration complète IaC de la plateforme cloud AWS
      - création de la stratégie de risque infrastructure
      - mise en place d'une intégration on-demand, silotée et iso-prod
  - title: Ingénieur DevOps
    company: ViaSema
    company_url: 'https://www.viasema.com/'
    company_logo: viasema
    location: Paris, France
    date_start: '2021-02-01'
    date_end: '2022-01-01'
    description: |2-
      Rationnalisation des processus métiers et internes de VIASEMA:
      - mise en place de l'approche industrielle et de la transformation DevSecOps.
      - évangélisation des équipes et structurelle
      - architecture d'infrastructure, négociations avec des partenaires clouds et déploiement de parc hybride (Azure).
      - mise en place de chaîne de livraison et déploiement continue (Gitlab-CI, kubernetes, Docker, Helm).
      - architecture réseau, politique de sécurisation des flux et contrôle d'accès.
      - introduction de la métrologie et des stratégies d'alerting(prometheus, grafana, logstash, datadog).
      Egalement à l'origine de changement organisationnels et managériaux, cohésion des équipes, approche agile et ouverture de la connaissance.
  - title: Assistant YAKA/ACU
    company: EPITA
    company_url: 'https://www.groupe-pomona.fr/en'
    company_logo: epita
    location: Paris, France
    date_start: '2020-02-01'
    date_end: '2020-12-01'
    description: |2-
      En tant qu'assistant d'enseignement, j'étais en charge, en équipe, d'assurer les cours de programmation aux étudiants de première année en C, Java et C++
  - title: Stagiaire DevOps
    company: Groupe POMONA
    company_url: 'https://www.groupe-pomona.fr/en'
    company_logo: pomona
    location: Antony, France
    date_start: '2019-09-01'
    date_end: '2020-01-15'
    description: |2-
      Participation dans le processus d'industrialisation du SI:
      - Implémentation de la chaine CI/CD/CT du Groupe Pomona (GitLab, Jenkins, Ansible, Terraform, SonarQube)
      - Définition et évangélisation et point de référence des bonnes pratiques DevOps pour la D.S.I du groupe
      - Définition et implémentation des standards d’architecture et des règles techniques de la chaine de livraison
      - Participation à la définition de la stratégie de gestion des environnements
      - Implémentation et prise en des premières solutions et chaines basées Azure
      - Participe la transition organisationnelle et à l’évolution des méthodes de travail [Agile/Scrum]
      - Participation à la conception et construction de la plateforme CaaS interne (Rancher/Kubernetes)
      - Implémentation de la première solution de métrologie (E.L.K, Prometheus & Grafana) infrastructure

design:
  columns: '2'
---
