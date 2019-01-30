---
layout: post
title: "FAQ for new projects"
date: 2019-01-30
description: |
  This page will help you to bootstrap new project
  in Zerocracy to start working with 0crat,
  it's configuring Slack chat, Github repos etc.
permalink: /pfaq.html
no_disqus: true
hidden: true
---

To start managing your project with 0crat you need to
login to [0crat.com](https://0crat.com) via Github,
find architect by submitting [RFP](https://www.0crat.com/rfp)
(see [policy#41](https://www.zerocracy.com/policy.html#41),
create a [workplace](https://slack.com/create) in Slack if you
don't have it.

<!--more-->

First of all product owner (PO) have to invite 0crat to slack channel (https://www.zerocracy.com/policy.html#11),
this channel will be used to manage project and to configure 0crat's project settings.

After that PO can invite adviser (a person with high reputation > 1024), this person will bootstrap 0crat, configure
it and assign roles. It can be done by project architect if he/she has enough reputation.

Adviser helps to setup the project, suggests how to configure 0crat and repository,
and with other Zerocracy-related questions. As a reward adviser will receive 4% of project funds from Zerocracy.

Adviser bootstrapps the project using `bootstrap` command, it assigns `PO` and `ARC` roles to adviser, 
so he/she will be able to configure the project (https://www.zerocracy.com/policy.html#12).

Then adviser can:
 * change project title using `title` command
 * [assign](https://www.zerocracy.com/policy.html#13) `PO` role to PO using `assign` command
 * invite architect and assign `ARC` role using `assign` command (in case if adviser and architect are different people)
 * [publish](https://www.zerocracy.com/policy.html#26) project if needed using `publish` project
 * [link](https://www.zerocracy.com/policy.html#17) Github repository using `link` command
 
When adviser done with configuration he/she resigns `PO` and `ARC` role from himself.

Now PO has `PO` role and is able to access project's page at `0crat.com/p/$PID`, where `$PID` is a project id.
PO can fund project at this page using Stripe or Zold.
 
