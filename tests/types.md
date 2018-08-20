# Types

Basically there are two types of tests from client point of view:

* **Functional**(Business) - tests system business requirements
* **Non-Function**(Technical) - tests system technical quality and everything not related to functional

## Test granularity

* **End To End** - tests whole system in production like environment with some integrations mocked 
* **Integration** - tests how component acts in collaboration with other components 
* **Component** - tests single application component (part) 
* **Unit** - tests single unit of code perhaps Class or Function

## Functional tests
* **Acceptance** - tests system ETE   
* **Exploratory** - manual tests executed by testes which trying to break system in unpredictable ways
* **Usability** - manual tests which check if system is friendly to user

## Non-Functional
* **Unit** - test that ensures system smallest bricks work as expected which significantly improves architecture
* **Integration** - tests application components in collaboration to ensure they fit together
* **Component** - tests single system component in isolation to ensure it nested elements fit together
* **Capacity** - tests maximum load system can handle in production like environment
* **Security** - tests security hole