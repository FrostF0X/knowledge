### Impact on code quality
This qualities emerge only from **well** written test code

* Clarify object dependencies
* Force context interdependency
* Force to clarify concepts
* Increase code granularity
* Decrease overall complexity
* Reduce code duplication
* Enhance SRP, OCP

### Unit tests as indicators

Unit test is greatest mechanism that can give a lot information about code, there are some cases of negative 
information:

Failing unit test - is great indicator of breaking something, perhaps existing functionality. Most unit test are 
written with purpose to fail sometimes, and that gives us benefit of quick fixing of bugs, and ability to refactor.

Tests that can be written - sometimes we can observe situation when unit test is just can't be written, and the only 
possibility to test this code is integration test. At this point we gain information about system architecture. 
Probably unclarified|unabstracted dependency on uncontrolled parts of the system, broken layering, tangled logic to 
fine grained code.
Remember "Code that is difficult to test is difficult to change"`

#### Smells 
Some typical smells indicated by unit tests:

Lots of code to set up tests may be caused by:
* Bloated constructor
* Awkward class API
* Testing many things at single time

A lot of expectations may be caused by:
* Testing many features at single time
* Unnecessary expectation that do not relates to this feature
* To much work for single feature

Also poorly test naming may indicate that author did not know or bother expected functionality.
