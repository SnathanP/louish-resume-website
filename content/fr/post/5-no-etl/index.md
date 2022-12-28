---
title: "AWS: objectif No-ETL"
subtitle: Retour sur un élément central du AWS re:invent 2022
summary: "Lors de l'édition 2022 re:invent, Adam Selipsky, CEO d'AWS, a profité de son créneau pour faire quelques annonces dont une qui m'a particulièrement intéressé: l'objectif No-ETL" 

# Link this post with a project
projects:
- full cloud

# Date published
date: '2022-12-10T14:55:00Z'

# Is this an unpublished draft?
draft: true

# Show this page in the Featured widget?
featured: false

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: Illustration by [Carmine Gallo](https://www.forbes.com/sites/carminegallo)
  focal_point: ''
  placement: 2
  preview_only: false

authors:
  - admin

tags:
- AWS
- re:Invent
- cloud

categories:
  - Cloud Architecture
---

L'ETL est un quasi incontournable des SI. Triple problématiques. Nécessite une solution spécifique. "Nous sommes spécifiques".
Et pourtant la problématique reste la même. Dans le cloud, il n'existait pas de solution managée ou optimisée et certaines solutions réfléchie entièrement en ce sens.
Des exemples d'architecture de DE pouvait alors ressembler à des data streams controllés et complété par des fonctions serveless (type AWS lambdas) dans une pipeline plus ou moins claire.
Cette absence de solution permettant complètement de gérer de A à Z la data permettait lors à des solutions telles databricks de trouver leur essor, proposant une offre de Data enginerring, d'analytics, de ML etc car étant les seules gérant la data de A à Z.
Cela est désormais révolu avec la dernière pierre à l'édifice coeur de la data chez Amazon: le no-ETL.

Sans rentrer dans les détails et nous en annoncons la mise en preview, Selipsky nous introduit la future possibilité de gérer de manière managée les flux en source des DB d'Aurora vers la data warehouse redshift.
Petite cerise sur la gateau, la possiblité d'utiliser Apache Spark sur Redshift.
