# PuppetConf Speaker Schedule & Notes


## Tuesday September 23, 2014


#### 9:00am - Keynote: Nearly a Decade of Puppet: What We've Learned and Where We're Going Next - Luke Kanies, Puppet Labs

##### Date
Tuesday September 23, 2014 9:00am - 9:50am

##### Location
Salon 7-9 (Lower B2)

##### About
Luke founded Puppet and Puppet Labs in 2005 out of fear and desperation, with
the goal of producing better operations tools and changing how we manage
systems. He has been publishing and speaking on his work in system
administration since 1997, focusing on development since 2001. He has developed
and published multiple simple sysadmin tools and contributed to established
products like Cfengine, and has presented on Puppet and other tools around the
world, including at OSCON, LISA, Linux.Conf.au, and FOSS.in. His work with
Puppet has been an important part of DevOps and delivering on the promise of
cloud computing. He serves as a board member for the Technology Association of
Oregon.

##### Notes
- Automate what you can so you an work on the interesting things!
- OUDA loop (evolving more quickly, ability to make decisions quicker)
- Clients going native!! - Rewritten all of 'facter' in c++
- Next generation Puppet Server
  - porting a bunch of services into clojure
  - "More Scaleable" puppet master (hehe)
  - Language changes
    - Data typing
    - iteration
    - "Lingua Franca" in the datacenter
- Moduke forge:
  - Announcing Puppet Approved modules (sigh..)
  - Puppet Supported Modules
- Futureparser?!
- Puppet Applications
  - Independent of the platform
  - Decoupled from each other
  - Puppet Apps available via Puppet Enterprise
    - Puppet Node Manager
- Instrumentation service built into the new Puppet Server
- ha-proxy load balancer between two puppet masters


#### 9:55am - Keynote: The Phoenix Project: Lessons Learned - Gene Kim, IT Revolution Press

##### Date
Tuesday September 23, 2014 9:55am - 10:20am 

##### Location
Salon 7-9 (Lower B2)

##### About
Gene Kim is a multiple award-winning CTO, researcher and author. He was founder
and CTO of Tripwire for 13 years, and has researched high performing IT
organizations for almost as long. He has written three books, including "The
Visible Ops Handbook" and "The Phoenix Project: A Novel About IT, DevOps, and
Helping Your Business Win."

##### Notes
- Technical Debt: It is what we feel the next time we want to make a change
- Four lessons learned
  1. The business value of devops is even higher than we thought
    - High performers are more agile
    - High performers are more reliable
    - High performers win in the marketplace
  2. Devops is as food for dev, as it is for ops
    - Facebook chat feature - 0 to 98 million overnight
    - Continually tested in production!
    - We need devops to make our work humane!
    - Dev and Ops: We're both engineers
      - Top predictor of IT performance was whether ops version controls all production artifacts
  3. THe need for high-trust management
    - Knight Capital failure - 15 min deployment error caused $440 million trading loss
      - Change control failure solution: put one more level of signing authority to 'fix' it - increasing the distance between person deciding to do the work, vs the person doing the work
      - Testing failure:
        - Do more testing - increases likelihood of disaster happening
      - Deploy more frequently!
  4. Devops is not just for the Unicorns. Devops is for the horses, too.
    - Devops Enterprise Summit
      - SFO - Oct 21-23 2014
      - http://devopsenterprise.io/
- Corrosive downward spiral if left-unchecked


#### 10:25am - Keynote: Trust Me - Kate Matsudaira, Popforms

##### Date
Tuesday September 23, 2014 10:25am - 10:50am 

##### Location
Salon 7-9 (Lower B2)

#### About
No matter where you are in your organization, you want to be trusted by your
boss, your team, and your friends. You want to be trusted to do a good job. You
want to be someone who others can count on when things go wrong (and in
    operations roles, they frequently do). However, building trust isn't always
so straightforward. Sure, you can earn someone's trust over time, but in the
devops world, where you are bridging different disciplines and communication is
key, how can you be sure you come off as trustworthy right away to the many
people who depend on you? This talk will cover some of the science behind why
people trust one another and give you some specific strategies to help you
build trust and level up your career.

##### Notes

- What happened to merit?
- How do you judge performance? Performance is subjective
- How do you get noticed? - The more autonomy = less your manager knows what you're doing (i.e. ambiguity)
- All this leads to trust - Trust is like money
- Are you a good investment? Success is contingent on trust.
- Does your boss trust you? Do you peers trust you? Have you done a good job to earn their trust?

Building Trust

