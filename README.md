# Darwin

This is our working manifesto, which (obviously) we keep as a public and open-source document. It has details specific to the product, engineering, data, messaging, and mobile teams, but a lot of it is just about how to work together effectively and bring out the best in each other.

## Core Values 
or, we hold these truths to be self evident that all _people_ are created equal.

### When rules suck, break them (together)
This entire document is just a pull request away from change. The same is true of our team. We appreciate our sprint retros so much because (beer and also) they're a time when we can question anything about what we do, and how we work.

Each member of the team is responsible for making this a great place to work, and for maximizing the power of technology to realize DoSomething's vision: the most young people doing the most good.

### Everything is an experiment
We're always looking for better ways to work, and end each sprint with a retrospective. The retro runs in the usual start-stop-continue style.

### Diversity
We know that our diversity -- of gender, ethnicity, race, education, geography, you name it -- makes us better communicators, because it reduces the chance that we'll thoughtlessly agree to a prevailing opinion. We seek out teammates who make us more diverse.

### Trust
We succeed only when we trust one another. We understand that no one on the team is perfect. When  you make a mistake, own up to it and learn from it. Trust is formed from by growing and learning from mistakes as a team. 

### Communication
While most people are in the New York office, not everyone is, most people are remote or WFH at least some of the time. Communication and documentation are important. Make liberal use of the tools we use to include everyone in the conversation, slack, hangouts, google docs and github. Write everything down. No tech decision, launch date, product build or product funeral should come as a shock to the people working on it. 
Be polite in communications, keep in mind tone and the opportunity for missunderstanding is greater with online interactions. Use emoji. Explain. Read what other people have said before hitting send on your message. Slack is instant, but that doesn't mean you have to reply in an instant. 

### Collaboration
When you join DoSomething, you join a team. [Hold strong opinions, weakly](http://blog.codinghorror.com/strong-opinions-weakly-held/)
We build products together, and have debates about everything before we build it. We want everyone to be on the same page. 

### Unacceptable behaviors 
(stolen and hardly adapted from [Vox](http://code-of-conduct.voxmedia.com/))

We are committed to providing a welcoming and safe environment for people of all races, gender identities, gender expressions, sexual orientations, physical abilities, physical appearances, socioeconomic backgrounds, nationalities, ages, religions, and beliefs. Discrimination and harassment are expressly prohibited in our employee handbook. Harassment includes, but is not limited to, intimidation; stalking; unwanted photography; inappropriate physical contact; use of sexual or discriminatory imagery, comments, or jokes; sexist, racist, ableist, or otherwise discriminatory or derogatory language; and unwelcome sexual attention.

Furthermore, any behavior or language which is unwelcoming—whether or not it rises to the level of harassment—is also strongly discouraged. Much exclusionary behavior takes the form of microaggressions—subtle put-downs which may be unconsciously delivered. Regardless of intent, microaggressions can have a significant negative impact on victims and have no place on our team.

There are a host of behaviors and language common on tech teams which are worth noting as specifically unwelcome: Avoid “well, actuallys”—pedantic corrections that are often insulting and unproductive; make an effort not to interrupt your colleagues while they are speaking; never respond with surprise when someone asks for help; and take care neither to patronize your colleagues nor assume complete knowledge of a topic. This last point is especially important when talking about technical topics: Many women and people of color in the tech industry have many tales of being either [mansplained](https://www.guernicamag.com/daily/rebecca-solnit-men-explain-things-to-me/) about a field in which they are experts, or else excluded from learning opportunities because a colleague wouldn’t make an effort to answer questions—don’t be that person. Remember, your colleagues may have expertise you are unaware of. Listen more than you speak.



## How we get work done
All of our code is open source and on GitHub. We work with GH Issues and pull requests. Every PR is peer-reviewed.


### Code review and pull requests
We do work in branches, generally off of dev (or master, depending on the project). We commit often, to capture our thinking. We package up our work as pull requests, and try to make these PRs as small as possible.

A teammate must review our PR and give a +1 as approval before we can merge our changes. There's no tooling to prevent our merging in changes. We enforce this by personal behavior, not by mechanics.

When possible, we use StyleCI to enforce coding style and conventions. StyleCI gets called for each PR and update.


### API design
We love the book [Build APIs you won't hate](https://leanpub.com/build-apis-you-wont-hate). And follow RESTful standards.  

### Data collection

### Deploying code
We deploy as often as we can, and look for ways to increase the frequency. We have ChatOps integration through Slack and George, which is our customized Hubot.

For projects under active development, we usually deploy daily. The most demanding deployments are on Phoenix, our main web app. This is a Drupal 7 app and a pain to test. We've automated much of the critical-path testing via Ghost Inspector, which reports results through Slack.

In Slack, a Phoenix deployment looks like `@george deploy production v2.2.53`, so we can target version and environment.

We use both Jenkins and Wercker for deploys. Jenkins is standard for the Phoenix deploys, Wercker for most other deploys.


### Infrastructure & DevOps
We host on AWS, Google Cloud, and Heroku.


#### AWS
Our main environment, including our user-facing web apps, user and content APIs, and message broker architecture, is on Amazon.


#### Google Cloud
We're building our data ingestion and warehousing on Google. There are networking bandwidth advantages that have been helpful.


#### Heroku
Several services, such as George/Hubot, are hosted on Heroku. It's easy, quick, and either cheap or free for us. It's a good hosting tool for quick hacks and prototypes.


### Testing & monitoring
We maintain quality with unit and functional testing, but we’re constantly trying to find better ways to test. We know that unit testing can suck/be impossible in some situations (e.g., Drupal), so we look for other ways, like Ghost Inspector.

We monitor with New Relic, StatHat, Runscope, and Ghost Inspector.


### Documentation
We believe in great documentation -- not for documentation's sake, but to make on-boarding and institutional memory better. Writing good docs also makes you more thoughtful about your choices. It's like teaching: you can't teach something you haven't thought through all the way.

We document in code (doc blocks, etc.), and in Markdown Readme files in the source repos. Sometimes the project-level Readme is sufficient, but for [bigger projects](https://github.com/DoSomething/northstar/tree/dev/documentation) we'll break the docs into their own directory.


## How our teams work

### Titles & career growth
We try to keep some structure to our job titles because it maps more clearly onto the outside world. We don't want anyone to have an idiomatic title ("Chief monster imagineer") that might be a hindrance to making a great career move after DoSomething.

It's possible to switch between management and technical track -- there's not a rigid border. But it's important to know that you can have a rich career in either direction.

We don't have people with all of these titles. But this structure makes sense to us (for now).


#### Technical track

* Junior Software Engineer (JSE)
* [SE](Positions/SoftwareEngineer.md)
* [SSE](Positions/Positions/SeniorSoftwareEngineer.md)
* Principal Engineer / Application Architect: PE might be more hands-on than AA.


#### Management track

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
