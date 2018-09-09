### Test practices
To gain real benefits of unit test, developers team must understand how to write clean and maintainable tests.
In this part there are gathered some of main practices and smell related to test implementation.

##### Packaging
Prefer packaging tests classes to separate module and not deploying to production  

##### Naming
Tests class conventionally names with pattern {{ClassName}}Test
Tests methods should describe what feature is tested in specific method. Should be human readable (Your code too ...)
and have sentence structure. Should give first overview of object feature. 
Also there are some conventions like [Given-When-Then](../acceptance/index.md#Given-Then-When) which can clarify some
intentions. Pick suitable convention for your project or use plain sentences.   

Bad naming may be caused by code author ignorance, indolence, or poor domain knowledge.
It may result into maintainability and readability problems.

##### Flow
All test can be created with such flow in mind: **Setup** => **Exec** => **Verify** => **Teardown**
If it is hard to write test like that then it means that code is hard to test and probably it is root of the problems