1. Declaration of Independence
  - Contribution
  - Does your work amtter?
  - Schedule a weekly planning session with yourself
  - Where can you fill in the gaps
  - Manage your manager (hehe)
    - Don't use 1-on-1's as 'status' meetings. It is a waste of time.
    - "Do you have any feedback for me"
  - You should send your status in email every week (keep it brief)

2. Police Badge
  - Reputation
  - success doesn't come from hard work, success comes from people
  - Be the model teammate
  - Help others make things happen

3. Oprah
  - Relationship architecture


#### 11:10am - Infrastructure-as-Code with Puppet Enterprise in the Cloud - Evan Scheessele, HP

##### Date
Tuesday September 23, 2014 11:10am - 11:50am

##### Location
Salon 13-15 (Lower B2)

##### About
In this approachable talk, we tell the story of one business’s cloud-journey:
We used Puppet Enterprise as a customer of the OpenStack-based HP Helion Public
Cloud to manage a portfolio of enterprise applications. Our project’s
underlying objective was to foster business agility via
"infrastructure-as-code"—and so these past 12 months, our small team retooled
our organization’s web services operations around Puppet and pervasive
automation.

With Puppet, we adopted end-to-end transformation of our pipelines for
application provisioning on top of HP’s Helion OpenStack cloud platform, and as
a result we benefited from hyper-consistent configuration management running
atop continuous delivery of cloud infrastructure stacks. Results: push-button,
     E2E deployment automation from nothing to running, configured apps.

We will talk about deep integration with PuppetDB, and Puppet roles and
profiles across our portfolio of diverse applications. We've also leveraged
Hiera, extending it with Hiera-HTTP to make a developer portal that allows
product teams self-service control over stacks' data configuration management.

##### Notes

- Business Agility
- Talked a lot about openstack
- Found this talk quite 'enterprisey'
- "Went from 1000 AWS button clicks to 1 (jenkins) button click"


#### 1:30pm - "Sensu and Sensibility" - The Story of a Journey From #monitoringsucks to #monitoringlove - Tomas Doran, Yelp

##### Date
Tuesday September 23, 2014 1:30pm - 2:10pm

##### Location
Salon 7-9 (Lower B2)

##### About
As the Yelp infrastructure and engineering team grew, so did the pain of
managing Nagios. Problems like splitting alerting across multiple teams,
         providing high availability, and managing Nagios systems in multiple
         environments had become pressing. As we grew toward a service-oriented
         architecture and pushed some services out into the cloud, we rapidly
         needed more automated monitoring configuration.

An evolutionary solution wasn’t going to solve all of our problems—we needed to
revolutionize our monitoring. Sensu is built from the ground up to solve many
of our issues and to be easy to extend.

This talk will cover our puppet 'monitoring_check' API (which sets up
    monitoring for our services within puppet), how and why we deploy Sensu and
our custom handlers and escalations, along with how we provide automatic 'self
service' monitoring for dynamic services and deal with the challenges posed by
the more ephemeral nature of cloud architectures.

##### Notes

- How monitoring either helps or hinders dev + ops collaboration

- Started with Nagios
  - Low developer visibility about production
  - hehe "disaster girl"
  - Escalation of issues are hard
  - Ops ignore alerts from services
  - High friction, low trust, low visibility
  - When your "normality' is "everything on fire" - This Is Dysfunctional (i.e. fucked up)

Sensu
  - Designed to be pluggable/extensible
  - Arbitrary check metadata

Sensu Data Flow:
  - sensu client runs checks on each machine
  - pushes results to rabbit
  - clustered clients
  - sensu server (multiple, ha)
  - process check results, invokes handlers
  - writes state to redis
  - read by api
  - all layers behind haproxy
  - Multiple DC sensus to 'monitor' each other

Sensu Handlers
  - JIRA ticket
  - email
  - irc
  - pagerduty
  - awsprune

How do checks get run
  - every machine rus the client
  - client managed by puppet
  - client has a tcp socket you can connect to

Single source of truth
  - DNS is canonical for sensu servers
  - configure things in one place

Automatic Monitoring
  - e.g. cron jobs - check successful recently
  - cron::d

User specified monitoring
  - data lives in the service config
  - next to the code to emit metrics
  - nest to metadata about sla's and lb timeouts
  - developers can push without ops

Cluster checks
  - Assert some % of machines ar ehealthy
  - TO make a JIRA ticket, vs paging


#### 3:10pm - The Seven Habits of Highly Effective Puppet Users - David Danzilio, Constant Contact

