---
title: Discover GitOps!
subtitle: GitOps, a challenge of tomorrow!
# Summary for listings and search engines
summary: GitOps is an approach for managing Kubernetes infrastructure and applications that uses Git as the source of truth for configuration. Its main interest is to automate deployment processes, simplify collaboration between teams and reduce human errors thanks to a declarative approach to configuration.

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

GitOps is an approach to operational management that uses Git as the source of truth for infrastructure and the applications deployed on it. This method is based on the idea of versioning configuration files and infrastructure definitions in a Git repository, which serves as the single source of truth for all system components.

Thus, with GitOps, all changes to infrastructure or applications are made through changes to the Git repository, either manually or through automated processes. For example, when a developer makes a code change and pushes it to the Git repository, the GitOps deployment tool detects that change, builds the application, and automatically deploys it to the appropriate infrastructure. The state of the infrastructure is updated, taking this latest addition into account.

The advantages of GitOps are multiple and converge, in the DevOps movement, to rationalize processes while making them more accessible, more open:
- Single source of truth: the GitOps being based on the versioning of the resources, it consists of the only reference of the state of the infrastructure. Not only are we reducing the human factor in knowing this infrastructure, but we are also simplifying its management and ensuring its consistency!
- Continuous integration: gitops goes perfectly with automation. We can thus draw the full power of the DevOps approach by extending the continuous deployment of applications with the continuous deployment of infrastructure. We increase the SLA, we perform precise, reliable and repeatable MEPs!
- Traceability: the code being versioned, we also exploit all the capacities to trace the changes, to control who can publish; a big plus for safety. Finally, like authentic developers, we provide the ability to revert changes in the code and therefore the infrastructure!
- Collaboration: one of the big challenges of the infrastructure is to get out of this fatality that the infrastructure is inaccessible to ordinary mortals. Now, the infrastructure is described on YAML (or other) in an (almost) readable way for humans and above all, centralized. It may be necessary to equip yourself with an infra->English dictionary at first, but this change alone is a giant step!

In more technical terms, there are a few tools that allow you to orchestrate turnkey GitOps in a Kubernetes application context. The two relevant tools in my opinion are:
- FluxCD: an open-source tool that deploys in server mode directly on the target cluster and allows you to define custom workflows. This tool is intended to be handled in CLI but is very light.
- ArgoCD: also open-source, the tool is very complete and a little more substantial to deploy (Helm is your friend). It is GUI oriented and allows a fine management of users allowing them to also have their hands on the management of the environment. I personally have a preference for the latter, I'll let you figure out why.

There are also other tools, or other methods of managing GitOps. Some involve a little rock&roll management of gitlabCI, GitHub Action and co. Others, like JenkinsX (Jenkins in the name) don't necessarily appeal to me right now.

In conclusion, GitOps is a powerful tool for configuration management and continuous application deployment that offers a single source of truth, continuous automation, full visibility and traceability, efficient collaboration, and enhanced security. GitOps is a growing trend and for good reason: simplicity, speeding up deployments while reducing human error.