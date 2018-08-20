### Integration tests

Test can be considered as integration if it has no full control over [unit of work](../terminology.md#unit-of-work) 
they are executed against. This tests often include UI, databases, external API, dependencies on Time and so on.
Designed to ensure that integration of different pieces of software (classes, components, services) works as expected.
Have less logical coverage then unit tests, but are very helpful to ensure product 
[external quality](../terminology.md#external-quality). 
  
### Characteristics
* Have one or more **real** dependencies
* Are inconsistent - can provide different unexpected result depending on integration points state
* Don't have full control over unit of work
* Often slow at executing or require long startup time
* Unlocalized - tests many things at once
* Smaller logic coverage
  
## Doubles
Sometimes in component or system tests points of integrations are replaced with test doubles (mocks or fakes)
It is great to have 2 kinds of test in your warehouse to be able to understand if but emerges from integration or 
local broken logic.  

## External system
There are some point associated with integration with external system:

* Service availability
* Is service provider able to support you by answering questions
* If API connection will be developed easily
* Test version of external system
* Application behaviour when API response is unexpected
* Capacity testing

### In case of test system version
Make sure you don't hit production instance wia adding it to firewall.
Don't run integration test against system you are confident in - it can case a lot of miss failing tests.

You may write integration test that covers literary every possible problem like:
connection errors, timeouts, long responses, malformed responses, 
responses with unnecessary lot amount of data  and so on. 
