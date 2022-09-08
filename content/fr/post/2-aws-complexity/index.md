---
title: A propos de la complexité d'utilisation des ressources AWS
subtitle: Récemment, j'ai effectué un peu d'exploration sur AWS et j'ai pu experimenté l'interaction de certaines resources, notament réseau. La plupart de mon temps a été dédié à comprendre comment ces ressources interagissaient, est-ce toujours raisonnable ?
summary: Récemment, j'ai effectué un peu d'exploration sur AWS et j'ai pu experimenté l'interaction de certaines resources, notament réseau. La plupart de mon temps a été dédié à comprendre comment ces ressources interagissaient, est-ce toujours raisonnable ?

# Link this post with a project
projects:
- full cloud

# Date published
date: '2022-09-08T17:55:00Z'

# Date updated
lastmod: '2022-09-08T17:55:00Z'

# Is this an unpublished draft?
draft: true

# Show this page in the Featured widget?
featured: false

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: Illustration by [Roman Ceresnak](https://medium.com/codex/aws-academy-introduction-aws01-vpc-virtual-private-cloud-ae3665ac8789)
  focal_point: ''
  placement: 2
  preview_only: false

authors:
  - admin

tags:
  - cloud
  - aws
  - wemaintain

categories:
  - Cloud Architecture
---

Le Cloud est un outil merveilleux, la flexibilité qu'il nous donne est d'une plus-value incomparable aux infrastructures d'il n'y a pas si longtemps. Plus besoin d'être dans le prédictif, dans l'anticipation du besoin, plus besoin d'expert CISCO introuvables et hors de prix. Pourquoi s'encombrer d'autant de savoir et de couches de savoir quand d'autres peuvent le faire bien mieux, de manière mutualisée et abordable ?
Récemment, j'ai eu l'occasion de travailler sur les aspects réseaux de notre infrastructure à [WeMaintain](https://wemaintain.com) et de redécouvrir l'énorme palette d'outil proposé par AWS pour résoudre le moindre de nos besoins. Mais l'expérience n'a pas été aussi ergonomique qu'à ce que j'aurai pu m'y attendre. L'aurait-elle due?

La dynamique des acteurs cloud ces dernières années a été de rendre de plus en plus de services accessibles, à moindre coût. Ainsi, beaucoup d'infra y ont vu naissance et beaucoup d'existante y ont migré. Parralèlement, l'accès à ses services s'est simplifié, rendant l'attrait plus fort et l'expérience utilisateur plus engageante, selon moi. Dans cette dynamique, en 2022, 