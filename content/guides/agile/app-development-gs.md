---
title:  "Getting Started with Modern App Development"
linkTitle: "Modern App Development"
topics:
- Agile
tags:
- Agile
team:
- VMware Tanzu Labs Nerds
---

Most developers work on existing applications: products and services that have been built, maintained and updated over long periods of time. Normally, these apps exist as a web of tightly coupled, sparsely documented systems. Over time, large organizations develop layers of manual processes designed to minimize risk and ensure compliance. As a result, software releases are often infrequent, high-ceremony events that require heroism and brute force. This bleak status quo is untenable for businesses that want to compete and win in the digital age. The question you need to answer is simply: “How can I modernize my most important apps so I can get new features to production faster?”

There is hope. Your existing portfolio can be transformed iteratively and in a way that reduces time, cost, and operational inefficiencies, while increasing security, resiliency, and compliance.

### Overview
There are different reasons and many ways to start a modernization journey. These are the two most common rationales:
- Transform a portfolio to gain operational efficiency from containers, automation and resiliency. This involves broad and strategic efforts to migrate, modernize and transform an existing portfolio of apps to cloud-based technologies. Moving quickly to retire heritage assets helps organizations achieve improved time and cost-centric outcomes across an application portfolio. Do you need to do some light refactoring to get apps ready for containers? Do other apps require deeper updates? Do you need to break apart app or data monoliths? Are you thinking of on-premises or a public cloud? Are you moving to Kubernetes and other open-source projects? Whatever your priorities, *we’ve got the expertise to help you realize meaningful business outcomes and we're happy to freely share it with you.*
- Modernize the system, transforming monoliths into microservices for agility. This involves modernizing an existing “system of systems” that’s business critical, expensive to update, technically complex and under active development. *We’ll gladly share our techniques for how we update such critical systems to a modern architecture.* With APIs and microservices, you can quickly push updates to delight users and lower operational costs.

Tanzu Labs has helped hundreds of organizations evaluate, plan, and execute their app and data modernization strategies. We're here to share our approach which defines incremental steps that gradually increase the cloud maturity of existing systems, the automation needed in your software development life cycle (SDLC), and the knowledge of your team. 

There are four elements of a successful application modernization initiative:

  1. **Start small.** Even if your portfolio contains thousands of applications, start with a single business unit and a handful of apps that are valuable to your business.
  1. **Automate everything.** Use test-driven development, continuous integration and continuous deployment to reduce manual process time and software delivery lifecycle cost.
  1. **Learn by doing.** Inform a strategy and build your skills through hands-on work, rapid feedback, measuring results and creating a cookbook of patterns as you go.
  1. **Break things down.** Iterate quickly and continually on “thin slices” of complex systems.
  
### Start small
Focus is critical. First, find a progressive organization and locate a handful of custom apps with business relevance that are in active use. Use surveys and/or workshop techniques to quickly determine the amount of effort required and prioritize based on low technical risk and high business relevance. These applications allow you to maximize time spent understanding and automating processes along the path-to-production cycle. It also affords rapid progress and “quick wins” to celebrate in the early days.

### Automate everything
To start, roughly model the end-to-end path-to-production process as a baseline. Do it for the initial set of “start small” apps in terms of how code moves into production: existing steps, lead and wait time, handoff mechanisms, and organizational dynamics. Initially, this looks like sticky notes organized on a wall in a time sequence. From there, it can be organized into a spreadsheet where cost and time can be easily modeled. Through this process, you’ll define a roadmap of automation and workflow changes to streamline and eliminate bottlenecks. 

📸  
***IMAGE OF PATH TO PROD STEPS*** 

Existing portfolios often have little to no automated test coverage, which contributes to release management pains. Although it’s not feasible to retrofit test coverage across all existing systems, Tanzu Labs recommends all new code be written to include unit and integration tests. All existing code ported to the cloud should include smoke tests for backing services, along with acceptance tests, if feasible. 

Where possible, integrate testing into the Continuous Integration (CI) pipeline so that it becomes a standard part of release management. Push transformed applications to production and start to transition the existing QA function to a more exploratory, functional testing role. Document new testing practices and push to make them standard throughout your organization as the modernization initiative expands.

