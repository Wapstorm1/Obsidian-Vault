Defines conditions a feature must meet to be accepted by the Product Owner or stakeholders.

**Key Features of Acceptance Criteria**

1. **Purpose**:
• Provide clear and measurable definitions of “done” for a specific functionality.
• Ensure that both developers and stakeholders have a shared understanding of requirements.
• Serve as a baseline for writing test cases.

2. **Basis**:
• Derived from business requirements or user stories.
• Typically written in simple, user-focused language.

3. **Scope**:
• Focus on specific functionality, not the overall project or testing scope.


**Example of Acceptance Criteria**

**Scenario: Login Functionality**

• **User Story**: “As a user, I want to log in to my account so that I can access personalized features.”

• **Acceptance Criteria**:
1. Given the user is on the login page, when they enter valid credentials and click “Login,” then they are redirected to the dashboard.
2. Given the user enters incorrect credentials, when they click “Login,” then an error message is displayed.
3. Given the user has forgotten their password, when they click “Forgot Password,” then they are redirected to the password recovery page.



* This is about push-notifications
  **💡 Bonus Checks You Could Add:**
- 🔕 Should push notifications respect **user settings** (e.g., disabled alerts)?
- 🔂 What happens if **multiple messages** arrive — do we batch them?
- 🌐 How should push behave **offline** or **on airplane mode**?