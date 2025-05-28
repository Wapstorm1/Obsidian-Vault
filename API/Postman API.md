We use [[Postman]] to test [[API]]. In general testers use it to send some requests to test endpoints. And make sure they work as designed. As I understood for the Udemy corse. We should have some sort of API documentation of the project/product provided by the dev team or somebody else. 

We have:
1. **Endpoints**:
• [[URL]]s that represent resources (e.g., /users to get user data).

2. **HTTP Methods**:
• Actions like [[GET]] (fetch), [[POST]] (create), [[PUT]] (update), [[DELETE]] (remove), **[[PATCH]]**(replace).
![[Pasted image 20241228213955.png]]

3. **Request and Response**:
• A **request** contains the method, headers, body, and parameters.
• A **response** contains the status code, headers, and data (JSON, XML, etc.).

4. **HTTP Status Codes**:
• There are 5 categories of status codes: 
- 100-199 are informational responses
- [[200-299]] are successful responses 
- [[300-399]] are redirection responses 
- [[400-499]] - client error responses
- [[500-599]] - server error responses

5. **Data Formats**:
• APIs often exchange data in JSON or XML format. [[Overall]] [[JSON]] (Lightweight) we use for working with [[REST]], [[XML]] is older and uses for [[SOAP]]. Those are 2 formats of data which APIs use for data exchange. 

6. **Authentication**:

• Some APIs require authentication using:

• **API Keys**

• **Bearer Tokens**

• **OAuth**

7. **Collections**:

• Group related API requests (e.g., all /users endpoints for a user service).

8.  **Environment Variables**:

• Manage settings like baseUrl, authToken for different environments (Dev, Staging, Prod).

9. **Requests**:

• Define API calls with the method, URL, headers, and body.


The difference between **authentication** and **authorization** is:
**Authentication**

• **What it is**: Verifying **who you are**.

• **Purpose**: Ensures the user is legitimate.

• **Example**: Logging in with a username and password.


**Authorization**

• **What it is**: Verifying **what you are allowed to do**.
• **Purpose**: Grants or denies access to resources based on permissions.
• **Example**: A logged-in user is allowed to view their account details but not access admin settings.

**Key Difference**
• **Authentication** comes first (proving identity).
• **Authorization** happens after (assigning permissions based on identity).