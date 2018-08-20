### Best practices
This document covers best practices of writing good unit tests. 
One of cornerstone of good unit tests is rule: Write tests you want to read.
And to understand how to write good unit tests we have to understand what is good unit test:

Properties of good unit test:
* automated and repeatable
* easy to implement
* easy to understand
* relevant in future
* quick
* consistent in its result
* fully isolated
* have full control under [SUT](../terminology.md#sut)
* clarifies problem when it fails

### Unit test frameworks
Unit test frameworks (xUnit) enhance some properties of good unit test like:
* structuring and formalizing test classes
* repeatability
* easiness in implementation and lot of generic matchers
* rich executing UI

### Parametrized tests
Go on with parametrized test when it clarifies and makes tests cases easy to read, understand and maintain.
Avery additional parameter makes tests more generic. Don't go for it because generic things are harder to understand.

### Test granularity
When testing at too large grain:
* there are to much of possibilities and low logic coverage
* such kind of test are very hard to change

When testing at too large fine grain:
* we loose object collaboration errors
* to much coupling to implementation it is hard to understand concept

### Layers
Tests may have declaration and implementation layer:
Declarative tends to be more declarative and implicit, only showing scenario and hiding details under abstraction.
Implementation is implementation of that abstraction.
  
### Interfaces

Don't use mocks to mock concrete classes, if you have desire to mock something then probably we have one of 2 cases:
* It is heavy weight object that is hard to create
* It is object which you have no full control over which is probably belongs to IO or infrastructure layer

To clarify concepts and for better architecture it is better to create interface.

### Bindings

Don't mock third-party code (code that you own) because, it means that your application depends and highly coupled to
code that cannot be changed. Create wrapper around binding and mock it instead. 

### Notes

Don't mock return values with no logic like DTO and entities.
   
  