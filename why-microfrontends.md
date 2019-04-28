# Why Microfrontends?

For a lot developed applications a simple, layered architecture like the Onion Architecture or the [Clean Architecture](https://blog.cleancoder.com/uncle-bob/2012/08/13/the-clean-architecture.html) from Uncle Bob is feasable and maybe the one of the better options available. A small, simple monolith has not a high complexity, is easy to understand and easy to maintain.

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

With evolvability we are talking about the capability of a software system to **adjust its architecture** to fit the needs of requirements in the future.



