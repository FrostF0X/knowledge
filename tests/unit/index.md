# Unit tests

is an automated piece of code that invokes the [unit of work](../terminology.md#unit-of-work) being tested, and 
that checks some assumptions about result.
It is one of the best practises to increase code quality, maintainability, stability of project.

### Requirements to adaptation

Before starting to adapt units programmer should have some set of required skills. Some of that skills are basic
understanding of software architecture, and SOLID patterns which will help to write **testable** code that is essential 
for practice. Without this you will spend a lot of time trying to cover with test some untestable code and probably you
will be disappointed in practice. Or you will accidentally write some integration tests, and gain no understanding 
about process.  

### Practice adaptation

Unit tests is practice that is hard to adopt for software engineer. As described below units can do harm to 
your project so should be tried mainly on katas and pet projects where risk of failure is low and consequences are 
not so sever. However it is hard to understand power of unit tests when they applied to projects with small codebase 
and long release cycle. For small codebases such advantages as: reducing debugging time, documentation, improving 
external quality are not so valuable. So after adopting units it is essential to examine their value on real-world
application.

### Risks
Unit testing is two sided sword and if adopted in wrong way can do enormous harm even to green field projects.
Many projects fail because of unit tests that are hard to change, understand and with low coverage level. Story 
begins when some teams decides to adapt unit testing in some new project without having good mentorship, and all 
majority of team have no great understanding of the topic. Test are implemented poorly and are hard to change, and 
read. In point of time when business logic requires change members face the problem of such low quality tests
that bogs them down and continuously indicate fails. In consequence some test cases are removed or ignored. A lot of 
work is rubbished and team will never desire to repeat such failure and will be disappointed in practice.  

### Advantages

* Quicker feedback loop
* Reduce debugging time
* Simplifies refactoring
* Allow running code far from GUI
* Forces you to fix code problems (when integrated to CI pipeline)
* Describes what production code does (documentation)
* In cooperation with component/integration/end-to-end produces software with significant external quality
* Increases internal code quality
* Also they dramatically increase code quality as described [here](code-quality.md)

However all this advantages emerges only from healthy, and well implemented unit tests.

### Disadvantages

* Increases development time at project start
* Requires great level of team technical competency 
* Requires strong team acceptance and understanding
* Poorly written unit tests only **increase** technical depth


