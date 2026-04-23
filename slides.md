---
# You can also start simply with 'default'
theme: the-unnamed
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
# background: https://cover.sli.dev
# some information about your slides (markdown enabled)
title: "It's Not Rocket Science, It's a Flywheel: Engineering OS Communities with DevEx"
info: |
  It's no secret that building and sustaining thriving open source communities requires moving beyond sporadic contributions and fostering an ecosystem of engaged members. That process is not simple, and requires a lot of time and effort, which is not often something a maintainer has, which more often than not leads to maintainer burnout or project stagnation.
  In this talk, Jeremy will connect the principal of a "flywheel" that we see in everyday life with the principles of Developer Experience, and discuss what a "DevEx Flywheel" should look like. He will explore how things like feedback loops, "time to joy", onboarding, and documentation all contribute to an experience that can enhance contributions, which in turn improves project health, value, and more.
  Stop hoping for community growth; start engineering it through Developer Experience.
conference: "LinuxFest NW 2026"
socialimg: /images/bluesky-jerdog-white.png
# https://sli.dev/features/drawing
drawings:
  persist: false
# slide transition: https://sli.dev/guide/animations.html#slide-transitions
defaults:
  layout: center
transition: slide-left
# enable MDC Syntax: https://sli.dev/features/mdc
mdc: true
# open graph
# seoMeta:
#   # By default, Slidev will use ./og-image.png if it exists,
#   # or generate one from the first slide if not found.
#   ogImage: auto
#   # ogImage: https://cover.sli.dev
fonts:
  - sans: News Cycle
  - mono: Fira Code
## Current slide
# apply unocss classes to the current slide
class:
  - text-center
  - my-cool-content-on-the-right
layout: image-right
image: /images/slides/rocket-flywheel.png
backgroundSize: contain
---

# It's Not Rocket Science, It's a Flywheel
## Engineering OS Communities with DevEx

<!--
How many maintainers do we have? What about contributors?
-->

---
layout: image-left
image: /images/slides/xkcd_dependency.png
backgroundSize: contain
class: my-cool-content-on-the-right
---

## The Maintainer's Dilemma

> "I want to grow my open source project/community, but that's going to require a lot of time and effort that I don't have.... So I guess I'll just wait and hope for the best."

