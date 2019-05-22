---
layout: post
title: "Core Review Tips"
date: 2019-05-22
description: |
  Few rules to become better code-reviewer and receive
  extra bonuses for good review in Zerocracy.
author:
  name: Kirill
  twitter: kirill_g4s8
---

As an architect of a few projects in [Zerocracy](https://www.zerocracy.com)
I'm merging a couple of [GitHub](https://github.com) pull requests
every day. Each pull request I'm looking at has passed the code-review step. However,
reviewers often miss some important concerns when accepting pull requests.
Here I'll explain what I'm expecting from a good code review.

<!--more-->

## Pull Request Should Fix Reported Issue

Time to time I'm getting pull requests which solve
something different from the reported issue. This may be
a missunderstanding between a bug-reporter and a developer. Or
a developer decided to include some extra features in the pull request. Or
the developer has made some refactoring. In any case, the reviewer
should ask the developer to fix that:

  * If the developer didn't understand the issue but submited some code that didn't
    solve the issue, the reviewer should
    [reject it](https://www.zerocracy.com/policy.html#27)
    and get the payment.

  * If the developer made some unneccessary refactoring, than
    the reviewer should ask to remove it. This point seems to be obvious
    but quite often reviewers forget about that and focus only
    on problems in the code or implementation details. But it should be the
    first step of code review, in my opinion.

## Demand Unit Tests

Each new feature or a bug fix should be started with a unit test. If a unit test
is not present, the reviewer needs to fork the PR branch and ensure that the code
works. But a good reviewer is lazy and doesn't want to fork each PR just to verify it.
Instead of this, the reviewer can ask to include a test to verify that provided
solution works. If the test was included and CI passed, the reviewer can be sure
that a new feature was implemented correctly or a bug was fixed.
The only important code to review is assertions accuracy in the tests
but it can be verified without forking, just by looking at the source code.

## Pay Attention to Documentation

It's a common mistake of a code reviewer: they focus only on code issues
but miss documentation mistakes. It may be vague javadoc or
bad-written README update or something else. In any case, the reviewer
should ask to fix the documentation, because it's an important part of a new code
and it's hard to handle it automatically.

## Puzzle Checks

In Zerocracy we're using [PDD](https://www.yegor256.com/2010/03/04/pdd.html)
(Puzzle Driven Development) to close complex tasks which can't be done in
30 minutes budget. Some developers abuse this methodology and submit
puzzles which are not related to the original issue. The most common scenario is
when a developer was asked to implement a new feature, but submits another feature
task in a pull request, which he/she thinks the product should also
implement. Usually code reviewers ignore these puzzles, the architect also
misses it, and a new feature request is added
to the [WBS](https://en.wikipedia.org/wiki/Work_breakdown_structure) without
PO's or ARC's [approval](https://www.zerocracy.com/policy.html#14).
A good PR reviewer should spot these new puzzles and ask the developer to remove them, if
a puzzle is not a part of the original issue.

## Don't Deal With Huge PRs

New developers are attempting to solve the entire issue in a single pull request,
without using [puzzles](https://www.yegor256.com/2010/03/04/pdd.html).
Instead of explaining the code, reviewers check the entire
pull request with dozen of comments, and then the developer fixes all comments
which involve new issues in the code. It may take many cycles unless the developer
closes the PR and quits the project. The reviewer needs to remember that he/she will
be payed only for [15 minutes](https://www.zerocracy.com/policy.html#27)
for each PR. It should be obvious that it's not possible to review a huge pull
request, even before starting to review. A good reviewer must
ask the developer to reduce the size of the PR
or reject it entirely if it's not possible.

I'm not writing about implementation review or code style review, because it doesn't always
needed---if the project has configured the CI pipeline with unit tests, integration tests,
style checkers or linters, than it will be checked automatically. The only point that
code reviewer may pay attention to is why the developer suppressed some checks, or not implemented
a unit test (or implemented it incorrectly). So, I'd say that the main responsibility of a reviewer
is to verify that the PR complies to the current project workflow and can be verified
automatically, and that all unit tests were written correctly to be handled by the CI tools.
Of course some checks can not be performed automatically but
most of them can, so manual review should not take a lot of time.
