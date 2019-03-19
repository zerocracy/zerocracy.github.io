---
layout: post
title: "How to become a QA in Zerocracy?"
date: 2019-03-18
description: |
  If you want to work as QA in projects under Zerocracy,
  you need to know some basics about this role and learn
  Zerocracy rules to be able to review jobs.
author:
  name: Kirill
  twitter: kirill_g4s8
---

We're receiving too many requests for joining as a QA,
so to avoid explaining same things in chat, I'll write it in this post.
The most common misconception about QA role is that the person (who is applying
for that role) is thinking that he/she will be asked to test software or verify
that bugs were fixed. It's wrong, we have another role for that:
`TST` ([tester](https://www.zerocracy.com/policy.html#56) role).
`QA` role responsibilities include different things: verifying that completed jobs
are up to quality, checking that Zerocracy rules were respected. Here I describe
the list of steps to get the `QA` role in Zerocracy projects and what to do next.

<!--more-->

Before you start, please read [our policy](https://www.zerocracy.com/policy.html), pay attention
to the [§30 “Quality Review”](https://www.zerocracy.com/policy.html#30) section. You should have a good
knowledge of the Policy if you want to be a QA, because the primary job of quality assurance in Zerocracy is to
review completed tickets and check against these rules.

When you're ready, go to [GitHub](https://github.com) and create an account if you don't have one.
Then submit a [join form](https://www.0crat.com/join), say that you are "joining as a QA" in the description,
your resume will be reviewed and accepted by one of the members with high reputation. The person who will
[invite](https://www.zerocracy.com/policy.html#1) you becomes your mentor, don't hesitate to ask him any questions
about Zerocracy, he/she will receive a part of your payments [for that](https://www.zerocracy.com/policy.html#45),
until you earn some good reputation. Then you'll need to configure the profile: hourly rate (Zerocracy QA has fixed
hourly price at the moment: $16), wallet, and pass identification (see Policy for more details).

After that you can join [sandbox](https://www.zerocracy.com/policy.html#33) projects to understand how
things are going. If sandbox projects don't have enough funds or tasks,
ask someone in [our Telegram chat](https://t.me/zerocracy) to invite you to a real project.
Also, I would recommend to see how QA work was done before you in some public projects, e.g. in
[yegor256/takes](https://github.com/yegor256/takes/).

When you're done, you can try to join any project, which you find on the [board page](https://www.0crat.com/board).
To join a project use [apply](https://www.zerocracy.com/policy.html#2) command in
[@zerocrat_bot](https://t.me/zerocrat_bot) Telegram bot: `apply <project> QA $16`,
project's `PO` and `ARC` will receive your application and may assign you the `QA` role.
Keep in mind, that if you have any of `DEV`, `REV`, `ARC` roles in the project, you can't
join as a `QA`.

If you have the `QA` role in project, `@0crat` bot will assign you completed jobs for review.
It can be issues, completed by `DEV`, or pull requests, completed by `REV`.
Depending on the job type try to find any [rule violation](https://www.zerocracy.com/policy.html#42),
ask the performer to fix it if possible, and then report the quality, right there in the ticket.
Don't forget to confirm that the performer agrees with your quality verdict (because you may miss something).
After each verdict you will receive [payment and reputation points](https://www.zerocracy.com/policy.html#30).
If you report a `good` quality, the performer will receive [QA-bonus](https://www.zerocracy.com/policy.html#31).
To see all pending tickets waiting for review, in "agenda" page, to see it,
click the link on your profile.
