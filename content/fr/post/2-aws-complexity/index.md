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
lastmod: '2022-09-12T17:12:00Z'

# Is this an unpublished draft?
draft: false

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

La dynamique des acteurs cloud ces dernières années a été de rendre de plus en plus de services accessibles, à moindre coût. Ainsi, beaucoup d'infra y ont vu naissance et beaucoup d'existante y ont migré. Parralèlement, l'accès à ses services s'est simplifié, rendant l'attrait plus fort et l'expérience utilisateur plus engageante, selon moi. Dans cette dynamique, en 2022, je me suis attelé à vouloir créer un [réseau virtuel privé (VPC)](https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc.html) dans AmazonWebService (AWS) afin de tester la possibilité de créer une zone isolée d'internet, dont l'accès n'est possible que depuis un bastion et dont le but est d'opérer uniquement des services internes à notre SI. Dans un monde idéal, ce VPC n'était connecté à internet que pour les besoins de mises à jour de ses composants.

![Initial VPC needs](/fr/post/2-aws-complexity/vpc-commons-needs.png "Initial needs schema")

La réalité de l'exécution a été légèrement différente et c'est la que nous rentrons dans le vif du sujet. Quand bien même l'accès à ces services s'est simplifié, leur usage est resté à peu près le même. CICD, sous-réseau, gateway mais si tout les mots-clés n'y sont pas, l'ensemble des notions restent le même. Il y a même désormais une couche supplémentaire: celle du provider cloud. En ajoutant leur interfacage sur ces concepts réseaux, ils ont développé leurs propres modules qui répondent à leurs propres règles et recommandations. Ainsi, un expert réseau se doit désormais d'être aussi un expert réseau cloud. La complexité monte quand d'Azure à AWS les noms, les règles changent également. Et nous voilà avec une toute nouvelle profession. Non pas que cela soit gênant, car elle couvre bien plus de besoin avec moins de compétente, mais qu'on aurait pu s'attendre à ce qu'elle n'existe pas du tout.

En effet, j'ai été fortement étonné quand j'ai eu, moi-même, à mettre en application des architectures réseaux basées sur des besoins basiques. Créer un VPC isolé d'internet ne me semble pas si spécifique. Créer un VPC dont l'accès depuis l'extérieur est impossible ne me le semble pas non plus. Et pourtant, c'est à moi de faire les recherches, de me documenter pour accomplir cela selon le standard du provider cloud en question.

Ne serait-on donc pas encore à l'apogée du cloud et du no-infrastructure ? Car si une dynamique est claire, c'est bien celle de rendre le cloud si accessible que le seul métier qui y soit associé soit "expert clic-clic AWS/Azure/etc", si cela devait encore être un métier et pas juste une formation.

Toujours est-il que mon métier d'ingénieur m'a permis de m'en tirer en une après-midi. Peut-on aller plus loin?

Le schéma final de l'infrastructure de mon projet ressemble finalement à cela et je l'imagine être le standard, selon mes recherches.

![Final VPC schema](/fr/post/2-aws-complexity/vpc-commons.png "Final VPC schema")

Il aurait même pu être encore plus parfait si je ne m'étais pas rendu compte que des acteurs tels GitHub[^1] ne gérait pas encore l'IPv6 et si je n'avais pas eu à intégrer une couche IPv4 en dépit, j'aurai eu un egress IPv6 only, ce qui est vachement sexy.

Dans un futur proche ?

[^1]: [Shame](https://github.com/community/community/discussions/10539)