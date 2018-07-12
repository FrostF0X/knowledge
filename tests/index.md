# Automated tests

Software is flexible as customers business, so we frequently change existing functionality, and this changes are 
**unpredictable** to whole service behavior. 
To make this changes **predictable** and **safe** we have to introduce regression testing, 
which cant be done manually for medium/large size project.

## When to automate

If your are executing same test case twice or more and functionality will not change in future it is great occasion 
to think about automation.

Don't automate test to fragile functionality of your application (maybe UI) because there is a high chance of 
deleting this test in future because of failures that it causes.

## When not to automate

Exploratory test - may give you additional information about which tests or even features your system is missing.
Exploratory tests are executed manually by testing with intention to understand if system is suitable for users needs.
Also give feedback about if there are some unpredicted bugs. After gathering this info you can write automated test 
to be sure bug will never occur again. Also by analysing user point of view you can undestand what features are missed.