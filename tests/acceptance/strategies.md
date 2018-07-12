## Paths

**Happy** path - canonical path through application state.
 
**Alternative** path - in large system path that variates a bit from happy in case of starting/ending point
 
**Sad** path - path that is based on inappropriate start state, end state or actions
 
## Paths Strategy
Write main happy path test that uncovers whole features and serves as basic acceptance criterion and specification.
Depending on what your project looks like write: 
* **alternative** paths when your project is stable (has good unit and component coverage) to uncover other valuable 
to business types of user experience.
* **bad** paths to be more confident in conditions parts.
 
## Given-Then-When

Methodology of describing test scenarios, where:

* **Given** - initial system state
* **When** - actions to be taken in this scenario to achieve next state
* **Then** - required next system state 

## Test throwing out
Delete test suites that fails to often - it reveals that suite is executed against feature that constantly changes.

## Project lifecycle
The easiest time to adopt test its beginning of project, just write every user story as test cases and implement them.

If you are beginning with tests on mature project then it is very important to write test for existing most valuable 
functionality (should be discussed with customers and users), and be covered with **happy path** tests
Then continue to write tests for every new features.