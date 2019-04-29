# Why Microfrontends?

For a lot developed applications, a simple, layered architecture like the Onion Architecture or the [Clean Architecture](https://blog.cleancoder.com/uncle-bob/2012/08/13/the-clean-architecture.html) from Uncle Bob is feasable and maybe  one of the better options available. A small, simple monolith has not a high complexity, is easy to understand and easy to maintain.

{% hint style="info" %}
A monolith is per se not bad, it depends on the need of the project whether to choose a monolith approach or not.
{% endhint %}

## The problematics of a monolith

The monoloth approach will bring in some drawbacks when application systems get more complex in structure, size and distribution of the team and evolution. A monolith can become quite complex to understand. It may start very easy, but it is hard to keep the architectural boundaries over years with changing the develoment team and people ouround it.

### Complexity

Complexity is a hot topic. It has a direct impact on how fast we can produce value and how easy it is to maintain it. A monolith has, by nature, a quite high degree of coupling between its components. When we need to touch a lot of different parts of the application to change something, we have a high coupling and it brings complexity with it.  
Every architect will try to reduce the complexity of his system to a minimum on which it is still possible to implement the requirements. Unfortunately, complexity, will only grow and not shrink over time. Sometime it will exeed the teams capability to react on requirements and changes.

### Scaling

Scaling a monolith up is easy, scaling it out can become more complex, depending of the coupling of its components. Scaling out single components is rather not possible. Larger application systems with multiple developer teams may run into another scaling issue. Puttig more people on a project will not automatically increase the teams productivity. People in the team means coupling on people, code, infrastructure etc. Having them working distributed is even worse. The communication and coordination overhead increases the more people work on this software.

### Evolvability

With evolvability we are talking about the capability of a software system to **adjust its architecture** to fit the needs of requirements in the future. Monolith usually have a higher coupling between its components, which makes it more difficult to adjust its architecture for future needs.

There is a good book called [Building Evoliutionary Architectures](https://www.oreilly.com/library/view/building-evolutionary-architectures/9781491986356/) from Neil Ford, Rebecca Parsons and Partrick Kua is you want to read more about this topic.

## The way out of the monolith

There are several architectures on the road to avoid those drawbacks. It usually starts with the modularization of the monolith to break up the dependencies and lower the complexity. Some go a bit further and introduce a so called [Microkernel Architecture](https://www.oreilly.com/library/view/software-architecture-patterns/9781491971437/ch03.html).

### Service Oriented Architectures

However, this architecture styles still don't solve the problem of scalability and evolvability. To increase scalability the components require to be run in separate processes capable to handle its own network traffic. The way out gets continued by the Service Oriented Architecture. Which is already an improvent in terms of scalability and breaking up the dependencies between teams. Each service can be developed and deployed separately. This enables larger teams to work on the project.

### Microservice Architectures

Services in a service oriented architecture are still quite large in functionality and code. A [microservice architecture](https://microservices.io) breaks this up. Services in a microservice architecture should be small enough to be understood as it whole by every developer in the team. They can be deployed independently, are scalable and so small that throwing away a service does not hurt.

## From UI monolith to microfrontends

We have seen many projects with a service oriented or microservice architecture. In the end they all have a single user interface. We call this a UI monolith. As the name already indicates, a UI monolith brings back the original problematics to our enhanced architecture.

* A UI monolith is limited in scaling.
* It is not maintainable.
* Scaling in teams is difficult.
* It is not independently deployable.
* Its evolvability is limited.

So, how hane we break it up again to gain the full advantage of our chosen architecture?

{% hint style="info" %}
Every component and service should have its own user interface which get composed to the user interface of the system.
{% endhint %}

When the user interface of the application gets composed by small user interfaces, provided of its components or services we are talking about **Microfrontends**.

There are many architectures and paterns helping to get microfrontends. You can find an overview of them in the architecture section.



