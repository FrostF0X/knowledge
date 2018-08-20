### Interfaces

Is only abstract class without fields and methods implementation.

Some best practices: 
* Define role of the object and is not coupled to particular implementation.
* Create system that will talk to interfaces and don't mind where data comes from, it will clarify decoupling.
* Don't use variables names of implementation even if you know which class is under interface.
* Don't name implementation class with **IMPL** postfix

### Implementation postfix
* every realization has something specific - clarify it
* when interface is designed well - does one thing is is easy to find something specific in implementation
* when naming with this pattern you begin to operate over implementation and interfaces don't means anything to your 
design