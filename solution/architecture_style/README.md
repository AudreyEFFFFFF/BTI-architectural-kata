# Architecture Style

## Selected Architecture

We decided to use an event-driven, service-based architecture. Our process for coming to that decision was a 

## Usage Observations

Our first step after reading the requirements documentation was to create a user story diagram. This would help us understand the businesss needs of the system and derive technical needs from them.

<Usage Diagram here>

On observing this diagram, we saw a number of distinct tasks working within a shared environment on shared resources (such as data stores, the LLM, etc.) communicating with eachother by pushing tasks to eachother. This immediately struck us as a good fit for a service-based and event-driven architecture.

That said, we want to check our instincts via a more structured process of examining different architecture patterns.


## Architecture Priorities

We came to a consensus that our top 3 architecture priorities are 
1. Observability
2. Data Integrity
3. Interoperability

With adaptability, testability, and security also being important qualities.

### Observability

One of the priorities for this platform was transparency. Observability into the technical processes was more than a technical requirement – it was a mission requirement. How can we claim transparency as our highest priority if we do not take that priority into every part of our platform design.

That said, observability is a paramount technical need. LLMs are an immature, constantly-evolving technology with obscured inner-workings. We felt it was important from a technical perspective to keep careful watch of our system.

For these reasons, observability was a clear #1 priority.

### Data Integrity

One of this platform's critical functions is data collection and analytics. Thus, Data Integrity is a high priority for the platform.

Additionally, LLMs always carry some risk of distorting data or "hallucinating" data that does not exist. This makes it more important that our own data acts as a reliable source of truth.

### Interoperability

A system requirement is that the platform integrates in a clean and user-friendly way with most popular HR software - our platform is, after all, only useful if it is actually used, and will only be used if it is easy to do so. There are at least a dozen different ones, each having a unique API with which our platform will need to communicate, and new ones can enter the market at any time. Thus, we needed to architect for inter-operability.


### Worksheet

![Characteristics](images/styles_worksheet_1.jpeg)

![Styles](images/styles_worksheet_2.jpeg)

As the results of the priority analysis aligned with our instincts about the best architecture patterns for this task, we felt comfortable moving forward.


