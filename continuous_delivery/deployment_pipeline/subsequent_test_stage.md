# Subsequent test stage
By subsequent test stage we meant 2 right quadrants of test types: 
* Exploratory testing
* Nonfunctional requirements testing 

This two stages may run in parallel because first is dependent on human and second on machine resources.

##### Exploratory testing

For deployment system in terms of manual testing ability to:
* deploy any build to any environment
* see which change from version control system has triggered particular build

**are crucial**
 
##### Nonfunctional requirements testing

Depending on your system requirements capacity, security test may run as automatic part of every pipeline or may be 
executed on demand before some releases. Main idea here is to find best suit for you product, in bank system you 
probably want to execute this tests every time before release, on another hand if you develop web service than you 
don't need this tests on release basis. 
Also capacity testing may not have strict desired values and only give feedback about result depending on which 
business and developers can decide whether to release system or not. 
 
 