##### Date
Tuesday September 23, 2014 3:10pm - 3:50pm

##### Location
Salon 13-15 (Lower B2)

##### About
Puppet is an incredibly powerful tool, and part of that power is its
flexibility. Flexibility often leads to a wide range of ideas on
implementation. I've consulted on countless Puppet implementations, and I've
seen the entire spectrum, ranging from bat-shit insane to picture perfect. But
even the bat-shit insane implementations worked (to a point), and at some
point, what seemed bat-shit to me was picture perfect to the folks running it.
As I got to understand some of the unique implementations, I started to ask
myself: if there's no clear right way to implement Puppet, is there a
particularly effective way?

When trying to answer this question I started by looking at the teams who got
it right, and a pattern quickly emerged. All of these teams had common
behaviors that went far beyond policies and procedures. These behaviors were
broadly understood by team members, nearly universally adhered to, and almost
second nature. These habits led to more stable, maintainable, and well
understood Puppet deployments. In this talk, I'll share with you the behaviors
I saw and discuss how you can turn these seemingly obvious best practices into
habits amongst your team members.

##### Notes

A collection of observations of high performing puppet users

1. Think like a software developer
  - Puppet has fundamentally changed our roles
  - System administration != software development
  - Puppet is easy because it's a DSL (wrong!)
    - we made it easy to write bad code!
  - You can't expect people to be good at something they've never done before
  - Software engineering is a mature discipline
  - Will be particularly important in Puppet 4!

2. Treat puppet like code
  - Stop treating puppet as a bunch of configuration data
  - Version control
  - Documentation
    - Should be just enough documentation for someone else to step in
    - Someone else ~= future-you ;)
  - Refactoring
    - Eliminating complexity
    - Reducing technical debt (code smell)
  - Code Review
    - Collaboration
    - Communication tool
  - Style
    - Style GUide

3. Stop, Drop, and Design
  - DESIGN vs sit down and start writing
  - Software needs to be designed
  - Separation of concerns
    - results in modular code
  - Package, File, Service (first puppet pattern)
  - Roles and Profiles (puppet pattern)
  - Identify Interfaces (puppet pattern)
    - limit your entry points
    - What information does this module need
    - where does it come from
    - where does it need to go
  - Public and private classes
    - public should validate input and pass it onto private classes
    - look at the '[rivate' function in stdlib
  - Data separation
    - Data inside your puppet code is bad
    - Essentially makes it a singleton
    - Virtually guaranteeting your code will need to be rewritten
    - Hiera!
    - params pattern
  - Module data (emerging pattern)
  - Stability
    - Software needs to be behave
    - identify a stable feature set, track them, write them down
    - Use Semantic versioning
    - Simplicity!
  - UNIX philosophy
    - Focus on your module's core functionality
  - Hooks
    - Provide hooks to enable/disable functionality
  - Write modules as if they're going to be open sourced
    - Design with someone else is mind

4. Test all the things
  - Testing has become relatively inexpensive
  - Your infrastructure is too important not to test
  - How
    - puppet-syntax
    - rspec-puppet (unit tests)
    - beaker (integration testing framework)
    - kitchen-ci
    - serverspec
  - Test First (TDD!!)
  - Make your tests count
  - Don't re-write your test code in yet another DSL - focus on testing your interfaces

5. Continuous Integration and Deployment
  - Automated testing
    - Fully automated test suite
  - Unit Tests
    - rspec-puppet
  - Integration Tests
    - integration between classes & modules
  - Acceptance tests
    - make sure your code actually does what it does in real world conditions
  - Test under real world conditions

6. Make nice with Ruby
  - Puppet is ruby!

7. Get Involved
  - Share your knowledge
  - Puppet is rapidly evolving
  - Share your modules


#### 4:20pm - 7 Puppet Horror Stories in 7 Years - Kris Buytaert, Inuits

##### Date
Tuesday September 23, 2014 4:20pm - 5:00pm

##### Location
Salon 7-9 (Lower B2)

##### About
Bad things can happen with any good technology. The way you use it, the way you
abuse it, the way your environment isn't prepared for it. This talk will go
over seven years of horror stories: different cases in which we've lost hours
and hours debugging our infrastructures. Issues include SSL, DNS, and five
others. 

But once we understood what was going on it all seemed trivial. Horror stories
are what build up your experience. We want to share these "aha!" moments with
you so you don't need to spend seven days figuring out identical or similar
problems. Instead, you can focus on building awesome stuff, rather than
fighting trivial problems the world has already solved.

##### Notes

