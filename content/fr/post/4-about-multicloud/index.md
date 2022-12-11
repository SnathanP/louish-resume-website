---
title: Une note sur le multicloud
subtitle: Retour sur une conférence à propos du multicloud
summary: Il y a quelques jours, j'ai pu assister à une conférence dont le sujet traitait du multi-cloud, retour sur son contenu et positionnement.

# Link this post with a project
projects:
- full cloud

# Date published
date: '2022-12-10T14:55:00Z'

# Is this an unpublished draft?
draft: false

# Show this page in the Featured widget?
featured: false

# Featured image
# Place an image named `featured.jpg/png` in this page's folder and customize its options here.
image:
  caption: Illustration by [Sreejata Basu](https://www.muvi.com/author-blog.html?u=sreejatamuvi-com)
  focal_point: ''
  placement: 2
  preview_only: false

authors:
  - admin

tags:
  - cloud

categories:
  - Cloud Architecture
---


Il y a quelques jours, j'ai pu assister à une conférence dont le sujet traitait du multi-cloud[^1]. Le contenu même de la présentation ne s'est finalement révélé n'être qu'un tableau pros/cons bancal sur le multi-cloud. Finalement, la partie la plus intéressante aura été la séance de question-réponse. Comme j'ai été très sceptique sur les réponses de l'intervenant ou même sur sa posture un peu trop enthousiaste pour le multi-cloud, je souhaitais faire quelques retours sur cette thématique et donner ma position.

Le multi-cloud n'est pas aujourd'hui quelque chose de souhaitable.

Et je vais commencer par rappeler, tels mentionnés par l'intervenant, les bénéfices du multi-cloud :
- la capacité à faire jouer la concurrence sur les services négociés.
Et c'est tout.
Et même sur cet unique avantage, nous pouvons en rediscuter, car dans un contexte où juste trouver un ingénieur infrastructure est un parcours du combattant, souhaitons nous vraiment dilapider cette précieuse bande passante sur un multi-cloud ?

La seule raison qui peut mener à une situation de multi-cloud acceptable serait le legacy, comme par exemple l'acquisition et fusion. Autrement, n'y allez pas volontairement, car devoir travailler sur le plus petit dénominateur en commun de différents clouds nous ferait faire un retour en arrière de 10 ans.
L'avenir du cloud est dans le managé, est dans le vendor-locking.
C'est assez choquant à dire, mais comprenons que les ressources des DSI sont limitées. A tel point qu'investir l'équivalent d'un salaire dans un outil qui économiserait des mois-hommes est le genre de levier qui permet, en définitive, de gérer efficacement son budget. Ne soyons pas frileux de nous engager profondément avec un fournisseur, quels qu'il soit, car toute la puissance de leur solution prend vraiment sens quand on se donne la peine de les utiliser pleinement. Et ce n'est pas achevable ici pour le multi-cloud. Très peu d'entreprises sont capable de revendiquer un lift&shift indolore, bien au contraire.
Cela me désole d'autant plus que des cabinets tels que celui du présentateur font conseil sur ce type d'infrastructure chronophage, et c'est bien dans leur intérêt.

La seule chose achevable par le multi-cloud est de réinventer la roue à vos frais.

[^1]: On parle ici de l'utilisation de 2 fournisseurs cloud ou plus pour la gestion d'infrastruction, d'opérationel. Il n'est pas question de parc hybride ici.