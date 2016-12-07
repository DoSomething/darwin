# Darwin

This is our working manifesto, which (obviously) we keep as a public and open-source document. It has details specific to the product, engineering, data, messaging, and mobile teams, but a lot of it is just about how to work together effectively and bring out the best in each other.

## The basics
_Or, we hold these truths to be self-evident, that all_ people _are created equal._

### When rules suck, break them (together)
This entire document is just a pull request away from change. The same is true of our team. We appreciate our sprint retros so much because (beer and also) they're a time when we can question anything about what we do, and how we work.

Each member of the team is responsible for making this a great place to work, and for maximizing the power of technology to realize DoSomething's vision: the most young people doing the most good.

### Everything is an experiment
We're always looking for better ways to work, and end each sprint with a retrospective. The retro runs in the usual start-stop-continue style.

### Diversity
We know that our diversity—of gender, ethnicity, race, education, geography, you name it—makes us better communicators, because it reduces the chance that we'll thoughtlessly agree to a prevailing opinion. We seek out teammates who make us more diverse.

### Trust
We succeed only when we trust one another. We understand that no one on the team is perfect. When you make a mistake, own up to it and learn from it. Trust is formed by growing and learning from mistakes as a team.

### Communication
While most people are in the New York office, not everyone is, and most people are remote or working from home at least some of the time. Communication and documentation are crucial. Make liberal use of the tools we use to include everyone in the conversation: Slack, Gangouts, Google docs, and GitHub. Write everything down. No tech decision, launch date, product build or product funeral should come as a shock to the people working on it.

Be polite in communications: the opportunity for misunderstanding is greater with online interactions. Use emoji. Explain. Read what other people have said before hitting send on your message. Slack is instant, but that doesn't mean you have to reply in an instant.

We encourage feedback in all directions, it makes us better. The sooner you're able to provide feedback the better. Within 48 hours is generally a good rule of thumb. A favorite structure for providing feedback is SBI:

* Situation
* Behavior
* Impact

