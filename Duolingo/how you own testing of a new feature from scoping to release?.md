I usually own testing of a new feature from the moment it's scoped to the release.I start from understanding the main idea/purpose of the feature. After that i clarify acceptance criterias and some question with PM and devs.

For example in Stryber when I was working with MVPs mobile features with incomplete requirements, I firstly identified the core functionality. Based on that I decided what needed deep testing - happy paths, critical edge cases. data - and kept light coverage for secondary features. 

During the development, I tested incrementally as builds developed, gave fast feedback to devs. I relied on exploratory testing especially with unclear requirements. 

Before the release I did regression for core functionality, verified fixes, and then gave QA approval. I reported what was covered, what was not, and etc. so the release decision was transparent. 

1. Scoping - understand main idea of the feature + Acceptance criterias
2. Coverage planning - Identify core functionality and decide what to test and how deep
3. Execution - test builds as they develop (incrementally) and give feedback.
4. Release decision - regression, fixes, qa approval

