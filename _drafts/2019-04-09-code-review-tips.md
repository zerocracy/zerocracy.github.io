---
layout: post
title: "Core review tips"
date: 2019-04-09
description: |
  Few rules to become better code-reviewer and receive
  extra bonuses for good review in Zerocracy.
author:
  name: Kirill
  twitter: kirill_g4s8
---

As architect of few project in [Zerocracy](https://www.zerocracy.com)
I'm merging a couple of [Github](https://github.com) pull request
every day. Each pull request I'm looking at has passed code-review step but
reviewers often miss some important concerns when accepting pull requests.
Here I'll explain what I'm expecting from good code review.

<!--more-->

## Pull request should fix reported issue
Time to time I'm getting pull requests which solves
something different from reported issue, it may be
missunderstanding between bug-reporter and developer, or
developer decided to include extra features in pull request,
or made some refactoring, in any case reviewer should ask developer to fix that:
 1. if developer didn't understand the issue but submited some code that didn't
 solve the issue,
 then reviewer should [reject it](https://www.zerocracy.com/policy.html#27)
 and get payment.
 2. if developer made some unneccessary refactoring, then
 reviewer should ask to remove it. This point seems to be obvios
 but quite often reviewers are forgetting about that and focusing only
 on problems in code or implementation details. But it should be the
 first step of code review in my opinion.

## Ask for unit tests
Each new feature or bug fix should be started with a unit test. If unit test
was not present, code reviewer needs to fork PR branch and ensure that the code
works. But good reviewer is lazy and don't want to fork each PR just to verify it.
Instead of this, reviewer can ask to include a test to verify that provided 
solution works, if test was included and CI passed, reviewer can be sure
that new feature was implemented correctly or bug was fixed. 
The only important code to review is assertions accuracy in tests
but it can be verified without forking but just by looking at source code.

## Pay attention to documentation
It's a common mistake of code reviewer to focus only on code issues
but miss documentation mistakes, it may be vague javadoc or
bad-written README update or something else. In any case code-reviewer
should ask to fix documentation, because it's important part of new code
and it's hard to handle it automatically.

## Puzzle checks
In Zerocracy we're using [PDD](https://www.yegor256.com/2010/03/04/pdd.html)
(Puzzle Driven Development) to close complex tasks which can't be done in
30 minutes budget. Some developers abusing this methodology and submitting
puzzles which are not related to origin issue, the most common scenario is
when developer was asked to implement new feature, but submits another feature
task in pull request which he/she thinks product should also
implement. Usually code reviewers ignores these puzzles, architect also
can miss it, and new feature request will be added
to [WBS](https://en.wikipedia.org/wiki/Work_breakdown_structure) without
PO or ARC [approve](https://www.zerocracy.com/policy.html#14).
Good PR reviewer should check new puzzles and ask to remove it, if
puzzle is not a part of solving issue.

## Don't deal with huge PRs
New developers are attempting to solve whole issue in one pull request
without using puzzles. Instead of explaining that code reviewers are reviewing whole
pull request with dozen of comments, after that developer fixing all comments
which involves new issues in code. It may take many cycles unless developer
closes PR and quit the project. Code reviewer need to remember that he/she will
be payed only for [15 minutes](https://www.zerocracy.com/policy.html#27)
for each PR. It should be obvious that it's not possible to review huge pull
request before start to review, so good reviewer can ask developer to reduce PR
size or reject it entirely if it's not possible.


I'm not writing about implementation review or code style review, because it doesn't always
needed - if project has configured CI pipeline with unit tests, integration tests,
style checkers or linters, then it will be checked automatically, the only point that
code reviewer may pay attention, is why developer suppressed some checks, or not implemented
a unit test (implemented unit test not correctly). So I'd say that main code-reviewer work
is to verify that PR complies to current project workflow and can be verified
automatically and that all unit tests were written correctly to be handled by CI tools.
Of course some checks can not be performed automatically but 
most of them can, so manual review should not take a lot of time.
