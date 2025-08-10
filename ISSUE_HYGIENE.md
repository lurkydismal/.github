## tl;dr

- **P4** means "important bug", and each level above **P4** (from **P3** to **P0**) is an order of magnitude higher importance.
- If you have permission, assign bugs to yourself if you are working on them.
- Detach bugs that you are not working on soon.
- If an issue is not assigned, assume it is available to be worked on.

## Overview

I use GitHub issue tracker.

This page mostly talks about how I handle things for the issue tracker.

### Issue philosophy

I assume that this repository, like all non-trivial software, has an infinite number of bugs.
Bugs includes known defects, as well as feature requests, planned work, and proposals.

Within the bug database I try to make sure each issue is actionable and discoverable.
I do this by carefully updating the issue subject line, making sure every issue
has steps to reproduce, and using labels to categorize the issue in ways that can be found by GitHub search.

## Comments

### Do not add "me too" or "same" or "is there an update" comments to bugs

I prioritize issues in part based on the number of +1 (thumbs
up) reactions on the top level comment of the bug. Adding comments like "me
too" or "same here" is generally distracting and makes it harder to find
other more meaningful content in the bug. If you have no new details to add,
consider just thumbs upping the issue. If you wish to subscribe to the issue,
click the "subscribe" button in the right hand column of the GitHub UI.