1. Deploying a puppetmaster
  - chicken and eggs
  - hehe "considered renaming the puppetmaster to schrodinger"

2. Honor your parents or your disks will flood
  - filebuckets - see puppet bug 2385

3. Release Management
  - RPM mirroring
    - pulp
    - PRM
    = Yum Repo Server by IS24
  - ensure => latest is not a great option if you don't control all your repositories

4. We are all devs now
  - Inside a fact included on all nodes, 'exit 0 unless condition' :)

5. Software defined Network
  - broken ipsec setup
  - restarting tunnels solved it

6. Three hard things in IT
  - Beware what you collect!

7. _hmm I think I missed one here_


#### 5:10pm - Killer R10K Workflow - Phil Zimmerman, Time Warner Cable

##### Date
Tuesday September 23, 2014 5:10pm - 6:00pm

##### Location
Golden Gate B (B2)

##### About

How do you harness the power of 10,000 killer robots and make them do your
bidding? You are using or thinking about using the awesomeness of r10k. How do
you automate the automator in your workflow? At Time Warner Cable, we have
created a process for doing just that. Focus on writing great modules and don’t
worry about how your changes will get deployed to your puppet master(s)—just
know they will be there. Come learn about a sane Puppet dev and release
automation process.

The following will be covered:
- Overview of Iterative Development Flow Using R10K
- Automated Puppetfile Manipulation
- GitHub Post-Receive Hook (where the magic happens)
- Capistrano Integration
- Release Deployment Workflow (versioning, git, Jenkins and r10k)
- Jenkins Build and Release Process
- Puppet Deployment Process—Ship It!

##### Notes

R10k - tool for deploying onto masters

Single Repos are not a great idea
  - simplify development
  - Easy jenkins flow
  - Puppet code and hiera data together

Early workflow

  - Simple CI job
  - Single release job
  - Single deploy job

Ways this failed
  - Wait for *all* the tests to run on *all* the modules
  - Deploy everything just to get simple changes updated on the masters
  - Deploy everything just to get hiera data updated on the masters

Early pain points
  - Monolithic repo
  long ci cycles
  al or nothing deploys
  upgrading forge modules

R10K helps automate deployments & environments

R10K and puppetfile - match made in heaven

*There was a bunch of handwaving at this point and I stopped taking notes - might be useful to add links to the presentation/Github repo here instead*


## Wednesday September 24, 2014


#### 9:00am - Keynote: Animating the Puppet: Creating a Culture of Puppet Adoption - Dan Spurling, Getty Images

##### Date
Wednesday September 24, 2014 9:00am - 9:35am 

##### Location
Salon 7-9 (Lower B2)

##### About
If you are at PuppetConf, then you probably already believe in the value
proposition of automation and consistency. But how do you transform your entire
team to deliver on the “cloud” promise? Hear how Getty Images is building a
puppetized culture that focuses on improving business applications and not just
supporting the underlying technology.


### 9:40am - Keynote: Decentralize Your Infrastructure - Alan Green, Sony Computer Entertainment America

##### Date
Wednesday September 24, 2014 9:40am - 10:15am

##### Location
Salon 7-9 (Lower B2)

##### About
We keep asking what we think is a valid question, but a misinformed one: how do
we centralize our infrastructure in order to distill the myriad of technologies
we encounter? The real question is: how do we encourage innovation, and
maintain a sense of urgency, while still managing project and budget
constraints?

### 11:10am - Continuous Integration for Infrastructure as Code - Gareth Rushgrove, Puppet Labs

##### Date
Wednesday September 24, 2014 11:10am - 11:50am

##### Location
Salon 7-9 (Lower B2)

##### About
Within the Puppet community we talk a lot about testing modules, with
rspec-puppet or, increasingly, with Beaker, but we don't often discuss what a
complete infrastructure continuous integration pipeline might look like.

Continuous integration is about bringing all the pieces of a system together as
early as possible, to avoid problems with integration later on. That means
looking not only at individual modules, but also at how they work together and
how we can verify their combined behavior.

This talk will cover:

- Building and testing base images using Puppet, Packer, and Serverspec
- Integration testing collections of modules using Vagrant and Cucumber
- Writing assertions against the state of your infrastructure, based
on data in PuppetDB and from API driven infrastructure
- Automatically generating tests based on what Puppet knows about your
infrastructure

We'll also discuss what features Puppet is missing that would make full system
testing easier, and what tools might look like in the future.


### 1:30pm - The DevOps Field Guide to Cognitive Biases (2nd Edition) - Lindsay Holmwood, Bulletproof Networks

