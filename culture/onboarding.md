---
title: Onboarding into Engineering
description: Your first steps to being productive
---

### Onboarding

You have hopefully been onboarded. You have a mentor and a spirit guide. You now know where we keep the snacks!
Awesome.

Some team members have backgrounds in art, but of course not all.
[/recommendations/art.md](/recommendations/art.md) has some useful links if you want to read more about the art
world, or keep up with the latest news.

### Chat

Most of our day-to-day business is conducted in Slack. Teams, offices, and common concerns frequently have their
own channels. For more information on our usage of Slack, see [`/culture/slack.md`](/culture/slack.md).

### GitHub

Artsy stores source code on [GitHub](https://github.com/artsy). Make sure you have an account and are part of the
Artsy organization. If you can't visit [this page](https://github.com/artsy/gravity), then you don’t have the right
access. Your mentor can get you sorted out.

Our projects use physics terms as code names, starting with [Gravity](https://github.com/artsy/gravity) (inspired
by [Zachary Coffin's "Temple of Gravity"](http://www.zacharycoffin.com/work/temple-of-gravity)).

See the [engineering projects map](https://github.com/artsy/potential/wiki/Project-List) for a comprehensive list
of our (many) repos and who owns them. It can be a bit overwhelming, so here are some important ones:

- [Gravity](https://github.com/artsy/gravity): Artsy's main API
- [Force](https://github.com/artsy/force): Artsy web site ([www.artsy.net](https://www.artsy.net))
- [Eigen](https://github.com/artsy/eigen): iOS app
- [Volt](https://github.com/artsy/volt): Content Management system for partners

### AWS

Many applications depend on Amazon Web Services. Your mentor or anyone else in Engineering can set you up with an
IAM profile within our organization's account (see
[instructions](https://github.com/artsy/potential/wiki/Platform-FAQ#add-a-new-aws-user)).

### Engineering-wide Standup

We have an engineering team-wide standup on _Mondays at 11:30 a.m. Eastern_ (virtual:
[https://zoom.us/my/artsyclassroom](https://zoom.us/my/artsyclassroom)) where we:

- Share any team updates
- Mention significant project milestones or new repositories
- Ask for help if we're blocked or need input from a different team
- Plan the week's _lunch and learn_
- Recognize and congratulate each other for significant accomplishments

The standup is fully documented [here](/events/open-standup.md).

### Open Source Culture + Projects

At Artsy, we <3 open source and encourage you to become part of the community. Here is a
[list of some open source technologies](http://artsy.github.io/open-source/) we currently use.

Read @dblock's blog post on
[Becoming Open Source by Default](http://code.dblock.org/2015/02/09/becoming-open-source-by-default.html).

Read this [article by the mobile team](http://www.objc.io/issue-22/artsy.html) on the culture of open source at
Artsy and their reasons behind open-sourcing our [mobile app](https://github.com/artsy/eigen).

Orta also wrote a blog post on the
[mechanics behind open-sourcing Eigen](http://artsy.github.io/blog/2015/04/28/how-we-open-sourced-eigen/).

### Artsy's Stack(s)

Read @orta's
[blog post describing our stack in 2017](http://artsy.github.io/blog/2017/04/14/artsy-technology-stack-2017/),
which evolved from [our stack in 2015](http://artsy.github.io/blog/2015/03/23/artsy-technology-stack-2015/), which
evolved from [our tech stack at launch in 2012](http://artsy.github.io/blog/2012/10/10/artsy-technology-stack/),
which evolved from a Rails monolith.

### Artsy APIs

See [apis](https://github.com/artsy/potential/blob/master/apis/README.md) in Potential.

### Artsy Data

See [data](https://github.com/artsy/potential/blob/master/data/README.md).

## How We Work

The engineering team [Playbook](/playbooks/being-an-artsy-engineer.md) discusses why we make the technical and
non-technical decisions we do.

### Development Environments

The [scripts/setup](https://github.com/artsy/potential/blob/master/scripts/setup) script will install common
dependencies for local development (homebrew, Ruby, etc.).

Projects can provide their own setup scripts that build on this common foundation. See
[Gravity's script/setup](https://github.com/artsy/gravity/blob/master/script/setup) as an example.

### Text Editor

Most engineers use [Visual Studio Code](https://code.visualstudio.com), but feel free to use whatever makes you
most comfortable. We recommend that projects include a `.vscode` folder with settings, and an
[extensions.json](https://code.visualstudio.com/docs/editor/extension-gallery#_workspace-recommended-extensions) so
that developers can have the same experience. For example:

- [reaction](https://github.com/artsy/reaction/tree/master/.vscode)
- [emission](https://github.com/artsy/emission/tree/master/.vscode)
- [metaphysics](https://github.com/artsy/metaphysics/tree/master/.vscode)
- [force](https://github.com/artsy/force/tree/master/.vscode)
- [positron](https://github.com/artsy/positron/tree/master/.vscode)

A lot of engineers have moved from Sublime Text or vim, if you want to retain your keyboard shortcuts / modes, you
can find a
[list of extensions handling that](https://code.visualstudio.com/docs/getstarted/keybindings#_keymap-extensions).

### Contributing Code

As all of our code is housed on GitHub, we make contributions through
[pull requests](http://artsy.github.io/blog/2012/01/29/how-art-dot-sy-uses-github-to-build-art-dot-sy/).

Read more in [the Playbook](/playbooks/being-an-artsy-engineer.md#workflow) or see this
[step-by-step guide](https://github.com/artsy/potential/blob/master/github/workflow.md). If you're unfamiliar with
Git, check out this [short tutorial](https://try.github.io) on basic git commands (such as `git status`,
`git commit`, and `git push`).

### Deploying

Once your pull request is merged, we use services like [CircleCI](https://circleci.com/) to run the full test suite
to make sure code changes did not break existing features.

Many of our apps automatically deploy to a staging environment once CI (continuous integration) succeeds.
Production deploys vary by project, but are usually documented in project READMEs.

We try to deploy early and often. You don't need permission to deploy--just announce in #dev slack channel in case
the team has any concerns.

More about [continuous improvement](/playbooks/being-an-artsy-engineer.m#continuous-improvement).

### Getting Help

- **Slack:** If you know what team could potentially help you, browse the channels in Slack to find the most
  relevant place to ask your question. If you aren't sure, [#dev](https://artsy.slack.com/messages/dev) is a good
  place to start.
- **Ask Your Neighbor:** Everyone is friendly. Don't hesitate to reach out to the people around you for even the
  most basic of questions.
- **Check Atlas:** Turns out a lot of common questions are available in [atlas.artsy.net](http://atlas.artsy.net) .
