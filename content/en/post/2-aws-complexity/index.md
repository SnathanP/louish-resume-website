---
title: About the complexity of working with AWS resources
subtitle: Recently, I have been doing some exploration on AWS and I was able to experience the interaction of certain resources, notably the network. Most of my time was spent understanding how these resources interact, is that reasonable?
summary: Recently, I have been doing some exploration on AWS and I was able to experience the interaction of certain resources, notably the network. Most of my time was spent understanding how these resources interact, is that reasonable?
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

The Cloud is a marvelous tool, the flexibility it gives us is of incomparable added value to the infrastructures of not so long ago. No more need to be predictive, anticipating needs, no more need for unfindable and overpriced CISCO experts. Why bother with so much knowledge and layers of knowledge when others can do it much better, in a shared and affordable way?
Recently, I had the opportunity to work on the network aspects of our infrastructure at [WeMaintain](https://wemaintain.com) and to rediscover the huge range of tools offered by AWS to solve the least of our needs. But the experience was not as ergonomic as I might have expected. Should she have?

The dynamic of cloud players in recent years has been to make more and more services accessible, at a lower cost. Thus, a lot of infrastructure was born there and a lot of existing infrastructure migrated there. At the same time, access to its services has been simplified, making the appeal stronger and the user experience more engaging, in my opinion. In this dynamic, in 2022, I set out to want to create a [virtual private network (VPC)](https://docs.aws.amazon.com/vpc/latest/userguide/what-is-amazon-vpc. html) in AmazonWebService (AWS) in order to test the possibility of creating an isolated zone of the Internet, access to which is only possible from a bastion and the purpose of which is to operate only services internal to our IS. In an ideal world, this VPC was only connected to the internet for the purposes of updating its components.

![Initial VPC needs](/fr/post/2-aws-complexity/vpc-commons-needs.png "Initial needs schema")

The reality of the execution was slightly different and that's where we get to the heart of the matter. Even though access to these services has been simplified, their use has remained more or less the same. CICD, subnet, gateway but if all the keywords are not there, all the concepts remain the same. There is now even an additional layer: that of the cloud provider. By adding their interfacing to these network concepts, they have developed their own modules that meet their own rules and recommendations. Thus, a network expert must now also be a cloud network expert. The complexity rises when from Azure to AWS the names, the rules also change. And here we are with a whole new profession. Not that it's embarrassing, because it covers much more needs with less competence, but that one would have expected that it does not exist at all.

Indeed, I was greatly surprised when I myself had to implement network architectures based on basic needs. Creating a VPC isolated from the internet doesn't seem so specific to me. Creating a VPC that cannot be accessed from the outside doesn't seem like it to me either. And yet, it's up to me to do the research, to document myself to accomplish this according to the standard of the cloud provider in question.

Wouldn't we be at the peak of cloud and no-infrastructure? Because if a dynamic is clear, it is that of making the cloud so accessible that the only profession associated with it is "expert click-click AWS/Azure/etc", if this were still to be a profession and not just a training.

Still, my job as an engineer allowed me to get out of it in an afternoon. Can we go further?

The final form of my project's infrastructure ultimately looks like this and I imagine it to be the standard, according to my research.

![Final VPC schema](/fr/post/2-aws-complexity/vpc-commons.png "Final VPC schema")

It could even have been even more perfect if I hadn't realized that players like GitHub[^1] didn't yet manage IPv6 and if I hadn't had to integrate an IPv4 layer despite it, I would have had a egress IPv6 only, which is damn sexy.

In the near future ?

[^1]: [Shame](https://github.com/community/community/discussions/10539)