### Learn by doing
The most successful Tanzu Labs customers have assembled a small team of employees to drive the initiative. This team uses prioritization models to make effective decisions -- through technical, business and organizational lenses. They work on getting apps into production while automating existing release management processes. As work is done, they capture lessons, patterns and techniques in a cookbook to help accelerate future efforts. Successful modernization teams include these roles:

---
| PRODUCT OWNER | UX DESIGNER | ANCHOR | DEVELOPER |
| --------------|--------|------------|
|Owns prioritization, coordination and measurement. Ensures the team stays unblocked from issues and communicates results. |Technical leader who pairs with a product owner on backlog, guides technical practices, and does hands-on technical work.|Architect developers who know the existing app and underpinning stacks. They grow cloud native skills as they do the work. |
---
### Break things down
Many of your existing apps will move to cloud without much effort, while others (where it makes business sense) should be broken down into cloud native architectural components. A smaller number (hopefully) could be described as a “system of systems” that include dozens of deployable artifacts across a network of servers and backends (such as mainframes). These systems may appear to require significant investment, which can be daunting.

Tanzu Labs recommends targeting “thin slices” by identifying short event flows (within the core domain of a logical system) along with the components required to produce those events. Slice by slice, the team translates the domain model into a  new software architecture and working code using microservices, APIs, message queues and so on that will run on cloud, while interoperating with remaining modules where they reside.

Tanzu Labs uses the [SWIFT methodology](https://www.swiftbird.us/), which employs agile and domain-driven design (DDD) principles to iteratively modernize complex systems. This approach allows you to understand, plan and get started on complex modernization in days, not weeks or months. Here’s how we do this:

- Define Objectives and Key Results [OKR](https://en.wikipedia.org/wiki/OKR). Create a backlog of prioritized user stories tied back to OKR.
- [Event Storm](http://ziobrando.blogspot.com/2013/11/introducing-event-storming.html) the system, using language that business and technical people understand.
- Identify the highest potential thin slice of the system to start transforming.
- Conduct a [Boris](https://www.swiftbird.us/boris-exercise) exercise that models the relationships between capabilities ina system.
- In parallel, generate a documented backlog of work for each identified capability in real time.
- Identify tactical patterns, like anti-corruption layers and service choreography.
- Start hands-on experimentation, feedback and iterative progress.

### How to know if you’re succeeding
How do you know what good looks like? We like metrics offered by [DevOps Research and Assessment](https://cloud.google.com/devops/) (DORA).Here are a few signals that show your effort is succeeding:

- Increased deployment frequency: More software releases this quarter than last quarter
- Release management efficiency: Lower lead and process time, fewer steps and hand offs
- Improved operational metrics for transitioned apps: MTTR, MTBF, support tickets, etc.
- Improved security: Faster patching, zero downtime upgrade, etc.
- Efficient infrastructure usage: Higher density compute, auto-scaling and cost reductions

### Go for it!
Waiting to untangle legacy applications that hinder a better customer experience isn’t an option. We hope this guide was useful. More will be coming soon! Feel free to each out to us any time at [tanzu.vmware.com/labs](https://tanzu.vmware.com/labs).

-------------
-------------
-------------
-------------

### What Is App Development?
Most developers work on existing applications: Products and services that have been built, maintained and updated over long periods of time. Normally, these apps exist as a web of tightly coupled, sparsely documented systems. Over time, large organizations develop layers of manual processes designed to minimize risk and ensure compliance. As a result, software releases are often infrequent, high-ceremony events that require heroism and brute force. This bleak status quo is untenable for businesses that want to compete and win in the digital age. The question you need to answer is simply: “How can I modernize my most important apps so I can get new features to production faster?”There is hope. Your existing portfolio can be transformed iteratively and in a way that reduces time, cost, and operational inefficiencies, while increasing security, resiliency, and compliance.

### Before You Begin

There are a few things you need to do before getting started with App Development:

- Step 1

- Step 2

### Using App Development

### What Are the Key Considerations and Decisions to Make?

### What Decisions Should be Deferred?
Ideally decisions should be made when they have to be made rather than prematurely. 

### How can I Start Simple 🌱, and Let the Work Inform the Direction and Architecture?

### How can I Avoid Being Naive About Architecture?

