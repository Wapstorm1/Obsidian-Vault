* QA and QC
* Defect clustering
* **Absence-of-Errors Fallacy** - It says: Just because there are no bugs doesn’t mean the software is **correct or useful**.
* SDLC stages
* After the deployment - - 🔁 **Smoke testing** right after deployment to check if basic flows still work 🧾 **Release note review** — QA helps verify what was actually deployed 🚨 **Set up alerting/log monitoring** if you’re in a DevOps-involved team
* STLC repeat
* Test plan [[attributes]] repeat
* During test env. set up stage also good to mention: ### **Bonus Items to Add (for next level thinking):** - **Environment config files** (e.g., API keys, DB connections, .env settings) **Database seeding** or backups to reset to known state - **Logging & debugging tools** (so issues can be traced)- **User roles setup** (e.g., admin, guest, limited-access users)
* Test closure stage [[activities]] from **STLC**
* A **Decision Table** helps you test **all meaningful combinations** of conditions that lead to different results. 2 в степені n - where n is number of conditions yes/no
* Repeat sanity testing
* Test scenarios - When writing full test cases would take too lon



> [!NOTE] Repeat All Agile stage from tester perspective
> 
> ### **Backlog Refinement (aka Grooming)**



### **What to Check in Requirements (Manually):**

1. **Are they clear and unambiguous?**
    
    → Can I easily tell what should happen — or are there “maybes” and “shoulds”?
    
2. **Are acceptance criteria defined?**
    
    → What does “done” mean for this story?
    
3. **Are edge cases and user roles mentioned?**
    
    → What happens with empty inputs? Invalid data? Different user types?
    
4. **Is anything missing or conflicting?**
    
    → Do these rules match other features? Is the flow broken?
    
5. **Do I see test data or examples?**
    
    → If not, ask for them!