<span style="position: fixed; bottom: 0; left: 5%; z-index: 1000; color: blue;">source: [xkcd](https://xkcd.com/2347/)</span>

<!--
We all want thriving open source communities with many engaged contributors. How many have said a variation of this to themselves? This is fine for a time, but what happens when you start getting a lot of new contributions, issues, PRs, and questions? How do you get more help? How do you get more contributors? How do you grow your community? And how do you prevent the inevitable burnout that comes from trying to do it all yourself? Or falls victim to the software supply chain attacks that have become all too common? The latest NPM anyone?

There's always hope, right?
-->

---
layout: image-right
image: /images/slides/ted-lasso-hope-that-kills-you.gif
backgroundSize: cover
---

## Hope is Not a Strategy{style="margin: 50% auto;"}

<!--
Relying solely on hope for community growth is a passive approach that often leads to stagnation, or failure. We can't just hope for a community to grow, especially within Open Source projects where active engagement and contribution are crucial. You have to engineer the conditions for it.
-->

---
layout: two-cols
class: text-center
title: "About Me"
transition: slide-down
---

<span style="position: relative; top: 20%;">

  ## Jeremy Meiss

  <p style="font-weight: bold;">Director, DevEx & DevRel</p>
  <p class="text-sm italic">OneStream Software</p>
  <p style="font-weight: bold;">DevOpsDays KC Organizer</p>

</span>

::right::

![alt text](/images/profile-pic.jpg){style="position: relative; margin: auto; width: 70%; border-radius: 15px 50px; "}

<!--
My name is Jeremy Meiss, and I am the Director of Developer Experience and Developer Relations at OneStream Software. I also help organize DevOpsDays Kansas City.
-->

---
layout: image-left
image: /images/slides/parts-of-flywheel.jpg
backgroundSize: contain
---

## What is a "flywheel?"

<v-click>

> "a mechanical device that uses the conservation of angular momentum to store rotational energy; a form of kinetic energy that is proportional to the product of its moment of inertia and the square of its rotational speed. <br /><br />A flywheel is a heavy wheel attached to a rotating shaft to smooth the transfer of power from an engine to a machine."

-- [The Engineering Choice](https://www.theengineeringchoice.com/what-is-flywheel/)

</v-click>

<!--
Speaking of engineering... Who here knows what a flywheel is, or can give an example of one? [click]A flywheel is a mechanical device specifically designed to efficiently store rotational energy. It is a heavy wheel that requires a significant initial effort to start spinning, but once it gains momentum, it becomes easier to keep it spinning. The energy stored in the flywheel can be released gradually, providing a consistent and reliable source of power.
-->

---

## What is a "flywheel?"
### For the Physicists in the room...

$\frac{1}{2} I  w^{2}$

`w` = angular velocity, `I` = moment of inertia

<!--
The kinetic energy (or more specifically rotational energy) stored by the flywheel's rotor can be calculated by this formula. "w" is the angular velocity, and "I" is the moment of inertia of the flywheel about its axis of symmetry. The moment of inertia is a measure of resistance to torque applied on a spinning object (i.e. the higher the moment of inertia, the slower it will accelerate when a given torque is applied).

I have nothing more on that, I just wanted to be able to tell my mom that at one point in life I gave a talk with math and physics in it.
-->

---

## What is a "flywheel?"
### Metaphorically in Community

> a self-reinforcing loop or cycle that, once set in motion, gains momentum and drives continuous growth and improvement

<!--
In the context of business and community building, the term "flywheel" is used metaphorically to describe a self-reinforcing loop or cycle that, once set in motion, gains momentum and drives continuous growth and improvement.

Let's hold that in mind for a moment and define Developer Experience (DevEx).
-->

---

## Developer Experience (DevEx)

>_"...the **journey** of developers as they learn and deploy technology, which if successful, focuses on eliminating obstacles that hinder a developer or practitioner from achieving success in their endeavors."

-- **Jessica West**, Director of Education & Customer Experience (Chronosphere)

<!--
My friend Jessica West defines Developer Experience (DevEx) as "the journey of developers as they learn and deploy technology, which if successful, focuses on eliminating obstacles that hinder a developer or practitioner from achieving success in their endeavors."
-->

---
layout: image-left
image: "/images/slides/cornell-devex.jpg"
backgroundSize: contain
class: my-cool-content-on-the-right
title: "DevEx isn't new"
---

### DevEx isn't new

_REF: F. Fagerholm and J. Münch, "[Developer experience: Concept and definition](https://ieeexplore.ieee.org/document/6225984?arnumber=6225984)," 2012 International Conference on Software and System Process (ICSSP), Zurich, Switzerland, 2012._

<!--
But DevEx isn't a new thing. The first mention of "developer experience" as a concept was in a paper presented at the June 2012 IEEE International Conference on Software and System Process in Zurich. There are references in the paper going back to 1985 that deal with "programmer performance and the effects of the workplace." A few things stand out in this paper, which is a really great read.
-->

---
layout: image-left
image: /images/slides/cornell-devex.jpg
backgroundSize: contain
class: my-cool-content-on-the-right
title: "DevEx isn't new"
---

### DevEx isn't new

>"New ways of working such as globally distributed development or the integration of self-motivated external developers into software ecosystems will require a better and more comprehensive understanding of developers' feelings, perceptions, motivations and identification with their tasks in their respective project environments."

_REF: F. Fagerholm and J. Münch, "[Developer experience: Concept and definition](https://ieeexplore.ieee.org/document/6225984?arnumber=6225984). 2012."_

<!--
The first is where it talked about these New ways of working where development was globally distributed and integrating self-motivated external developers into software ecosystems and would require a better and more comprehensive understanding of developers' feelings, perceptions, motivations and identification with their tasks in their respective project environments.
-->

---
layout: image-left
image: /images/slides/cornell-devex.jpg
backgroundSize: contain
class: my-cool-content-on-the-right
title: "DevEx isn't new"
---

### DevEx isn't new

>"...developer experience could be defined as a means for capturing how developers think and feel about their activities within their working environments, with the assumption that an improvement of the developer experience has positive impacts on characteristics such as sustained team and project performance."

_REF: F. Fagerholm and J. Münch, "[Developer experience: Concept and definition](https://ieeexplore.ieee.org/document/6225984?arnumber=6225984). 2012."_

<!--
The second was this line, that DevEx could be a means for capturing how devs think and feel about their activities at work, and that improving their experience impacts things like sustained team and project performance.

So all of this interest in DevEx isn't a new concept - but is largely driven by companies trying to sell you something, from the top down, with very little (if any) focus on developers themselves. That doesn't mean there isn't some good value to be had in these frameworks, but we need to be careful about how we use them, and how we think about them.
-->

---
layout: two-cols-header
class: text-center
---

## Developer Experience (DevEx)
### The impacts of the experience

::left::

### Negative

- Time wasted (technical debt, poor tooling, bad docs, etc.)
- Losing developers (attrition, burnout, etc.)
- Lost opportunities (missed deadlines, lost revenue, etc.)

::right::

### Positive

- Frictionless onboarding, workflows, docs
- Clear standards, guardrails
- Fast feedback loops

<!--
A positive DevEx is characterized by frictionless workflows that empower developers, reduce unnecessary cognitive overhead, and allow them to focus on high-value, creative work.
-->

---

## Developer Experience (DevEx)
### Core Dimensions

<v-clicks>

1. Feedback Loops
2. Cognitive Load
3. Flow State

</v-clicks>

<!--
There are 3 core dimensions that you can measure (and improve) in Developer Experience.
[click]**Feedback Loops:** This dimension concerns the speed and quality of the learning cycles that define a developer's workflow. It answers the question: "How quickly do I learn if my change is correct?" Fast, high-quality feedback loops are characterized by rapid build and test times, swift code reviews, and smooth, predictable deployments. Slow or noisy feedback loops, in contrast, kill momentum and create frustration. [click]**Cognitive Load:** This refers to the total amount of mental effort required to perform a task. In software development, cognitive load is increased by factors such as complex architectures, poorly documented code, inconsistent tooling, and ambiguous processes. Reducing unnecessary cognitive load allows developers to dedicate their finite mental energy to solving the core problem at hand, rather than fighting their environment. [click]**Flow State:** Often described as "being in the zone," flow state is a mental state of deep, energized focus and full immersion in a task. It is in this state that developers are at their most productive, creative, and satisfied. Achieving flow state requires long, uninterrupted blocks of time, clear goals, and an environment free from distractions and context-switching.
-->

---

## Developer Experience...
### ...for Open Source projects?

<!--
What makes DevEx different in Open Source projects? The biggest difference is that in OSS, the developers are not your employees. They are volunteers, and they have a choice about where they spend their time and energy. This means that the stakes are higher, and the barriers to entry need to be lower. You need to make it as easy as possible for new contributors to get started, and you need to make it worth their while to stick around.
-->

---

## Back to the flywheel...
### The FlyWheel Effect

![alt text](/images/slides/good-to-great.webp){style="width: 50%; margin: auto;"}

<!--
Jim Collins, in his book "Good to Great," popularized the concept of the "flywheel effect" in business. His research identified that no matter how dramatic the end result, good-to-great transformations never happen in one fell swoop. In building a great company or social sector enterprise, there is no single defining action, no grand program, no one killer innovation, no solitary lucky break, no miracle moment. Rather, the process he described was relentlessly pushing a giant, heavy flywheel, turn upon turn, building momentum until a point of breakthrough, and beyond. The key to the flywheel effect is that it requires consistent, focused effort over time to build momentum. Each small push adds to the overall momentum, and as the flywheel spins faster, it becomes easier to keep it going.
-->

---

## The DevEx Flywheel

![alt text](/images/slides/devex-flywheel.png) {style="width: 40%; margin: auto;"}

<!--
So if we apply the idea of the flywheel to DevEx, we come up with a conceptual model that illustrates how various aspects of the developer experience interact to create a self-reinforcing cycle of community growth and project improvement. By focusing on key components such as feedback loops, onboarding, documentation, and "time to joy," maintainers can engineer a flywheel effect that accelerates contribution and engagement.
-->

---

## The DevEx Flywheel
### Core Components
#### Onboarding & Documentation

- README.md, CONTRIBUTING.md, Code of Conduct ([CNCF Templates](https://contribute.cncf.io/maintainers/templates/))
- Issue templates & PR templates
- Good first issues
- Publish non-code ways to get involved [2012 Andy Lester "14-ways" post](https://web.archive.org/web/20220701201249/https://smartbear.com/blog/14-ways-to-contribute-to-open-source-without-being/)

<!--
This is the first push on the flywheel. Lower the barrier to entry.

- Your README.md is the front door. Does it have a clear "What is this?" and a "How do I run this?" section? Your CONTRIBUTING.md is the welcome mat. It must be clear, concise, and friendly.
- Do you have Issue and PR templates to guide new contributors?
- Do you have a set of "good first issues" that are well-defined and easy to tackle?
- Publish ways to get involved that don't require code: Docs, blogs, testing, answer questions, etc.
-->

---

## The DevEx Flywheel
### Core Components
#### "Time to Joy" & Tooling

- Hello World
- Dev Containers (devcontainer.json)
- Linters & Formatters (Prettier, ESLint, [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/))

<!--
- There's a reason why almost every developer-facing tool has a "Hello World" example. For years, companies like Twilio, Stripe, and others have focused on "Hello World" as a key metric for developer onboarding. We've called this "Time to Joy" among other things. The faster a new contributor can get a simple example running, the more likely they are to stick around. This should be as quick as possible.
- Friction in setup is a joy-killer. Automate your development environment. Things like devcontainers.json helps contributors get a fully configured, one-click development environment in VS Code or GitHub Codespaces.
- Use tooling like linters and formatters to remove style debates from code review, and to keep your codebase consistent.
-->

---

## The DevEx Flywheel
### Core Components
#### Feedback Loops

- First Response (ex. [GitHub Actions](https://github.com/marketplace?query=thank&type=actions))
- Code Reviews
- "Office Hours"

<!--
- A contribution without feedback feels like shouting into the void. Fast, constructive feedback is critical momentum. Automate the first response, like a GitHub Action that thanks a new contributor for their first issue or PR.
- Make code reviews about collaboration, not criticism. Provide clear expectations and guidelines for reviewers and contributors. PR templates can help set the tone from the start.
- While it might be harder with a small project, "office hours" or regular video calls can help build relationships and provide real-time feedback, and can help your project grow.
-->

---

## The DevEx Flywheel
### Core Components
#### Recognition & Value

- Celebrate all contributions ([All-Contributors Bot](https://allcontributors.org/), [GitHub Action](https://github.com/marketplace/actions/contribute-list))
- Publicly thank contributors (release notes, blogs, social)

<!--
This is the push that keeps the flywheel spinning. Contributors work on your project for free. The currency you pay them in is recognition and value.

- Celebrate every contribution, not just code. Documentation, issue triage, and community help are all vital. You can automatically add contributors to your README with tools like the all-contributors bot.
- Publicly thank contributors. Include contributors in release notes, blog posts, and social media shoutouts.
-->

---

## The DevEx Flywheel
### Core Components
#### Leadership Pipeline

- Mentorship programs
- Clear paths to maintainership
- Empower contributors to lead initiatives
- Foster a culture of inclusivity and collaboration

<!--
A thriving community of engaged members becomes the primary source for future leaders. Maintainers can identify and mentor promising contributors into co-maintainer roles, distributing the workload, sharing the emotional labor, and mitigating the risks that are primary drivers of burnout.
-->

---

## The DevEx Flywheel in Action

![alt text](/images/slides/flywheel-spinning.jpg) {style="width: 60%; margin: auto;"}

<!--
Let's put it all together.

- Good Docs -> New contributor arrives, feels confident.
- Great Tooling -> They get set up quickly ("Time to Joy"!).
- Helpful Feedback -> Their first PR is a positive experience.
- Public Recognition -> They feel valued and stick around.
- New Leaders Emerge -> Growing community, less burnout, more sustainability.

Now you have an engaged contributor who helps improve the project and mentor others. The flywheel is spinning. How do you measure that?
-->

---

## Measuring the Spin

<v-clicks>

- How many new contributors and who are they? ([CHAOSS](https://chaoss.community/?p=3613), [OpenSource.com](https://opensource.com/article/17/4/encourage-new-contributors))`
- Contributor Absence Factor: How reliant is a project on a small number of contributors? ([CHAOSS](https://chaoss.community/?p=3944))
- How long until a first response or close? (CHAOSS [First Response](https://chaoss.community/?p=3448), [Time to Close](https://chaoss.community/?p=3446))
- Contributor Activity, Churcn/Retention: Staying for more than one PR?

</v-clicks>

<br />

<v-click>

### Further Reading

- [View the CHAOSS Metrics Catalog](https://chaoss.community/kb-metrics-and-metrics-models/)
- [GitHub Repository Insights](https://docs.github.com/en/repositories/viewing-activity-and-data-for-your-repository)

</v-click>

<!--
You can't improve what you don't measure. CHAOSS Community has a wealth of good metrics you can use to track your project, as well as GitHub's Insights tab.

[click]- How many contributors are making their first contribution to a given project and who are they? Identify first-time contributions across key community interactions, including code commits, issue creation, pull requests, and code reviews. Track new contributors by time period to analyze trends and changes in project engagement.
[click]- The Contributor Absence Factor assesses the degree to which a project relies on a small number of contributors by identifying the smallest number of contributors responsible for 50% of total contributions.
[click]- Measuring how much time passes from when a request (community, issue, PR, etc.) is opened to when it's first responded to and when it's closed can help you identify potential bottlenecks, areas you need more help, etc. This can signal to contributors the level of activity and engagement in a community - with long delays indicating low engagement. , and short delays indicates high participation, etc.
[click]- Contributor Churn/Retention: Are your contributors staying for more than one PR? How long between contributions? Are they becoming regular contributors? Active contributors > # of contributors
[click]For more information, see the CHAOSS Metrics Catalog and GitHub's Repository Insights.
-->

---

## It starts with a single push

1. Follow your own contribution guide. Where do you get stuck?
2. Ask a friend who isn't familiar with the project to try. Compare notes.
3. Pick the single biggest point of friction and fix it this week.

<!--
You don't have to do everything at once. The goal is small, consistent pushes.

- Your first step: Go back to your project and try to follow your own contribution guide. Where do you get stuck?
- Ask a friend who isn't familiar with the project to try.
- Pick the single biggest point of friction and fix it this week. That's your first push on the flywheel.

-->

---

## Conclusion

- Stop hoping for community growth and start engineering it.
- DevEx principles in business can be applied to OSS projects.
- Focus on Onboarding, Tooling, Feedback, and Recognition.
- Small, consistent improvements create powerful, sustainable momentum.

<!--
Stop hoping for community growth and start engineering it.

Use the DevEx Flywheel as your model.

Focus on Onboarding, Tooling, Feedback, and Recognition.

Small, consistent improvements create powerful, sustainable momentum.
-->

---
layout: two-cols
---

<div style="padding-top:200px; align-items: center; justify-content: center; margin: 0 auto; display: flex;">

  <h2>Thank you!</h2>

</div>

::right::

<p><img src="/images/bluesky-logo.svg" style="vertical-align: middle; display: inline; margin: 5px; max-height:50px; padding-right:10px">@jerdog.dev</p>
<p><img src="/images/linkedin.png" style="vertical-align: middle; display: inline; margin: 5px; max-height:50px; padding-right:10px">/in/jeremymeiss</p>
<p><img src="/images/devto.png" style="vertical-align: middle; display: inline; margin: 5px; max-height:50px; padding-right:10px">@jerdog</p>
<p><img src="/images/mastodon.png" style="vertical-align: middle; display: inline; margin: 5px; max-height:50px; padding-right:10px">@jerdog@hachyderm.io</p>
<p><img src="/images/www.png" style="vertical-align: middle; display: inline; margin: 5px; max-height:50px; padding-right:10px">jmeiss.me</p>

<!--

-->

---
layout: end
---