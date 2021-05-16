# reimagined-design-patterns

Give a summary description of Four design patterns that you choose from the following design patterns: **Adapter,  Builder, Composite, Decorator, Observer, Interpreter, State, Mediator, Memento, Prototype, Proxy**. In your summaries say:

- what kind of problem(s) you can solve with that pattern and when you use it, maybe with a short example
- how the pattern works, what the basic idea of the pattern is
- what the main advantage and what the the main disadvantage is of using this pattern
- Write a short summary for each of the four patterns, about half a page for each pattern (rather less than more). 

> Do not add diagrams, and do not try to give a complete description of the patterns as found in the books. Rather think of how you would explain the essential ideas of these patterns in a few sentences to a colleague while drinking coffee.

**ADAPTER** 

Summary:

Adapter design pattern is one of the structural design pattern and its used so that two unrelated interfaces can work together by converting the interface of one class into an interface expected by the clients/functions.The object, that joins these unrelated interfaces, is called an Adapter.The adapter can also act as a converter or translator. 

Example :

When a particluar ECU receives information from other ECUs, type conversion(Ex. metres to Kilometre) of the recieved information would be required before processing the information in the received(reason being Standard units of ECU might differ) .This can be done with the help of adapter function.

Advantages :

Helps achieve reusability and flexibility.
Adaptor class can be modified without modifying existing code.
Saves validation time.

Disadvantages :

There is a slight increase in the code size and complexity
Sometimes many adaptations are required along an adapter chain to reach the type which is required.
