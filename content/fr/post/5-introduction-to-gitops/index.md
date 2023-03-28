---
title: Découvrez le GitOps !
subtitle: Le GitOps, un enjeu de demain !
# Summary for listings and search engines
summary: Le GitOps est une approche pour la gestion de l'infrastructure et des applications Kubernetes qui utilise Git comme source de vérité pour la configuration. Son principal intérêt est d'automatiser les processus de déploiement, de simplifier la collaboration entre les équipes et de réduire les erreurs humaines grâce à une approche déclarative de la configuration.

# Link this post with a project
projects:
- gitops

# Date published
date: '2023-03-28T22:50:00Z'

# Date updated
lastmod: '2023-03-28T22:50:00Z'

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: Illustration by [Pradeep Loganatha](https://pradeepl.com/)
  focal_point: ''
  placement: 2
  preview_only: false

authors:
  - admin

tags:
  - gitops

categories:
  - gitops
---

Le GitOps est une approche de la gestion opérationnelle qui utilise Git comme source de vérité pour l'infrastructure et les applications qui y sont déployées. Cette méthode repose sur l'idée de versionner des fichiers de configuration et les définitions d'infrastructure dans un référentiel Git, qui sert de source unique de vérité pour tous les composants du système.

Ainsi, avec le GitOps, toutes les modifications apportées à l'infrastructure ou aux applications sont effectuées via des modifications du référentiel Git, que ce soit manuellement ou au travers de processus automatisés. Par exemple, lorsqu'un développeur effectue une modification de code et la pousse sur le référentiel Git, l'outil de déploiement GitOps détecte cette modification, construit l'application et la déploie automatiquement sur l'infrastructure appropriée. L'état de l'infrastructure est mis à jour, tenant en compte ce dernier ajout.

Les avantages de GitOps sont multiples et convergent, dans la mouvances DevOps, à rationnaliser les processus tout en les rendant plus accessible, plus ouverts:
- Source unique de vérité: le GitOps se basant sur le versionnement des ressources, il consistue l'unique référence de l'état de l'infrastructure. Non seulement on réduit le facteur humain dans la connaissance de cette infrastructure, mais en plus on en simplifie la gestion et on en assure la cohérence!
- Intégration continue: le gitops se marrie parfaitement avec l'automatisation. On peut ainsi tirer toute la puissance de l'approche DevOps en prolongeant le déploiement continu applicatif avec le déploiement continu d'infrastructure. On augmente la SLA, on effectue des MEP précises, fiables et répétables!
- Tracabilité: le code étant versionné, on exploite également toute les capacités à tracer les changements, à maitrise qui peut publier; un gros atout pour la sécurité. Enfin, tel d'authentiques dévelopeurs, on mets à disposition la capacité à revert des changements dans le code et donc l'infrastructure !
- Collaboration: un des gros enjeux de l'infrastructure est de sortir de cette fatalité que l'infrastructure est inaccessible au commun des mortels. Désormais, l'infrastructure est décrite sur YAML (ou autre) de manière (presque) lisible pour l'humain et surtout, centralisée. Il faudra peut-être s'équiper d'un dictionnaire infra->français dans un premier temps mais rien que ce changement est un pas de géant!


En termes plus techniques, il existe quelques outils qui permettent d'orchestrer clés-en-main du GitOps dans un contexte applicatif Kubernetes. Les deux outils pertinents selon moi sont:
- FluxCD: un outil open-source qui se déploie en mode serveur sur le cluster cible directement et qui permet de définir des workflows personnalisés. Cet outil est destiné pour être manipulé en CLI mais est très léger.
- ArgoCD: également open-source, l'outil est très complet et un peu plus conséquent à deployer (Helm est votre ami). Il est orienté GUI et permet une gestion fine des utilisateurs permettant à ces derniers d'avoir eux aussi la main sur la gestion d'environnement. J'ai personnellement une préférence pour ce dernier, je vous laisserai chercher pourquoi.

Il existe également d'autres outils, ou d'autre méthodes de gérer du GitOps. Certains impliquent une gestion un peu rock&roll de gitlabCI, GitHub Action et cie . D'autres, comme JenkinsX (Jenkins dans le nom) ne m'attirent pas forcément pour l'instant.

En conclusion, le GitOps est un outil puissant pour la gestion de la configuration et le déploiement continu des applications, qui offre une source unique de vérité, une automatisation continue, une visibilité et une traçabilité complètes, une collaboration efficace et une sécurité renforcée. Le GitOps est une tendance en forte croissance et à raison: simplicité, accélération des déploiements tout en réduisant les erreurs humaines.