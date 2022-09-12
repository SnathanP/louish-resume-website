---
title: ArgoCD in production at WeMaintain !
subtitle: For some time now at WeMaintain, ArgoCD has been around, spreading projects through projects. Since this Monday, it is now used for production apps! But to what extent?

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

Why not manage your IS like a business product?
Consumers, customers, suppliers, MVPs, stakeholders, planning; the more I think about it, the more common notions I see.

So all we were missing would be the link between theory and practice?

Not so much now: Infrastructure as Code, Network as Code, DevOps and now #gitops, all these concepts take shape through solutions such as Terraform, Istio, Ansible, Argo and many others.
Put end to end, the evolution of an IS is now completely possible through the code, like a project as a whole, and can itself be subject to the automation of its deployment (So InfraOps?: p). The infrastructure becomes reactive. Cloud technologies now allow us great flexibility, we are no longer anticipating a few years but reacting to a few minutes. The infrastructure becomes apparent, malleable and can now closely follow business needs.
Its operating processes are automatable and rationalizable, maximizing repeatability and reducing the human factor, the dream. CI over GitOps, canary and blue-green now even allow an automated delivery workflow, from the smallest integration to production.
And most importantly, other people now have the opportunity to consult this “new” code, to contribute to it, to question it and to bring a fresh, naive, vital vision to it.

Having laid the first GitOps brick at WeMaintain last week, I am already delighted to see the growing confidence in our processes and I am impatient to be able to go even further. And, I must say, it's a real pleasure to work in an environment that aims so far and gives itself the means to do so.