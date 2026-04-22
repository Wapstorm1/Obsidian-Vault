SW testing is away to: access the quality of a product, reduce the risks of a product failure during usage. 
**Dynamic testing** - any type of testing when a tester uses or interacts with functionality of a software. 
**Static testing** - quite opposite, meaning testing software before it is built like requirements, specifications, user stories. To identify uncertanties or wrong requirements before coding and testing. 

**Validation** - are we building a right product?
**Verification** - are we building product correctly?


> [!Debugging] Title
> Is seeking for a cause of defect. 

<p align="center"><strong>Test Process activities</strong></p>

1. Test Planning - plan for a testing the product (complex doc)
2. Test monitoring and control - what happened in the product and the plan. 
3. Test Analysis - analyze requirements, user stories, documentation, design. To identify test scenarios. 
4. Test design - how are we gonna to test the functionalities.
5. Test implementation - do we have test env, tools, devices and so on. If not - prepare them. 
6. Test execution - 
7. Test Completion


<p align="center"><strong>Test Levels</strong></p>

**Unit testing** - performed by devs. Meaning product is divided on units, small independent pieces. And they are tested separately. 

**Integration Testing**: integration of units between each other
* Component testing done by devs
* System integration done by testers

**System Testing (E2E)** - main test level for a tester. Testing of a product fully, to make sure that product is usable, main functionality is working and there are not critical errors. 

**Acceptance Testing (UAT)** - making sure that the product is ready for a targeted users. 
* Alpha testing - inviting users to the company to let them use product under the devs supervision and in designed env. 
* beta Testing - company gives the "test build" or pre-release build to chosen amount of users, and collect their feedback for improving before the release. 


<p align="center"><strong>Testing Types</strong></p>

* Functional testing - pretty obvious
* Non-Functional - all others, depends on a product specifications and needs (Stress, load, perfomance, security, penetration, usability, etc.)
* Black box - so you do action and get a result, how the result was appeared you do not know.
* White box - so you know the internal kitchen of the feature liek DB or API
* Dynamic and Static
* Regression - check the changes and previous functionality works after changes/fixes.
* Smoke testing - checking the new build by simple checks that make sure that the app works in general and not crashes.