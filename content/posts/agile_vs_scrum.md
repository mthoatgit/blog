---
author: "Hugo Authors"
title: "The dark side of Agile projects"
date: "2023-12-11"
#description: "Sample article showcasing basic Markdown syntax and formatting for HTML elements."
#tags: ["markdown", "css", "html", "themes"]
categories: [ "themes", "syntax" ]
series: [ "Themes Guide" ]
aliases: [ "migrate-from-jekyl" ]
ShowToc: true
TocOpen: true
draft: false
---

# Introduction

After several years in the industry, I've come to the realization that despite growing up with Agile methodologies, I no
longer find enjoyment in Agile projects. While many others share the same experiences, we persist in the belief that an
Agile approach is essential for a successful software project, and so we adhere to Scrum. It's as if we acknowledge its
superiority over traditional methods, but it struggles to resonate with our day-to-day reality. In my view, the issue
lies in the fact that we've formulated a mindset, an equation that's ingrained in our thinking:

* Agile == Scrum

Well, no, this oversimplification is flawed. In essence, Agile is not synonymous with Scrum but Scrum is one way to
embody Agile principles. To draw an analogy:

* mobile != car
* animalistic != dog
* vegetarian != carrot

Scrum represents just **one** approach to Agile software development. An Agile work environment is achievable with or
without Scrum. I'm not one of these Agile shamans that say that success hinges on flawless execution of the Scrum
process. As far as I'm concerned it simply takes more than just giving your middle management a Scrum Master Certificate
to have the benefits of an Agile project. The crucial factor is to remember and apply the lessons we've learned over
decades in software development.

# Waterfall

To see the full picture we have to take a little history lesson to get the context right. The predecessor of
Scrum and the other Agile software development forms is the waterfall process. The very name of this process offers a
clue about its inherent issue. Let me quickly explain its nature. The waterfall process emerged in an era when the needs
of a software project were not clearly understood. In an attempt to formalize the fundamental structure. As a result a
process with six phases was devised:

![Alt text](/blog/waterfall.png)

As previously noted, the issue with the waterfall process is evident in its name. It follows a single, unidirectional
path, making it difficult and costly to backtrack to a previous phase once completed. This led to the development of a
rigid, sequential, and heavily document-driven process. Each phase tended to have extended timeframes, as completion of
one phase was a prerequisite for advancing to the next. Customer involvement was typically confined to the project's
initiation and its conclusion.

# Agile Manifesto

