**Database Testing** is a type of software testing that focuses on verifying the integrity, consistency, security, and performance of databases used by an application. It ensures that data is stored, retrieved, and managed correctly while meeting the application’s functional and non-functional requirements.

**How to Perform Database Testing**

1. **Understand Requirements**:
• Review application workflows and database structure.
• Identify key database operations and performance criteria.

2. **Prepare Test Environment**:
• Set up the database with sample data for testing.
• Ensure connectivity between the application and database.

3. **Design Test Cases**:
• Write test cases for different database operations, including CRUD operations, validations, and constraints.

4. **Execute Tests**:
• Use tools or manual queries to test database operations.
• Verify results against expected outcomes.

5. **Log and Analyze Results**:
• Document issues like data corruption, query failures, or performance bottlenecks.

**Common Database Testing Scenarios**

1. **Data Validation**:
• Input: Insert a record for a new user.
• Test: Verify the user data is correctly stored and retrievable.

2. **Constraint Validation**:
• Input: Insert a record violating a foreign key constraint.
• Test: Ensure the operation fails and returns an appropriate error.

3. **Transaction Testing**:
• Input: Perform a transaction and force a failure midway.
• Test: Verify the rollback functionality restores the database to its original state.

4. **Performance Testing**:
• Input: Execute a query on a table with millions of records.
• Test: Measure query execution time and resource usage.