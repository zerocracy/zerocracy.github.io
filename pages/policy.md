---
layout: page
title: "Policy"
date: 2018-02-22
description: |
  Policy of Zerocrat, a project manager
  that never sleeps, owned and maintained by Zerocracy.
permalink: policy.html
---

The Policy explains basic work principles of
[0crat](https://www.0crat.com) ("Zerocrat"):
a project management AI bot developed
and hosted by [Zerocracy](http://www.zerocracy.com).

If you want to change something in the Policy or simply
suggest an improvement, please submit a ticket
[here](https://github.com/zerocracy/zerocracy.github.io/issues).
If you want to discuss the Policy or your troubles with the bot,
please join this [Telegram chat](https://t.me/joinchat/CLxAaQ0xp-g_3WWI3MBr2g).

Read this first: [What Is Zerocracy?](/toc.html)

## Developer (<a id="DEV">DEV</a>)

You can talk to Zerocrat in:

  * Slack: [start](https://www.0crat.com/add_to_slack) a private conversation with `@0crat`
  * Telegram: [start](https://telegram.me/zerocrat_bot) a chat with [`@zerocrat_bot`](https://telegram.me/zerocrat_bot)
  * GitHub: prepend your message in any ticket with [`@0crat`](https://github.com/0crat)

<a id="1" href="#1">§1</a>
"Invite."
To start working with us you have to be invited by someone we already know,
whose [reputation](#18) is over <del>+1024</del> <span id="1.min-rep" style="color:red">+256</span>.
Ask that person to say `invite` with your GitHub login to Zerocrat.
The person will be your "mentor" and will be responsible for helping you
out in the system. A mentor may have up to <del>16</del> <span id="1.max-students" style="color:red">24</span> students
and pays <span id="1.price">128</span> [points](#18) for each new invitation.
Fill out [this form](https://www.0crat.com/join) (you can do it every <span id="1.lag">16</span> days)
if you don't know anyone yet
or seek help in [our Telegram group](https://t.me/joinchat/CLxAaQ0xp-g_3WWI3MBr2g).
Once you are invited, your name and your performance metrics will be visible
in the [Team page](https://www.0crat.com/team).

<a id="2" href="#2">§2</a>
"Apply."
To join a project you have to find it on the [Board](https://www.0crat.com/board)
and send `apply` request to Zerocrat. The architect of the project will
either invite you or ignore your request. You can apply multiple times,
even to the project you already are a member of, for example, to request
a raise of your [project rate](#13).

<a id="33" href="#33">§33</a>
"Sandbox."
You can [apply](#2) to a project only if your [reputation](#18) is over
<del>+256</del> <span id="33.min-live" style="color:red">+128</span>.
If it is lower, you can only apply to [sandbox](https://www.0crat.com/board) projects
and your highest allowed rate is <span id="33.max-sandbox-rate">$16</span>.
You can't apply to a sandbox project if your reputation is over <span id="33.max-sandbox-rep">+1024</span>.
You will be automatically removed from a sandbox project once your reputation is over <span id="33.sandbox-rep-threshold">+1024</span>.
You will automatically get `REV` role in a sandbox project when your reputation is over <span id="33.rev-rep">+256</span>
and you will lose it if the reputation drops below <span id="33.rev-min-rep">+128</span>.

<a id="3" href="#3">§3</a>
"Election."
Zerocrat may assign a job to you according to its own election rules, if you have `DEV` role
and are not on [vacation](#38).
You will be notified in job's ticket. The rules include, in order of importance:

  * The highest [reputation](#18) wins;
  * No jobs will be assigned if [reputation](#18) is below <span id="3.low-threshold">-128</span>;
  * Lowest [project rate](#16) wins;
  * Shortest average [job completion time](#26) wins;
  * The emptiest agenda wins;
  * The maximum allowed size of agenda depends on your [reputation](#18):
    * <span id="3.jobs-1">3</span> jobs if less than <span id="3.rep-1">+512</span> points,
    * <span id="3.jobs-2">8</span> if less than <span id="3.rep-2">+2048</span>,
    * <span id="3.jobs-3">16</span> if less than <span id="3.rep-3">+4096</span>,
    * <span id="3.jobs-4">24</span> otherwise;
  * The size of agenda doesn't matter if the job is a code review;
  * The absolute maximum of jobs you may have in your agenda is <span id="3.absolute-max">32</span>;
  * If your [debt](#46) is over <span id="3.max-debt">$128</span> you won't get any new jobs.

<a id="4" href="#4">§4</a>
"Fixed Budget."
Each job has a fixed budget in minutes,
which will be multiplied by your hourly rate and paid to you when the job is completed.
The actual amount of time you spend on the job doesn't affect the amount of money you receive.
You will also get as many positive [points](#18) as many minutes you are paid for.

<a id="18" href="#18">§18</a>
"Points of Reputation."
You may earn positive and negative points for doing good and bad things in
the projects. They do not affect your cash income, but do affect the impression Zerocrat
has about you&mdash;the more points you have the more disciplined developer you are.
Zerocrat takes into account only the points you earned over the last <span id="18.days">90</span> days.

<a id="5" href="#5">§5</a>
"Boost Factor."
A job may receive a boost factor, which will increase or decrease its budget.
Default boost factor is `2x`, which means 30 minutes.
Default boost factor for a code review is `1x`.
In exceptional situations, you should ask project architect to boost your job.

<a id="6" href="#6">§6</a>
"Refusal."
You may refuse to complete any job by saying `refuse` or `resign`.
You will get a penalty of <span id="6.penalty">15</span> [points](#18) for that.

<a id="7" href="#7">§7</a>
"Definition of Done."
A job is completed when its ticket is [closed](http://www.yegor256.com/2014/04/15/definition-of-done.html).
Until then only one person is responsible for it: the performer.
It doesn't matter why the job is not finished, who its success depends on, where is the problem.
The 0/100 rule is simple: it's either done or not.

<a id="8" href="#8">§8</a>
"Ten Days."
If you don't complete a job in <span id="8.days">10</span> days Zerocrat _may_ take it away from you.
You will get no money and a penalty as big as the the [budget](#4) of the job, if this happens.

<a id="29" href="#29">§29</a>
"Pay per Bug."
Each time you report a new [bug](http://www.yegor256.com/2018/02/06/where-to-find-more-bugs.html)
that becomes a job, you earn <span id="29.price">+15</span> minutes.
The ARC makes a subjective non-disputable decision whether a reported bug deserves to be a job or not.

<a id="9" href="#9">§9</a>
"Impediments."
You may declare impediments for a job by saying `wait` to Zerocrat.
Until the job has impediments [Ten Days rule](#8)
is not applicable to it.

<a id="36" href="#36">§36</a>
"Speed Bonus."
Zerocracy measures the time interval between the moment
a job is assigned to you and the moment it goes out of scope.
If this interval is shorter than <span id="36.hours">48</span> hours,
you get extra <span id="36.bonus">+5</span> minutes.

<a id="16" href="#16">§16</a>
"Rate."
To make money in any project you must define your hourly rate.
To do that just say `rate` to Zerocrat. This rate is for marketing purpose
only, since each project will [set](#13) their own rates for you.
Your rate can only be between <span id="16.min">$16</span> and <span id="16.max">$256</span>.
You can use USD, EUR, GBP, or JPY (format like `17EUR` or `25.50GBP`), but all payments will be made in USD
(converted by [apilayer](https://apilayer.net)).

<a id="20" href="#20">§20</a>
"Wallet."
We can send you money either via
[PayPal](https://www.paypal.com),
[Bitcoin](https://bitcoin.org/en/),
[Bitcoin Cash](https://www.bitcoincash.org/),
[Ethereum](https://www.ethereum.org/),
or
[Litecoin](https://litecoin.org/).
To tell us how exactly you want to receive them just say `wallet` to Zerocrat.

<a id="46" href="#46">§46</a>
"Debt."
When Zerocrat fails to pay, for any reason, the payment amount will be added to our "debt" to you.
We attempt to pay the debt once a day, if it's larger than <span id="46.threshold">$64</span>
or older than <span id="46.days">32</span> days.
Possible reasons of not paying immedidately include, but not limited to:

  * Network connection with the payment gateway is broken;
  * Temprorary issues with our accounts in PayPal, Coinbase, etc.;
  * The amount is smaller than <span id="46.min">$24</span> (to avoid big commissions);
  * We are broke (just kidding).

<a id="32" href="#32">§32</a>
"Job Status."
You can always check the status of any job, just say `status` to Zerocrat in the job ticket.

<a id="48" href="#48">§48</a>
"Only points."
If you are not a member of a project, you can only earn [points](#18) there, not cash.

<a id="43" href="#43">§43</a>
"Graduation."
When your [reputation](#8) reaches <span id="43.threshold">+1024</span>,
Zerocrat will automaticatly set himself as your mentor.

<a id="44" href="#44">§44</a>
"Expel."
When your [reputation](#8) drops lower than <span id="44.threshold">-256</span>,
Zerocrat will automaticatly disconnect you from your mentor,
clean out your reputation and you will have to [start over](#1).

<a id="45" href="#45">§45</a>
"Tuition fee."
While you have a [mentor](#1) (and it's [not Zerocrat](#43)),
he/she gets <span id="45.share">8</span> cents of every dollar you make.

<a id="47" href="#47">§47</a>
"Breakup."
You can always terminate your relationship with a student, just say `breakup` to Zerocrat.
You will get a penalty of <span id="47.penalty">256</span> for this.

<a id="40" href="#40">§40</a>
"Reply to RFP."
If your [reputation](#18) is over <del>+512</del> <span id="40.min" style="color:red">+128</span>,
you will see new [requests for proposal](https://www.0crat.com/rfps).
You can "pay" <del>256</del> <span id="40.price" style="color:red">64</span>
points for an email address of any RFP, contact them directly,
and bring them to Zerocrat; to do that just say `rfp` to Zerocrat.
Remember, you are [not allowed](http://datum.zerocracy.com/pages/terms.html#non-solicitation)
to work with them without Zerocrat.

<a id="38" href="#38">§38</a>
"Vacation."
You can always "go on vacation" if you want Zerocrat to temporarily stop
assigning you new jobs; just say `vacation`.

<a id="52" href="#52">§52</a>
"Auto-Vacation."
If you receive <span id="52.awards">8</span> or more negative awards in the past <span id="52.days">16</span> days and
no positive ones, your vacation status will automatically be set to `on`, which means you will not receive new tasks.
You have to manually turn off vacation status to receive new tasks. Note that you can turn vacation off any time, but
the auto-vacation mechanism will be re-evaluated if you receive another negative award.

<a id="35" href="#35">§35</a>
"Quit."
You can always quit a project, just say `quit` to Zerocrat.
You will still have to finish the jobs assigned to you in the project.

<a id="39" href="#39">§39</a>
"GitHub name change."
If you [change](https://help.github.com/articles/changing-your-github-username/)
your GitHub name, your Zerocrat account will be lost.
You will have to create a new one from scratch.
[Why?](https://github.com/zerocracy/datum/issues/274)

## Code Reviewer (<a id="REV">REV</a>)

<a id="27" href="#27">§27</a>
"Code Reviews."
You will be asked to review pull requests if you have `REV` role assigned.
Be as critical as you can, as [this article](http://www.yegor256.com/2015/02/09/serious-code-reviewer.html) explains.
Either you accept or reject the changes, inform the architect, right in the ticket&mdash;the
architect will either merge the pull request or close it.
In either case, you will be paid <span id="27.price">+15</span> minutes.

## Product Owner (<a id="PO">PO</a>)

<a id="41" href="#41">§41</a>
"Submit RFP."
The best way to recruit Zerocrat and develop your project with us is to
find and hire an architect&mdash;one of our [best developers](https://www.0crat.com/team).
You have to fill out [the form](https://www.0crat.com/rfp),
pay non-refundable <del>$64</del> <span id="41.price" style="color:red">$16</span>,
and wait until one of them [replies](#40).
The RFP will expire and automatically disappear in <span id="41.days">32</span> days.
You can submit a new RFP only when the first one expires or is purchased.

<a id="11" href="#11">§11</a>
"Add to Slack."
To start working with us, you have to [invite](https://www.0crat.com/add_to_slack)
Zerocrat to your Slack.

<a id="17" href="#17">§17</a>
"Connect GitHub."
To connect your GitHub repository to the project you should
1) add a new Webhook: `http://www.rehttp.net/p/https://www.0crat.com/ghook`
(with "send me everything" option),
and
2) link the project in Slack: `links add github yegor256/cactoos`, where
instead of `yegor256/cactoos` you should put the coordinates of your GitHub repository.

<a id="21" href="#21">§21</a>
"Project funds."
You can add funds to the project by VISA or MasterCard via [Stripe](https://www.stripe.com)
at the project web page. Fund will be used to pay programmers for job
completion and to pay Zerocracy management [fee](#23).
We will automatically recharge your card when the project runs out of funds.
To disable recharing use [pause/activate](#24) option.

<a id="22" href="#22">§22</a>
"Refunds."
All unused funds will be returned to you immediately per your request by
[email](mailto:refund@zerocracy.com).
Refunds will be mailed back to you as a cheque of a US bank.

<a id="23" href="#23">§23</a>
"Management fee."
Zerocracy charges a fixed management fee of <span id="23.fee">$4</span> per each successfully
completed job. If your project is not [linked](#17) to any private GitHub repositories
this fee is waived. If the fee is waived the ledger of the project will
be publicly visible online.

<a id="24" href="#24">§24</a>
"Pause/Activate."
To put Zerocrat on hold and make a project completely inactive, say `pause`.
To return the project back to life say `pause off`.
This will disable [recharging](#22).

<a id="25" href="#25">§25</a>
"Destroy."
To completely delete all project files from our servers and terminate the
project say `destroy` and then [kick off](https://get.slack.help/hc/en-us/articles/201898668-Remove-someone-from-a-channel)
`@0crat` from Slack channel. There is no way back. We highly recommend to use
[pause/activate option](#24).

<a id="26" href="#26">§26</a>
"Publish."
To attract programmers to your project, you can publish it on the
[Board](https://www.0crat.com/board); just say `publish on` to Zerocrat in order to do it.
Your [reputation](#18) has to be over <span id="26.min-rep">+1024</span> and
you will be charged <span id="26.price">32</span> [points](#17) for this.
When your project is published, its statistical information will be visible in the Web.
You can unpublish it anytime, just say `publish off`.

<a id="37" href="#37">§37</a>
"Micro-Vesting."
On top of [cash](#13) you can give [equity](http://www.yegor256.com/2018/02/13/micro-vesting.html) to project contributors.
Just add the vesting rate to the `assign` [command](#13), for example:
`assign DEV yegor256 $16 $40`, where `$16` is the rate paid in cash and
`$24` to be paid in equity after each job [completion](#7).

<a id="50" href="#50">§50</a>
"Contribution."
Anyone can make a non-refundable one-time
[contribution](http://www.yegor256.com/2018/04/03/donations-via-zerocracy.html)
to your project, if you give them
the URL `https://www.0crat.com/contrib/PID` where `PID` is your project ID.
Your project has to be [published](#26) and [fee-free](#23).

## Architect (<a id="ARC">ARC</a>)

<a id="12" href="#12">§12</a>
"Bootstrap."
To let Zerocrat manage your project you have to create a new Slack
channel and add `@0crat` to it.
Then, you should say `bootstrap` to Zerocrat.
You need to have at least <span id="12.min">+1024</span> reputation points to be able to do that.
You will be charged <span id="12.price">256</span>
[points](#18) for each project you bootstrap.

<a id="13" href="#13">§13</a>
"Assign/Resign Role."
Everybody who will be managed by Zerocrat must have roles in the project.
To assign a role you say `assign`. To remove a role you say `resign`.
By default, all new people you assign are supposed to work for free. If you
want to pay them for the jobs they complete, add hourly rate to the `assign`
command, for example: `assign DEV yegor256 $50`. To change the hourly
rate of a person just assign the same role with a different rate, or `0`
in order to make them work for free;
this will not affect the [budgets](#4) of already assigned tasks.

<a id="34" href="#34">§34</a>
"Mandatory Roles."
A project must always have one PO and one ARC.
A project may not have more than two ARCs or more than two POs.
ARC and REV roles can't be assigned to the same person.
QA role can't overlap with REV, DEV or ARC.

<a id="14" href="#14">§14</a>
"Scope In/Out."
You should add jobs to the scope, by saying `in` to Zerocrat (or assigning the ticket to him).
You can remove a job from the scope by saying `out`.

<a id="53" href="#53">§53</a>
"Auto-In."
Zerocrat automatically adds pull requests to scope, unless
they are too small and don't deserve it. The decision is made by Zerocrat automatically.

<a id="15" href="#15">§15</a>
"Boosting."
You can increase a budget of the job by setting its boost factor.
Just say `boost 2x` (or `3x`, `5x`, etc.) to Zerocrat.
This operation is against our principles of [micro-budgeting](http://www.yegor256.com/2018/01/09/micro-budgeting.html),
that's why you get a penalty of <span id="15.penalty">10</span> [points](#18)
every time you do this.

<a id="19" href="#19">§19</a>
"Assign Job."
You can manually assign any job to a user, just say `assign @yegor256`
(where instead of `@yegor256` you put the GitHub login of the user) or
assign the ticket to that user in your ticket tracking system.
This operation is against our principles of automated task management,
that's why you will get <span id="19.penalty">5</span> [points](#18) every time you do this.
If you assign a job to its reporter/creator, you will get an additional penalty of
<span id="19.self-penalty">15</span> [points](#18).

<a id="28" href="#28">§28</a>
"Architect Review Bonus."
You will earn <span id="28.price">+10</span> minutes for each pull request successfully merged.
Only [in-scope](#53) pull requests will be paid.
It is recommended to use [Rultor](http://www.rultor.com) or a similar
solution, which will allow only the architect to merge.

<a id="49" href="#49">§49</a>
"Extra."
You can pay extra cash to any user by saying `pay` to Zerocrat.
You will get a penalty of <del>60</del> <span id="49.penalty" style="color:red">20</span> points for this.
The maximum you can pay in one go is <span id="49.max">120</span> minutes.

<a id="51" href="#51">§51</a>
"Hiring."
If your [reputation](#18) is over <span id="51.min">+1024</span>
you can invite programmers to your project by announcing a job
(you can find a link at your project dashboard).
Each announcement will cost you
<span id="51.price">128</span> reputation [points](#18).

## Quality Assurance (<a id="QA">QA</a>)

<a id="30" href="#30">§30</a>
"Quality Review."
If you have `QA` role in the project, you will be asked to review jobs after their completion.
You have to review the job for its quality and report to Zerocrat: `quality good`
(or `bad`, or `acceptable`).
You will be paid <span id="30.price">+8</span> minutes for the review, no matter what is your verdict.

<a id="42" href="#42">§42</a>
"QA Rules."
The quality of a job is "good" if all of the following requirements are met:

  * The formatting of a job description, as well as all messages inside it,
    follows [Github Markdown](https://help.github.com/articles/github-flavored-markdown/) style;
  * Messages in a job
    [always](http://www.yegor256.com/2014/11/24/principles-of-bug-tracking.html#4-avoid-noiseaddress-your-comments)
    start with a name of a user they are addressed to;
  * The job is closed only when the reported problem is solved,
    [see](http://www.yegor256.com/2015/02/12/top-down-design.html);
  * Ticket must have references to all pull requests where the problem was actually fixed;
  * Problem reporter and problem solver are two different persons;
    [see](http://www.yegor256.com/2014/11/24/principles-of-bug-tracking.html#1.-keep-it-one-on-one);
  * Ticket title and description clearly state what is broken and what kind of fix is expected,
    [see](http://www.yegor256.com/2014/11/24/principles-of-bug-tracking.html#5.-report-when-it-is-broken);
  * The ticket describes one specific problem and provides a single solution;
  * Pull request title explains the problem it is fixing;
  * Pull request description explains the solution proposed and
    contains a link to the original ticket it is related to ([discuss](https://github.com/zerocracy/datum/issues/296));
  * The code reviewer found at least three problems in the code ([discuss](https://github.com/zerocracy/datum/issues/294));
  * Comments were mostly about design problems, not cosmetic issues;
  * All problems found by the code reviewer were _addressed_ by the pull request author, which
    means that they were either fixed as the reviewer wanted or the reviewer was
    convinced that they should not be fixed;
  * All impediments registered in the ticket have explanations of the
    reasons and links to related tickets, if necessary ([discuss](https://github.com/zerocracy/datum/issues/300));
  * All commit messages have links to issues ([discuss](https://github.com/zerocracy/datum/issues/295)).

When you find any rules violation, ask job performer to confirm that
your complains are understood and he/she will try to avoid those mistakes
in the future. Until you get a confirmation,
[don't give](https://github.com/zerocracy/datum/issues/301) any quality mark;
don't wait for more than five days though.

The quality of a job is "bad" if any of the following happens
(these violations we can't forgive):

  * The code reviewer didn't find any issues in the source code
    changes of a pull request and just accepted it;
  * The job is closed without a solution provided.

<a id="31" href="#31">§31</a>
"QA Bonus."
Job performer will get an extra <span id="31.bonus">+5</span> minutes if QA reports `good` quality.
If the quality is `bad`, there will be no payment to the job performer at all.

