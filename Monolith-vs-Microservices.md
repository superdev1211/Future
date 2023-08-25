For a startup with 5 engineers servicing 10 requests per second, I would recommend starting with a monolithic architecture for the core product functionality. Here are a few key reasons why:

- Simplicity and Speed of Development: With a small team, you want to be able to build features and iterate quickly. A monolithic architecture reduces the overhead of managing and deploying many microservices when just getting started.
- Easier Coordination and Testing: With fewer moving parts to coordinate, it's faster for a small team to make changes and thoroughly test the full system. Microservices add complexity in terms of integration testing.
- Avoid Premature Optimization: At 10 requests per second load, a monolith can likely handle the workload fine to start. The complexity of microservices isn't needed yet for scalability.
- Start Simple, Refactor Later: It's easier to break out microservices from a monolith later if needed. Starting with microservices adds unnecessary initial complexity.
- Application Cohesion: The core functionalities likely have high cohesion at the start. This lends itself well to a monolithic app vs. distributed services.

So in summary, the simplicity and development speed of a monolithic start typically outweigh the benefits of microservices for an early-stage startup. As the product and team grow, microservices can be considered to help scale development and the application. But it's best to keep things simple up front.

Here are a few thoughts on choosing a software architecture for a startup with 5 engineers building a product servicing 10 requests per second:
- A monolithic architecture can make a lot of sense for a small team early on. It is simpler to develop and deploy and allows the team to focus on delivering features quickly rather than building infrastructure. Many successful startups like Facebook and Twitter started with monoliths.
- Microservices can provide benefits like independent scalability and using different tech stacks, but come with the overhead of managing many services. For a small team, this can be a distraction. Martin Fowler recommends delaying microservices until you have a more established system and team.
- Serverless/FaaS is compelling for its scalability and low overhead. However, it requires rethinking application design and can have hidden costs around frequent executions. I'd be hesitant to choose it from the start without experience.
- SOA provides loose coupling between components but can be complex to build. It requires more upfront design and infrastructure.
So for a young startup, I would default to a monolith. Focus on building product capabilities, not premature optimization. The team and product requirements are still evolving quickly. Once the system and team scale, you will be better positioned to consider breaking into microservices.

References:

- https://www.myhatchpad.com/insight/monoliths-vs-microservices-whats-best-for-your-startup/
- https://www.n-ix.com/microservices-vs-monolith-which-architecture-best-choice-your-business/
- https://www.couchbase.com/blog/microservices-development-best-practices/
- https://martinfowler.com/articles/microservices.html
