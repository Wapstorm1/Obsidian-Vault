Functional testing ensures that the application behaves as expected, focusing on verifying individual features and functionalities. Below are additional **functional testing types** you should know:

**Unit Testing**

• Focus: Individual units/components of the software.
• Performed by: Developers.
• Tools: JUnit, NUnit, TestNG.
• Example: Testing a login function to verify it accepts valid credentials and rejects invalid ones.

 **Smoke Testing**
• Focus: Verifies critical functionalities to ensure the build is stable.
• Also known as: “Build Verification Testing.”
• Example: Ensuring basic features like login, navigation, or page load are working after a new deployment.

**Sanity Testing**
• Focus: Checks new or modified functionality to confirm it works as intended.
• Performed after: Receiving a stable build.
• Example: Verifying a newly added search feature works correctly without affecting other modules.

**Regression Testing**
• Focus: Ensures existing features work after changes like bug fixes or new functionalities.
• Tools: Selenium, Cypress.
• Example: After updating the shopping cart functionality, testing all related modules like payment processing.

**Integration Testing**
• Focus: Tests interactions between integrated modules.
• Types:
• **Big Bang Integration**: All modules tested together.
• **Incremental Integration**: Modules tested in stages.
• Example: Ensuring the login module passes the correct user session data to the dashboard module.

**End-to-End Testing**
• Focus: Validates entire workflows, simulating real-world scenarios.
• Example: Testing the user journey of browsing products, adding items to a cart, making payment, and receiving an order confirmation.

**Ad-Hoc Testing**
• Focus: Performed without formal plans; testers try to break the system by using unconventional inputs.
• Example: Entering special characters in a search field to check error handling.

**Exploratory Testing**
• Focus: Simultaneous test case design and execution based on intuition and experience.
• Useful for: Uncovering edge cases and hidden bugs.
• Example: Exploring hidden areas of a web app by manipulating the URL or inspecting developer tools.

**Usability Testing**
• Focus: Ensures the system is user-friendly and intuitive.
• Example: Testing if the navigation menu is easy to use and all options are labeled correctly.

**UI/UX Testing**
• Focus: Tests graphical interface elements like buttons, forms, links, and menus.
• Example: Ensuring the “Submit” button works and redirects to the correct page.

**API Testing**
• Focus: Tests APIs for correctness, performance, and security.
• Tools: Postman, RestAssured.
• Example: Testing the response time and data accuracy of a REST API endpoint for fetching user details.

**Database Testing**
• Focus: Verifies database operations like CRUD (Create, Read, Update, Delete) and schema validation.
• Example: Ensuring user data is correctly stored in the database after registration.