**Definition**: A process of evaluating and verifying that a software application meets the specified requirements.

As a QA engineer, your work will follow a structured process. Here’s a **step-by-step guide** to the key terms and concepts you’ll encounter:

**1. Understanding Requirements**

• **Requirement Gathering**:
• Read and analyze the product requirements (e.g., BRD, FRS) to understand what needs to be built.

• **Key Terms**:

• **[[Acceptance Criteria]]**: Conditions a feature must meet to be accepted.
• **[[User Story]]**: A description of a feature from the user’s perspective (e.g., **“As a user, I want to** log in so I can access my account”).
• **[[Definition of Done]] (DoD)** Ensures user stories are clear, complete, and ready to be worked on.

![[Pasted image 20250113182954.png]]


**2. Test Planning**

• **[[Test Strategy]]**:
• Define the overall testing approach, including what types of tests to perform and when.

• **Key Terms**:
• **[[Test Plan]]**: A document outlining the scope, objectives, resources, and schedule for testing.
• **Scope of Testing**: Defines what features or areas will and won’t be tested.
• **Risk-Based Testing**: Prioritizing testing based on high-risk areas.

> [!Keep in mind]
> Test strategy is about overall test procedures in company, to determine main approach in general (which approaches to use, which frameworks to use etc.)
> On other hand Test Plan is similar but for specific project and more detailed, like home many tests, who is responsible, what are test datas etc.
> 

**3. Test Design**

[[Test design techniques]]
• **Writing [[Test Cases]]**:

• Create detailed steps to validate specific functionalities.

• **Key Terms**:

• **Test Case**: A set of actions to verify a specific feature or function.
• **[[Test Scenario]]**: It is a document which provide description what needs to tested focusing on E2E functionality or from user perspective.
• **[[Boundary Value Analysis]]**: Testing at the edges of input ranges (e.g., min/max values). Typically used for creating [[Edge cases]].
• **[[Equivalence Partitioning]]**: Dividing inputs into valid and invalid groups to reduce redundant tests.

• **Creating Test Data**:
• Prepare data needed for testing (e.g., dummy user accounts, mock transactions).

• **[[Requirement Traceability Matrix]] (RTM)**: In a nutshell it is a table to see if all requirements are covered at least by 1 test case. And to track it's status.


> [!Pay attention]
> • A **test scenario** acts as a parent document for **multiple test cases**.
> 

**4. Test Environment Setup**

• **Environment Configuration**:
• Ensure the application is deployed in a testing environment.

• **Key Terms**:
• **Test Environment**: A replica of the production setup for testing purposes.
• **[[Smoke Testing]]**: A quick test to ensure the build is stable for further testing.
• **[[Sanity Testing]]**: Verifies specific changes or bug fixes.


**5. Test Execution**

**[[STLC]]**


• **Running Tests**:
• Execute test cases and log results.

• **Key Terms**:
• **[[Functional Testing]]**: Validates that the application works as intended. 
• [[Non-Functional Testing]]: Validates 
• **Regression Testing**: Ensures new changes don’t break existing functionality.
• **Exploratory Testing**: Ad-hoc testing to uncover unexpected issues.(typically when there is not enough information, you test by discovering the feature specs in real time)
• **Defect Logging**: Document issues found during testing.
• **Defect Tracking**:
• Log bugs in tools like JIRA and track their resolution.

• **Key Terms**:
• **Bug Report**: A document detailing the defect, steps to reproduce, and severity.
• **Severity**: Impact of the defect (e.g., Critical, High, Low).
• **Priority**: Urgency of fixing the defect.

**6. Test Reporting**

• **Status Updates**:
• Share progress and results with stakeholders.

• **Key Terms**:
• **Test Summary Report**: A document summarizing the testing activities and outcomes.
• **Defect Density**: Number of defects per module or feature.
• **Test Coverage**: Percentage of features or requirements tested.


**7. Test Closure**

• **Wrap-Up**:
• Ensure all objectives are met before ending testing.

• **Key Terms**:
• **[[Exit Criteria]]**: Conditions that must be met before testing can be completed.
• **Retrospective**: A meeting to reflect on the testing process and identify improvements.


**How Do These Fit Together?**

• **Definition of Ready (DoR)** ensures the team has clear and actionable work before starting.

• **Definition of Done (DoD)** ensures that work meets quality standards before it is considered complete.

• **Exit Criteria** ensure testing phases or project milestones meet objectives before progressing.




> [!NOTE]
> **Example for Functional Testing**:
> • **Entry Criteria**: Test plan and test cases are ready, and environment is set up.
> • **Exit Criteria**: 95% of test cases executed, and all major defects are resolved.



**[[Story Points]]**

**[[Agile]]**

**[[Scrum]]**

**[[Validation & Verification]]**