##### Date
Wednesday September 24, 2014 1:30pm - 2:10pm

##### Location
Salon 4-6 (Lower B2)

##### About
Cognitive biases can deeply affect our behaviors toward others and our ability
to process information by herding us towards mental shortcuts that are
optimized for timeliness over accuracy, at the expense of rationalizing
irrational behavior.

In the first edition of this talk we looked at cognitive biases in the context
of teamwork—how biases affect our ability to interact with other people and
limit effectiveness of teams that collaboratively solve problems.

In this second edition, we turn our focus to cognitive biases during high
stress situations—outages and incidents.

You know that running drills are important, but what's stopping you from doing
them? What, during a stress-filled outage, convinces you that relationships
between systems exist, when in hindsight it's obvious they don't? What develops
common narratives that lead you to the same contributing factors at every
incident retrospective?

Attendees will leave the talk with an overview of biases they run into during
incidents, how to hack their brains to use these biases to their advantage, and
some tips on how to mitigate the effects of the limitations baked into their
wetware.

More confusion! Less rationality! Bigger cognitive dissonance! All this and
more in the second edition of "The DevOps Field Guide to Cognitive Biases".


### 2:20pm - The Grand Puppet Sub-Systems Tour - Nicholas Fagerlund, Puppet Labs

##### Date
Wednesday September 24, 2014 2:20pm - 3:00pm

##### Location
Golden Gate A (B2)

##### About
Hey, let's talk about the indirector. And the catalog. And maybe the node
terminus? And the configurer!

Most of us treat Puppet like it consists of one or two big systems -- the
puppet master, the agent, the CA. But each of these is built from smaller
systems, which we don't usually think about. This talk will be a high-speed
overview of the way Puppet's major subsystems and models fit together. We'll
discuss how the puppet master compiles a catalog, the nature of the catalog
itself, the type and provider system, where external data can enter the
process, and more.

You won't learn how to use Puppet from this talk! But if you've been using
Puppet for a while and want to understand how all these dozens of pieces fit
together, this is for you.


### 3:10pm - Puppetizing Multitier Architecture - Reid Vandewiele, Puppet Labs

##### Date
Wednesday September 24, 2014 3:10pm - 3:50pm

##### Location
Salon 10-12 (Lower B2)

##### About

Puppet is easy to use and understand for modeling a desired configuration state
within the bounds of a single system. For multitier applications however, or
configuration involving data and content distributed between variable numbers
of systems and tiers, the modeling gets more complex.

This talk will use Puppet Labs Professional Services’ implementation of a
flexible-architecture Puppet Enterprise deployment as a case study to talk
specifically about:

- Minimizing required configuration input for multitier apps
- Using Puppet to model variable size app tiers of expandable and contractible
size
- Art of the Possible and constraints to be aware of when using only pure
Puppet and its eventual consistency configuration model

The intended audience is advanced Puppet users interested in pushing Puppet to
today’s multitier limits. The talk will incorporate specific code examples and
a full working implementation of a Puppetized mulitier app. It will be
accessible to general Puppet practitioners looking for an art-of-the-possible
level understanding.


### 4:20pm - Orchestrated Functional Testing with Puppet-spec and Mspectator - Raphaël Pinson, Camptocamp

##### Date
Wednesday September 24, 2014 4:20pm - 5:00pm

##### Location
Salon 13-15 (Lower B2)

##### About
As Infrastructure as Code gets more widely adopted and more heavily automated,
the need for tests is on the rise. It has now become a common practice to
ship Puppet modules with unit and functional tests. The Puppet-spec and
Mspectator projects aim to validate Puppet catalogs and test your fleet on
the fly, using the serverspec library.


### 5:10pm - Managing the File and Exposing the API - Christopher Webber, Chef Software

##### Date
Wednesday September 24, 2014 5:10pm - 5:50pm

##### Location
Salon 13-15 (Lower B2)

##### About
One of the the most fundamental things we do with Puppet is manage
configuration files. As we build up more complicated modules, we become faced
with some interesting decisions about the APIs we expose in our modules. Does
it make sense to pass in a template as a parameter? How about the path to a
template? In this talk I will cover the various methods for working on files
including augeas, the concat module, templates, and other things like custom
types and providers. Additionally, I will touch on the different ways that
configuration files are handled including single monolithic files and conf.d
type patterns. With all of these elements, we will focus on how we present an
API to the users of our modules. The hope is that we will all be better aware
of how we can make our modules more compose-able for all.

