---
# (required) default post layout
layout: post
# (require) a string title
title: "GitHub CLI: Managing Pull Requests"
# (require) a post date
date: 2022-06-20 12:55:34 -05:00
# (custom) some categories, but makesure these categories already exists inside path of `category/`
categories: [git, github-cli, instructional]
# (custom) tags only for meta `property="article:tag"`
tags: [git, github-cli, pull-requests, instructional]
---

<hr>

As I try to move away from GUI's and more into a text-based environment, I find myself coming to points where I need to stop and branch out my knowledge.

Currently when I'm finished with a feature or project, I need to rely on GitHub's GUI for manipulating and managing my pull requests.

I've been fine with managing my code base this way until now and although the GitHub CLI can be a bit intimidating, it looks like a powerful tool and I'm excited to learn it.

<hr>

The following responses are color-coded:
- <span style="color: green">**Open**</span>
- <span style="color: purple">**Merged**</span>
- <span style="color: red">**Deleted**</span>

List all open pull requests
```bash
$ gh pr list
```

To view *all* pull requests (*past and present*)
```bash
gh pr list --state "all"

# or shortened

gh pr list -s "all"
```

List assigned pull requests by user
```bash
gh pr list --assignee 'harryrf3'
```

Check pull request status
```bash
gh pr status

# responses -
#  Current branch
#  Created by you
#  Requesting a code review from you
```

List closed pull requests
```bash
gh pr list --state 'closed'

# shortened

gh pr list -s 'closed'
```

List labeled pull requests
```bash
gh pr list --label 'bug'

# shortened

gh pr list -l 'bug'
```

Open pull requests from command line
```bash
# reference pr by number, branch, or url

gh pr view '3'

```

Create pull request for current branch
```bash
# shortened

gh pr create -t 'TITLE' -b 'BODY'
```

Create pull request from browser
```bash
# when running into issues with the cli

gh pr create --web
```

Checkout branch for pull request
```bash
# checks out branch pull request is on

gh pr checkout '14'
```

Command line aliases for command line pull requests management
```bash
# list pull requests under 'bug' label

alias listprs='gh pr list --label "bug"'

# list pull requests that are assigned to me

alias listmyprs='gh pr list -a "harryrf3"'
```

<br/>

> references: <br/>
> [goobar](https://www.youtube.com/watch?v=Ku9_0Mftiic) - Use GitHub CLI For Command Line Pull Request Management 