Check out this [10 minute guide](https://www.mindtools.com/blog/corporate/wp-content/uploads/sites/2/2014/05/SBI-Feedback-Tool.pdf) for more, and this [template](http://www.ccl.org/leadership/pdf/community/SBIJOBAID.pdf) if you need help organizing your thoughts.

### Collaboration
When you join DoSomething, you join a team. [Hold strong opinions, weakly](http://blog.codinghorror.com/strong-opinions-weakly-held/).
We build products together, and have debates about everything before we build it. We want everyone to be on the same page.

This goes both ways: when explaining something make sure to present enough context for everyone to contribute to the conversation. Conversely, if something is unclear, ask.

We also share responsibility for our work. At Facebook, they say that ["Nothing at Facebook is someone else's problem."](https://medium.com/facebook-design/how-we-changed-the-facebook-friends-icon-dc8526ea9ea8#.tjb5mkj4u). The MTA has their famous slogan: "If you see something, say something." At DoSomething we embody this with our own saying: "It's everyone's site." This of course extends to our mobile apps, admin apps, and the whole organization.

In order to accomplish this we foster curiosity. We trust each other, AND we know our ideas are made stronger when they are questioned. This culminates in our concept of collaborative accountability. We work together to make our products, experiences, and work processes better; we share responsibility for putting our best work forward; and we have owners who make sure that each component of what we do is working as expected.

### Unacceptable behaviors
_(Stolen and hardly adapted from [Vox](http://code-of-conduct.voxmedia.com/))_

We are committed to providing a welcoming and safe environment for people of all races, gender identities, gender expressions, sexual orientations, physical abilities, physical appearances, socioeconomic backgrounds, nationalities, ages, religions, and beliefs. Discrimination and harassment are expressly prohibited in our employee handbook. Harassment includes, but is not limited to, intimidation; stalking; unwanted photography; inappropriate physical contact; use of sexual or discriminatory imagery, comments, or jokes; sexist, racist, ableist, or otherwise discriminatory or derogatory language; and unwelcome sexual attention.

Furthermore, any behavior or language which is unwelcoming—whether or not it rises to the level of harassment—is also strongly discouraged. Much exclusionary behavior takes the form of microaggressions—subtle put-downs which may be unconsciously delivered. Regardless of intent, microaggressions can have a significant negative impact on victims and have no place on our team.

There are a host of behaviors and language common on tech teams which are worth noting as specifically unwelcome: Avoid “well, actuallys”—pedantic corrections that are often insulting and unproductive; make an effort not to interrupt your colleagues while they are speaking; never respond with surprise when someone asks for help; and take care neither to patronize your colleagues nor assume complete knowledge of a topic. This last point is especially important when talking about technical topics: Many women and people of color in the tech industry have many tales of being either [mansplained](https://www.guernicamag.com/daily/rebecca-solnit-men-explain-things-to-me/) about a field in which they are experts, or else excluded from learning opportunities because a colleague wouldn’t make an effort to answer questions—don’t be that person. Remember, your colleagues may have expertise you are unaware of. Listen more than you speak.

## How we get work done
All of our code is open source and on GitHub. We work with GH Issues and pull requests. Every PR is peer-reviewed. We maintain our roadmaps and feature requests in Trello.

### Code review and pull requests
We do work in branches, generally off of dev (or master, depending on the project). We commit often, to capture our thinking. We package up our work as pull requests, and try to make these PRs as small as possible.

A teammate must review your PR and give a +1 as approval before we can merge our changes. The main branch is [protected](https://help.github.com/articles/about-required-reviews-for-pull-requests/), it must be reviewed before a merge. The reason we review code is not to catch bugs, we want to improve the quality of code that we ship. We want our code to be maintanable, easily understood, and [stylish](https://github.com/DoSomething/code-style). If you put code into production, you vouch that it can be an example of how to write code for our site. When possible, we use StyleCI to enforce coding style and conventions. StyleCI gets called for each PR and update.

__Making a pull request__
- If your code is not ready for review, or is a prototype that won't be merged, don't create a pull request
- When you create a pull request, fill out the pull request template
- Highlight any areas you would particularly like review on

__Giving feedback on a pull request__
- Ask questions, don't make demands
- Be mindful about how comments come off: "Did you think about" is better than "Why didn't you just..."
- Compliment! If you see something you like, let them know
- If you see multiple examples of the same thing (spelling, caps) don't comment every time, rather make one comment saying you noticed it throughout
- Give context for your comments: "What are the benefits of refactoring X?" Without context, comments may seem arbitrary
- If you see a code smell, point them to the [prescription](https://sourcemaking.com/refactoring/smells)

__What should the reviewer look for?__
- Does this solve the issue it's referencing?
- Is the code readable?
- Is it well commented?

__Responding to feedback on your pull request__
- Don't take comments personally: it should be a conversation not a personal attack
- Make sure you understand _why_ you're making the requested changes: Does it make sense? Does it improve the code?
- After you're done implementing the changes, re-ping for a second review!

### API design
We love the book [Build APIs you won't hate](https://leanpub.com/build-apis-you-wont-hate). And follow RESTful standards when we're dealing with RESTful things, like CRUD operations.

### DevOps
We value deploying often and easily over rapidly evolving our toolsets. This means we accept that we need to run new software in existing environments as a first, second, and third option.

We know that we can get amazing work done with the tools we already have. We seek to constantly simplify our toolset and our production environment, because simplicity brings greater understanding, easier automation, more security, and better reliability.

At least two sprints before a new system goes into production, the responsible team needs to review (at least) these requirements with the DevOps team.

- Architecture and tech stack walkthrough
- Deployment mechanism
- Data storage & backup requirements
- New Relic integration
- Milestone dates (e.g., launch) on the Tech Dates calendar
- QA and Production DNS entry requirements
- LogStash support

Some apps may also require the following support.

- StatHat coverage of significant events
- Transactional ID handling (for instance, with our [Gateway](https://github.com/DoSomething/gateway) project)
- Runscope or Ghost Inspector tests for monitoring and debugging
- SSL requirements
- Laravel Queue requirements
- CDN support

### Deployments
We deploy as often as we can, and look for ways to increase the frequency. We have ChatOps integration through Slack and George, which is our customized Hubot.

For projects under active development, we usually deploy daily. The most demanding deployments are on Phoenix, our main web app. This is a Drupal 7 app and a pain to test. We've automated much of the critical-path testing via Ghost Inspector, which reports results through Slack.

In Slack, a Phoenix deployment looks like `@george deploy production v2.2.53`, so we can target version and environment.

We use both Jenkins and Wercker for deploys. Jenkins is standard for the Phoenix deploys, Wercker for most other deploys.

### Hosting infrastructure
We host on AWS, Heroku, and Digital Ocean.

#### AWS
Our main environment, including our user-facing web apps, user and content APIs, and Quicksilver (messaging) architecture, is on Amazon.

#### Heroku
Several services, such as George/Hubot, and [Gambit](https://github.com/DoSomething/gambit), our messaging engine, are hosted on Heroku. It's easy, quick, and either cheap or free for us. It's a good hosting tool for quick hacks and prototypes, but can also scale for production.

#### Digital Ocean
Some of our data warehouse is on Digital Ocean.

### Testing & monitoring
We maintain quality with unit and functional testing, but we’re constantly trying to find better ways to test. We know that unit testing can suck/be impossible in some situations (e.g., Drupal), so we look for other ways, like Ghost Inspector. But we strongly prefer frameworks that make it easier to unit test.

We monitor with New Relic, StatHat, Runscope, and Ghost Inspector. We centralize alerts and alerting policies in PagerDuty.

### Documentation
We believe in great documentation—not for documentation's sake, but to make on-boarding and institutional memory better. Writing good docs also makes you more thoughtful about your choices. It's like teaching: you can't teach something you haven't thought through all the way.

We document in code (doc blocks, etc.), and in Markdown Readme files in the source repos. Sometimes the project-level Readme is sufficient, but for [bigger projects](https://github.com/DoSomething/northstar/tree/dev/documentation) we'll break the docs into their own directory.

### Data collection
[TK]

## How our teams work

### Titles & career growth
We have a standard set of position levels across the organization:

* Associate
* Manager
* Director
* C-Level

Positions within product and engineering follow those levels as well. Where it makes sense we try to add more structure to our job titles because it maps more clearly onto the outside world. We don't want anyone to have an idiomatic title ("Chief monster imagineer") that might be a hindrance to making a great career move after DoSomething.

It's possible to switch between management and technical track—there's not a rigid border. But it's important to know that you can have a rich career in either direction.

We don't have people with all of these titles. But this structure makes sense to us (for now).

#### Technical track

* Junior Software Engineer (JSE)
* [SE](Positions/SoftwareEngineer.md)
* [SSE](Positions/SeniorSoftwareEngineer.md)
* Principal Engineer / Application Architect: PE might be more hands-on than AA.

#### Engineering Management track

* Technical Lead: This is a hybrid of technical seniority and management. The exact balance may change depending on the role or the team, and could go 100% in one direction.
* Engineering Manager
* Director of Engineering
* VP, Engineering
* CTO

#### Product track

* Junior Product Manager (JPM)
* PM
* Senior PM
* Director of PM
* Head of Product
