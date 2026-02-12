- Verified CI builds and deployment readiness in Jenkins using logs and runtime checks?
  In Global Payments I used Jenkins to trigger builds with specific configurations, download the generated artifacts, and verify that the correct version was deployed for testing. I also reviewed build logs when something failed to ensure the build completed successfully before starting validation.
  
- Focused manual testing on high-risk areas such as wallet integrations, staking logic, and transaction consistency.
  In 8allocate you had wallets, in the end you had only one. But it means user operations with wallets(connecting, deleting, using it, switch account etc). Stake was about depositing to the pools. 
  
-  Identified critical calculation and reconciliation issues prior to release, preventing user-impacting defects?