To solve the issue of the waterfall process the [Agile Manifesto](https://Agilemanifesto.org/) was written. It is a
foundational statement of values and principles that underpin Agile software development methodologies.

The main lessons I extracted from the manifest:

* Highest priority is to satisfy the customer through continuous delivery of valuable software.
* Welcome changing requirements, even late in development.
* Deliver working software frequently, with a preference for shorter timescales, ideally in weeks or months.
* Collaboration between customers and developers should occur regular.
* Build projects around motivated individuals and give them the environment and support they need.

Thereafter, Scrum got invented to make these principles suitable for actual software projects. In Scrum, the customer
collaborates closely with the development team to iteratively create value in small, focused development cycles known as
Sprints. The primary goal is to deliver a potentially shippable product increment at the end of each iteration. Regular
feedback from the customer is an integral part of the process, ensuring that the product
aligns with evolving requirements and expectations. You could say the idea of Scrum is to have many little
waterfall processes instead of a big one.

![Alt text](/blog/scrum.png)

While the benefits of the Agile mindset and even Scrum are evident to most people, as it addresses the main issues of
the waterfall process, there is still a considerable amount of frustration persisting in the real world.

# Where does the frustration come from?

As far as I'm concerned, the issue boils down to the tendency for projects to cherry-pick phases of a development cycle
in favor to quick solutions. Let me explain some aspects I encountered in my practice:

### Estimations become deadlines

Agile software development is exceptionally well-suited for projects that start
without precise requirements. The inherent flexibility of Agile methodologies, such as Scrum, allows teams to adapt to
changing needs and fosters collaboration with customers to refine and approach the project's true goals. The iterative
nature of Agile development facilitates continuous improvement, as each iteration provides an opportunity to gather
feedback, adjust priorities, and move closer to delivering a product that aligns closely with the customer's evolving
vision.

The clash between traditional project management and Agile methodologies often arises when estimating costs for the
customer. Many companies, especially those with a budget-driven approach, face challenges in obtaining upfront approval
to commence a project.

### Estimations without requirements

Now the development team can find itself in a unique scenario where the project management insists on using a
traditional approach, demanding estimations based on initially provided requirements that are as vague as the
estimations themselves. It's a familiar situation to hear reassurances like "Don't worry, these estimations will be
refined once we gather more information."

### Estimations collide with Daily Work

The real excitement kicks in as the team delves into the implementation phase,
fully immersed in the sprint mode. The
collaboration with the customer, orchestrated by Scrum, unfolds seamlessly, and the software evolves at a pace that
mirrors the ever-changing requirements. Amidst this dynamic process, there's the lingering challenge of an initial
deadline, seemingly oblivious to the fact that the requirements may have diverged significantly from the project's
outset. The juxtaposition of Agile adaptability with the rigid timeline adds an intriguing layer to the project's
journey.

### Project Management

Trapped in a project with a fixed price but evolving requirements, the project manager is forced
to battle the customer
for seemingly out-of-scope requirements to mitigate scope creep. Often without a choice due the existing situation the
project manager is creating a feature factory for the developers where they are pressed to deliver numerous features
within the constraints of time and budget. This can lead to a situation where not only the developers become demotivated
but also the customer is dissatisfied in the process.

## Feature factory

As already noted estimations are inaccurate by nature. The attempt of estimating the costs for the customer gives a
false sense of security, aiming to secure the project for the company. The consequence is that every task becomes tied
to the time required for its completion. With focus of creating the maximum business value in every iteration the
project transforms into a feature factory.

### Missing prioritization

Instead of focusing on prioritizing stories in the backlog to distill key objectives, there
is an expectation from the
customer that every item in the backlog must be completed. This overlooks the concept that not every written task
necessarily needs execution; some may remain as drafts or plans without the necessity to be carried out.

### Customer is task master
Because the customer not only identifies the problem to be solved but also prescribes the
solution, the defined
requirements often become excessively technical. In this scenario, the implementation process can feel more like
executing tasks as instructed, transforming the development process into a mere execution of predefined steps rather
than delivering a comprehensive solution. The requirements provided by stories resemble a mere catalog of tasks to be
carried out.

### Technical debt
Due to the customer's limited understanding of technical considerations, developers sometimes find it
challenging to
articulate technical requirements and elucidate why tasks that may seem straightforward take longer than anticipated by
the customer. The consequence is that developers often accrue technical debt in favor of quick solutions to meet the
expectations of the customer and the project manager.

### Changing scope and customer requests
If there's a constant influx of customer requests for new features, teams might
feel compelled to keep adding features to meet customer expectations. While customer feedback is crucial, it should be
balanced with a strategic vision for the product.

### Sprints becomes literal
The concept of employing shorter timeframes for implementation, allowing for more iterations, originates from the
intention to facilitate adjustments in the development process. Conversely, a detrimental approach is to interpret and
enforce sprints literally, adding stress to developers with the aim of pushing them harder. This transforms the time
frame for a sprint into the equivalent of a piece rate.

### Missing explicit definition of done (DoD)

A definition of done adds typically test coverage, code reviews and documentation among other things based on the nature
of the project to the actual implementation to mitigate technical debts. The absence of a clear Definition of Done (DoD)
not only ensures the accumulation of technical debt but can also result in estimation discrepancies among developers.
Consequently, this situation gives rise to communication issues within the team, stemming from inconsistent work quality
and unmet customer expectations.

A classic outcome of this scenario is that divergent expectations regarding the completion of a task not only lead to
significantly different time requirements by default but also contribute to additional time needed due to the challenges
by unmaintainable code. Even the "scout principle" becomes hard to follow at some point.

# Conclusion

We delved into the challenges and frustrations encountered in projects claiming to be Agile. One might conclude that the
outlined challenges not only contradict Scrum but also the waterfall model. While the Agile world comes with its own set
of challenges, the solution cannot be to dissect both approaches and attempt to reap the rewards that Agile methods
promise without adhering to their fundamental principles.

