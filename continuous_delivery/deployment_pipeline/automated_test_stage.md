# Automated test stage
It is automated functional tests stage which is more business facing than commit stage and check system basic business 
logic requirements.

Commit tests gives not enough confidence to ensure that system meets it functional requirements, it may event not 
start when all unit tests pass.

#### Best practices
* **Environment should be as close as possible to production**, however some external connection may be changed as test 
doubles or can be scaled down if complete copy of production is expensive.
* **Acceptance tests should be created by cooperation of developers and testers**, if it is false then either 
developers don't feel responsibility and therefore are not bothered by acceptance tests because of that they do not 
pay attention to them fail. Also tests written by testers without collaboration are tightly coupled to UI and 
therefore brittle
* **Developer should be able to run automated tests on their local environment** to be able to test some features in 
isolation and not run whole pipeline to understand test fails, which significantly reduce feedback.
* **Test should be written in business (ubiquitous) language** like **place order** rather than **click order accept 
button** to be more accurate, expressive and independent on UI  
