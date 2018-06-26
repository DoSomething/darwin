# Darwin

This is our working manifesto, which we keep as a public document. It has details specific to the product, engineering, and data teams, but a lot of it is just about how to work together effectively and bring out the best in each other.

## The basics

Each member of the team is responsible for making this a great place to work, and for maximizing the power of technology to realize DoSomething's vision: the most young people doing the most good.

### Everything is an experiment
We're always looking for better ways to work, and end each sprint with a retrospective to find these improvements. The retro runs in the usual start-stop-continue style. We hold an all-teams retro, which is great for general culture and surfacing larger questions or issues. Individual teams also hold their own retros, which focus more tightly on that team's work and goals.

This entire document is just a pull request away from change. The same is true of our team structures and working arrangements. We’ve arrived at our current arrangement through steady evolution, and we’re willing to keep evolving. The qualities we work to protect have to do with how we communicate and respect each other, and how we hold each other accountable to great work and a great attitude. The rest can change.

### Diversity
We know that our diversity—of gender identity, ethnicity, race, sexual orientation, age, education, religion, geography, you name it—makes us better communicators, because it reduces the chance that we'll thoughtlessly agree to a prevailing opinion. We seek out teammates who make us more diverse.

### Trust
As Google’s [Project Aristotle](https://www.nytimes.com/2016/02/28/magazine/what-google-learned-from-its-quest-to-build-the-perfect-team.html) shows, we succeed only when we trust one another. We understand that no one on the team is perfect. When you make a mistake, own up to it and learn from it. Trust is formed by growing and learning from mistakes as a team.

### Communication
While most people are in the New York office, not everyone is, and most people work remotely at least some of the time. Communication and documentation are crucial. Make liberal use of the tools we use to include everyone in the conversation: Slack, video chat, Google Drive and Calendar, Pivotal Tracker, and GitHub. Write everything down. No tech decision, launch date, product build, or product funeral should come as a shock to the people working on it.

Be courteous in communications: The opportunity for misunderstanding is greater with online interactions. Ask if you’re missing some important information. Use emoji. Give context. Read what other people have said before hitting send on your message. Slack is instant, but that doesn't mean you have to reply in an instant.

We encourage feedback in all directions, because it helps us improve. The sooner you're able to provide feedback the better. Within 48 hours is generally a good rule of thumb. A favorite structure for providing feedback is SBI:

* Situation
* Behavior
* Impact

Check out this [10 minute guide](https://www.mindtools.com/blog/corporate/wp-content/uploads/sites/2/2014/05/SBI-Feedback-Tool.pdf) for more on SBI.

Giving feedback to peers is hard. It usually feels awkward. But, when you get constructive, timely, actionable feedback from a peer, you realize it’s gold. It’s what you’ve always wanted to know from your colleagues. We talk about peer feedback a lot, because we realize that it’s both difficult and really valuable.

### Collaboration
When you join DoSomething, you join a team. [Hold strong opinions, weakly](http://blog.codinghorror.com/strong-opinions-weakly-held/).
We build products together, and have debates about everything before we build it. We want everyone to be on the same page.

This goes both ways: when explaining something make sure to present enough context for everyone to contribute to the conversation. Conversely, if something is unclear, ask.

We also share responsibility for our work. At Facebook, they say that ["Nothing at Facebook is someone else's problem."](https://medium.com/facebook-design/how-we-changed-the-facebook-friends-icon-dc8526ea9ea8#.tjb5mkj4u) We try to live that—our version is, “It’s everybody’s site.” The products and experiences we create are a direct reflection of the structure of our teams, how we communicate, and what we value.

### Unacceptable behaviors
_Stolen and hardly adapted from [Vox](http://code-of-conduct.voxmedia.com/)_

We are committed to providing a welcoming and safe environment for people of all races, gender identities, gender expressions, sexual orientations, physical abilities, physical appearances, socioeconomic backgrounds, nationalities, ages, religions, and beliefs. Discrimination and harassment are expressly prohibited in our employee handbook. Harassment includes, but is not limited to, intimidation; stalking; unwanted photography; inappropriate physical contact; use of sexual or discriminatory imagery, comments, or jokes; sexist, racist, ableist, or otherwise discriminatory or derogatory language; and unwelcome sexual attention.

Furthermore, any behavior or language which is unwelcoming—whether or not it rises to the level of harassment—is also strongly discouraged. A lot of exclusionary behavior takes the form of microaggressions: subtle put-downs that may be unconsciously delivered. Regardless of intent, microaggressions can have a significant negative impact on victims and have no place on our team.

There are a host of behaviors and language common on tech teams which are specifically unwelcome: Avoid “well, actuallys”—pedantic corrections that are often insulting and unproductive; make an effort not to interrupt your colleagues while they are speaking; never respond with surprise when someone asks for help; and take care neither to patronize your colleagues nor assume complete knowledge of a topic. This last point is especially important when talking about technical topics: Many women and people of color in the tech industry have many tales of being either [mansplained](https://www.guernicamag.com/daily/rebecca-solnit-men-explain-things-to-me/) about a field in which they are experts, or else excluded from learning opportunities because a colleague wouldn’t make an effort to answer questions. Don’t be that person! Remember, your colleagues may have expertise you are unaware of. Listen more than you speak.

## How we get work done
All of our code is open source and on GitHub. We organize stories and plan sprints with Pivotal Tracker, and maintain our roadmaps in Teamweek. Individual coding tasks are tracked as GitHub issues. We use pull requests to review and merge changes. Every PR is peer-reviewed. Please see here for an overview of our [Teams, Services, and Environments](http://docs.dosomething.org/engineering/overview).

### Code review and pull requests
We work in branches, generally off of dev (or master, depending on the project). We commit often, to capture our thinking. We package up our work as pull requests, and try to keep PRs reasonably small. (This also makes it more likely someone will review your PR!)

A teammate must review your PR, get their questions answered, and give a +1 as approval before you can merge your changes. The main branch is [protected](https://help.github.com/articles/about-required-reviews-for-pull-requests/). The reason we review code is not just to catch bugs, but because we want to improve the quality of code that we ship. We want our code to be maintainable, easily understood, and [stylish](https://github.com/DoSomething/code-style). If you push code to production, you’re implicitly vouching for it as an example of how to write code at DoSomething. When possible, we use StyleCI to enforce coding style and conventions. StyleCI gets called for each PR and update.

#### Making a pull request

- If your code is not ready for review, or is a prototype that won't be merged, don't create a pull request—or create one prefixed with DON’T MERGE in the title
- When you create a pull request, fill out the [pull request template](https://github.com/blog/2111-issue-and-pull-request-templates)
- Highlight any areas you would particularly like review on

#### Giving feedback on a pull request

- Ask questions, don't make demands
- Be mindful about how comments come off: "Did you think about" is better than "Why didn't you just..."
- Compliment! If you see something you like, let them know
- If you see multiple examples of the same thing (spelling, caps) don't comment every time, rather make one comment saying you noticed it throughout
- Give context for your comments, so they don’t read as arbitrary
- If you see a code smell, point them to the [prescription](https://sourcemaking.com/refactoring/smells)

#### What should the reviewer look for?

- Does this PR solve the issue it's referencing?
- Is the code readable?
- Is it well commented?

#### Responding to feedback on your pull request

- Don't take comments personally: it should be a conversation, not a personal attack
- Make sure you understand _why_ you're making the requested changes: Does it make sense? Does it improve the code?
- After you're done implementing the changes, re-ping for a second review!

### API design
We love the book [Build APIs you won't hate](https://leanpub.com/build-apis-you-wont-hate). Follow RESTful standards when dealing with RESTful things, like CRUD operations.

Version your API when making significant changes. With the proliferation of interrelated services in our environment, it can be very difficult to know whether a substantial change to an endpoint you own will have side effects elsewhere. There are [plenty of good resources](http://www.baeldung.com/rest-versioning) out there, as well as established practices at DoSomething. Talk to your fellow engineers to make sure your approach makes sense.

### DevOps

We value deploying often and easily over using the latest and greatest. This means we accept that we need to run new software on existing tech stacks as a first, second, and third option. A lot of our tech choices are [boring on purpose](http://mcfunley.com/choose-boring-technology).

We constantly seek to simplify our toolset and our production environment, because simplicity brings greater understanding, easier automation, more security, and better reliability. (Simplifying is hard, and takes vigilance.)

At least two sprints before a new system goes into production, the responsible team needs to review (at least) these requirements with the DevOps team.

- Mission criticality (an experiment, an add-on, or a new critical service?)
- Architecture and tech stack walkthrough
- Hosting paradigm: Can this run in a serverless environment?
- Deployment mechanism
- Data storage & backup
- Security and member data privacy
- ETL (data extraction) processes
- New Relic and other monitoring integrations
- Milestone dates (launch, etc.) on the shared Tech Dates calendar
- QA and Production DNS entries
- LogStash support

Some apps may also require the following support:

- Instrumentation of significant user or business events
- Transactional ID handling (for instance, with our [Gateway](https://github.com/DoSomething/gateway) project)
- Runscope or Ghost Inspector tests for monitoring and debugging
- TLS requirements
- Laravel Queue requirements
- [Blink](https://github.com/DoSomething/blink) (message bus) integration
- Fastly support

### Deployments
We deploy as often as we can, and look for ways to increase the frequency. We have ChatOps integration through Slack, where possible (e.g., [Heroku](https://devcenter.heroku.com/articles/chatops)).

We use both Jenkins and Wercker for deploys. Jenkins is standard for the Phoenix deploys, Wercker for most other deploys. Heroku-hosted apps use the standard Heroku deployment workflow.

### Hosting infrastructure
We host on AWS and Heroku.

#### Amazon
The bulk of our environment is hosted in AWS. We make heavy use of EC2, RDS, EBS, and S3.

#### Heroku
We run as much as we can on Heroku, because that environment puts devs in direct control of the deployment mechanism, and because we reduce our server footprint in AWS.

### Testing & monitoring
We maintain quality with unit and functional testing, and we’re constantly trying to find better ways to test. We strongly prefer frameworks, like Laravel, that have unit testing built in to their core.

We monitor with New Relic, StatHat, Runscope, and Ghost Inspector. We centralize alerts and alerting policies in PagerDuty.

### Documentation
We believe in great documentation—not for documentation's sake, but to make on-boarding and institutional memory better. Writing good docs also makes you more thoughtful about your choices. It's like teaching: you can't teach something you haven't thought through all the way.

We document in code (doc blocks, etc.), and in Markdown Readme files in the source repos. Sometimes the project-level Readme is sufficient, but for [bigger projects](https://github.com/DoSomething/northstar/tree/dev/documentation) we'll break the docs into their own directory.

### Data collection
We collect raw data in our [Quasar](https://github.com/DoSomething/quasar) warehouse; we prefer making apps push their events to the warehouse rather than writing ETL tools to scrape APIs.

We use Looker to surface and explore data.

## Titles & career growth

We have a standard set of position levels across the organization:

* Associate
* Manager
* Director
* C-Level

Positions within product and engineering implicitly follow those levels as well, but we add more structure to our job titles because it maps more clearly onto the outside world. We don't want anyone to have an idiomatic title (“Deputy Chief Monster Imagineer") that might be a hindrance to making a great career move after DoSomething.

It's possible to switch between management and technical track—there's not a rigid border. But it's important to know that you can have a rich career in either direction.

#### Technical track

* Junior Software Engineer (JSE)
* [SE](Positions/SoftwareEngineer.md)
* [SSE](Positions/SeniorSoftwareEngineer.md)
* [Staff Engineer](Positions/StaffEngineer.md)
* [Technical Lead](Positions/Roles/TechTeamLead.md): This is a role to play on a team, not a job title. The tech team lead serves as the engineering point person for a particular team, helps to define and delegate work, provide estimates, and make architectural decisions. Tech team leads do not manage the other engineers' careers, only their work. There is another version of this role that is technical only (does not involve leading a team), meaning that the engineer is responsible for leading, designing, and serving as the main maintainer of a large project/application/service. There is overlap in responsibilities at a high level. Technical leads gather for a monthly architecture governance meeting, where they work together on systems integration and other high-level topics. 

More information on the roles and responsibilities can be viewed either as a grid [here](https://docs.google.com/spreadsheets/d/1c0Ags_6-aJEEBuMC46pw5hshsmOD20IKuhPjigBbcSM/edit?usp=sharing) or on the different position pages linked to above.

#### Engineering Management track

_We don’t have people in all of these positions, but this is still the progression._

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
