---
title: ArgoCD in production at WeMaintain !
subtitle: For some time now at WeMaintain, ArgoCD has been around, spreading projects throught projects. Since this Monday, it is now used for production apps! But to what extent?

# Summary for listings and search engines
summary: 
# Link this post with a project
projects:
- gitops at wemaintain

# Date published
date: '2022-08-28T16:00:00Z'

# Date updated
lastmod: '2022-08-28T16:00:00Z'

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: Photo by [Liquidbase](https://www.liquibase.com/gitops-database)
  focal_point: ''
  placement: 2
  preview_only: false

authors:
  - admin

tags:
  - gitops
  - wemaintain

categories:
  - DevSecOps
---

Pourquoi ne pas gérer son SI tel un produit métier ?
Consommateurs, clients, fournisseurs, MVP, stakeholders, planification; plus j’y réfléchis et plus j’y vois de notions communes.

Tout ce qui nous manquait serait donc le lien entre la théorie et la pratique ?

Plus tellement désormais: Infrastructure as Code, Network as Code, DevOps et maintenant #gitops, tous ces concepts prennent forme au travers de solutions telles Terraform, Istio, Ansible, Argo et tant d’autres. 
Mis bout-à-bout, l’évolution d’un SI est désormais complètement possible au travers du code, comme un projet dans son ensemble, et peut lui-même être sujet à de l’automatisation de son déploiement (InfraOps donc? :p). L’infrastructure devient réactive. Les technologies cloud nous permettent désormais une grande flexibilité, nous ne sommes plus dans l’anticipation à quelques années mais dans la réaction à quelques minutes. L’infra devient apparente, malléable et peut désormais suivre de prêt les besoins métiers.
Ses processus d’exploitation sont automatisables et rationalisables, en maximisant la répétabilité et réduisant le facteur humain, le rêve. CI over GitOps, canary et blue-green permettent même désormais un workflow  de livraison automatisé, de la plus petite intégration à la mise en prod.
Et le plus important, d’autres personnes ont désormais cette possibilité de consulter ce “nouveau” code, d’y contribuer, de le questionner et d’y apporter une vision fraîche, naïve, vitale.

Ayant posé la première brique GitOps à WeMaintain la semaine dernière, je me réjouis déjà de constater la confiance grandissante dans nos process et suis impatient de pouvoir aller encore plus loin. Et, je dois dire, c’est un réel plaisir de travailler dans un milieu qui vise aussi loin et s’en donne les moyens.