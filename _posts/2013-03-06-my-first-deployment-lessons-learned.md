---
layout: post
title: "My first deployment: lessons learned"
description: "Things I learned from my first deployment"
category: Development
tags: [continuous integration, automation, testing]
---
{% include JB/setup %}

Two weekends ago I experienced my first code deployment at my client (and ever). I really don't know what I expected. I suppose I never really thought about the deployment much, assuming code just magically went to production at some point.

Turns out, it took some work to get our code to production.

Turns out, deployments should probably be more like my original description.

#### Automate your deployments

The thing that probably stands out to me the most was how much human interaction was required. One of our applications was deployed manually, meaning resources were manually copied/replaced and configuration files were being changed at the time of deployment. Not only did this introduce the potential of a lot of human error, but it was also a lot of work.

Conversly, another app we deployed *was* automated. There was significantly less human effort involved, and everything went pretty much as expected.

#### Seriously, automate your deployments

Not having automation also makes managing test environments difficult. Basically all my previously mentioned points come into play here as well. 

I now have the mindset that every test deployment I do is exactly that, a trial run of a production deployment. If you run into problems deploying to test machine, chances are you need to refine your process a little.

#### Your application and environments should mirror production behavior

If you ever change code or configuration to make testing easier in any way, I'll be the first to tell you **NO NO NO NO NO NO NO NO**.

If your application's behavior or the environment its running in doesn't match production, then there's almost no point in having the whole setup in the first place. Sure, your app is working. Great! But your still not preparing yourself for the real deal.

#### Document everything

Whats worse than having an app you have to deploy manually? Only having a handful of people who know how to do it. And if something breaks? Not having all the moving pieces of an application well documented will greatly increase your time spent debugging. It also limits how much your team can help everyone isn't in sync.

#### TL;DR - It's all about managing the number of unknowns

The fewer unknowns present in any scenario greatly reduce the probability that things will go wrong.

#### Finally, don't forget to check in your project files :)

They're important!
