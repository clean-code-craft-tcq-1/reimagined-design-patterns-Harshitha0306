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

- Helps achieve reusability and flexibility.
- Adaptor class can be modified without modifying existing code.
- Saves validation time.

Disadvantages :

- There is a slight increase in the code size and complexity
- Sometimes many adaptations are required along an adapter chain to reach the type which is required.


**DECORATOR**

Summary :

Decorator pattern allows a user to add new functionality to an existing object without altering its structure. This type of design pattern comes under structural pattern as this pattern acts as a wrapper to existing class.
This pattern creates a decorator class which wraps the original class and provides additional functionality keeping class methods signature intact.

Example :

In vehicle, incase of any error from the System modules , driver can be alerted with a warning signal before bringing the vehicle to safe state. Providing warning signal is a customer specific requirement which can be considered as a Decorator for the existing functionality.

Advantage :

- Ability to add more functionality dynamically without altering existing code.
- User friendly and indepedent.

Disadvantage :

- Usage of multiple decorators can make the maintainability difficult.
- Complex coding.

**STATE**

Summary :

In State pattern a class behavior changes based on its state. This type of design pattern comes under behavior pattern.
In State pattern, we create objects which represent various states and a context object whose behavior varies as its state object changes.
The functionality of the software or system changes based on the change of state.

Example :

ECU engine states for a Drive cycle
1.Pre-Drive
2.Drive
3.Post-Drive

The Software functionality and interfaces execution differ in each drive cycle state, where in _Pre-Drive_ all interfaces are initialised, in _Drive_ the software is executed for calcalulation and in _Post-Drive_ the processed interface values are stored in EEPROM.

Advantage :

-  Easier to add states for additional behavior Reduces conditional complexity.

Disadavantage :

- Large amount of code needed for state machine.