Adding comments explaining how a bug is dire and how you will stop using this repository if it is not fixed is upsetting Me.
Out of a respect for Me, and as required by my [code of conduct](https://github.com/lurkydismal/CCCaster/blob/master/CODE_OF_CONDUCT.md),
I ask that you avoid adding comments that are not actively helpful. There are other
venues if you want to complain without being constructive.

Asking for updates is also not generally helpful, because it just leads to issues
being full of comments asking for updates and that makes finding useful information
in a bug harder (an exception might be if you are participating in the triage process,
but even then consider reaching out to people directly if possible).

### Issues are not always the best venue for discussions

Discussions within an issue should remain focused on the topic, specifically about what the filed issue is and how to solve it.

If you move to another tool for part of the discussion, remember to add a summary of the discussion and document any decisions that took place.
This allows people following the issue to keep updated and continue to participate.

Issues are never an appropriate venue for asking for help with your code. Issues are also not a good venue for discussing repository direction.

### Comments providing workarounds

Providing workarounds for issues can be helpful for developers using this repository and finding a bug,
but please keep such comments to a minimum so as to avoid disrupting from trying to
fix the issue. Rather than discussing workarounds, provide a pointer to another forum
(e.g. Stack Overflow) where workarounds and temporary solutions are more appropriate. Thanks.
However, when a workaround has been identified, consider applying the `workaround available` label to make that info readily available.

### Avoid posting screenshots of text

If you want to show code, quote someone, please avoid sharing it via an image or
screenshot. Text in images cannot be copied, and cannot be automatically
translated via services like Google Translate. This makes it harder for others
who do not speak that language to participate in the issue.

It is perfectly fine to share a screenshot of text rendering invalidly, but
also include the actual string or character(s) that lead to it so that they
can be copied and pasted into a test case.

### Provide reduced test cases

To debug a problem, I will need to be able to reproduce it. The best way
to help us do that is to provide code, that
has been reduced as far as possible (such that removing anything further stops
showing the bug). Attach such a file or files to the issue itself.

For legal reasons, I cannot debug problems that require looking at proprietary
code or, generally, code that is not publicly available.

### Consider posting issues in English

If you are able to read and write English clearly, consider posting your issue
in English, even if it is about a language specific issue (like the way text
renders in some non-English language).

It is fine to post issues in languages other than English, but consider that
many readers will rely on automatic translation services to read your issue.
Please avoid using screenshots in languages other than English, as services like
Google Translate will not translate the text in images, and the pool of people
able to assist you will be reduced.

## Locking an issue

Under normal circumstances, open issues should not regularly be locked. The most
common reason for manually locking an open issue is that issue is well
understood by the one working on it,
is believed to be appropriately prioritized, has a clear
path to being fixed, and is otherwise attracting
a lot of off-topic or distracting comments like "me too" or
"when will this be fixed" or "I have a similar issue that might
or might not be the same as this one".

If you have a similar issue and are not sure if it is the same,
it is fine to file a new issue and linking it to the other issue.
Please avoid intentionally filing duplicates.

Very rarely, an issue gets locked because discussion has become
unproductive and has repeatedly violated the [Code of Conduct](CODE_OF_CONDUCT.md).

### Escalating an issue that has the wrong priority

I regularly look through all issues sorted by the number of thumbs-up reactions to determine the
relative priority of upcoming work, so that is one way to change my mind.

Please do not comment on an issue to indicate your interest.
Comments should be reserved for making progress on the issue.

### Thumbs-up reactions

To vote on an issue, use the "Thumbs-up" emoji to react to the issue.

When examining issues, I use the number of thumbs-up reactions to an issue as a guide to its priority.

I ignore other emoji reactions.

## Labels

The `severe:` prefix indicates labels regarding a level of severity (e.g. regressions, new features, crashes).
Severity in and of itself does not say how fast I will fix the bug;
rather it provides clues as to the nature of the defect, just as other labels do.
A bug may have the `severe: crash` label, but e.g. if it relates to crashing when
run with the system date set to 1998, I am not likely to consider it a high priority.

### Adding labels

Labels are more or less free, so I can add them pretty easily.
Please make sure labels use a consistent color and naming scheme.

Labels should be used for adding information to a bug. If you plan to use a label
to find all instances of a particular topic (e.g. finding all PRs where someone
wrote a design document), be aware that there is no way to force people to label issues
or PRs.

### Naming conventions

Common naming conventions for labels include:
- **`a: *`** - The `a` ("area") prefix is used for labels that are about a specific topic
that could span different layers of implementation.
- **`platform-*`** - The `platform` prefix is for bugs that are specific to one or more platforms.

## Milestones

I do not use GitHub milestones to track work.

## Assigning Issues

Issues are typically self-assigned. Only assign a bug to someone else if
they have explicitly volunteered to do the task. If you do not have permissions
to assign yourself an issue you want to work on, don not worry about it, just
<!-- TODO: Add tree hygiene -->
submit the PR (see [tree Hygiene](TREE_HYGIENE)).

Only assign a bug to yourself when you are actively working on it
or scheduled to work on it. If you do t know when you will be working
on it, leave it unassigned. Similarly, do not assign bugs to
people unless you know they are going to work on it. If you find
yourself with bugs assigned that you have not scheduled specific time
to work on, detach the bug so that other people feel empowered to work on them.

_Do_ assign a bug to yourself if you are working on it, or if you have
scheduled time to work on them and are confident you will do so! This is how
people can figure out what is happening. It also prevents duplicate
work where two people try to fix the same issue at once.

## File bugs for everything

File bugs for anything that you come across that needs doing. When you
implement something but know it is not complete, file bugs for what you
haven not done. That way, I can keep track of what still needs doing.

### Exceptions

Do _not_ file bugs that meet the following criteria:

- Asking meta-questions like "why was bug #XYZ closed?" Instead, post
  on the original issue or raise the actual problem that is still not
  resolved.
- Intentional duplicates like "This is the same as bug #ABC but that
  one is not getting enough attention." Instead, upvote the original
  issue or add a comment that provides new details that are not already
  captured or (best of all) assign it to yourself and start working on it!

### How to propose a specific change

If you have an idea that you would like to land, the recommended process is:

1. File a bug describing the problem.
<!-- TODO: Add design documents -->
2. Write a [design document](DESIGN_DOCUMENTS) that references this problem and describes your solution.
<!-- TODO: Add tree hygiene -->
3. See the [tree hygiene](TREE_HYGIENE) page for details on submitting PRs.

### Every issue should be actionable

Avoid filing issues that are on vague topics without a clear problem description.

Please close issues that are not actionable.

#### Issues should have clear steps to reproduce

Every issue should have a clear description of the steps to reproduce the problem, the expected results, and the actual results.

If an issue is lacking this information, request it from the commenter and close the issue if information is not forthcoming.
