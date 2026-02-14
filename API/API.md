An **API (Application Programming Interface)** is like a **messenger** that helps two systems (like apps, websites, or software) talk to each other.
So right now in a modern world API is a must. It is a standard of communicating of client and a server. Before API everything was local and connected to the database directly. Since Web developed and web products appeared, API was invented as a needed solution.
RESTful concepts are: **client server separation** - frontend and backend are independent, **Statelessness** - each request has all necessary info server does not need store some data for sessions, **standard HTTP methods**, 


**Simple Explanation**

• Imagine you’re at a restaurant:

• The **menu** is the API—it shows what you can order.

• You (the client) choose something from the menu.

• The **kitchen** (server) cooks the food you ordered.

• The waiter (API) brings your food back to you.

  

Similarly:

• Your app asks the API for data (like a list of products).

• The API gets the data from the server and gives it back to the app.




A REST API is RESTful if it follows these constraints:
### **1. Client–Server Separation**

Frontend and backend are independent.
Client does not know internal implementation.
Server does not care about UI.

### **2. Statelessness**

Each request contains all necessary information.
Server does not rely on stored session state between requests

Example:
Token is sent in every request.
No “memory” of previous calls required


### **3. Resource-Based Design**

Everything is treated as a resource.
Examples:

- /users
    
- /accounts
    
- /transactions

Not:
- /doTransferNow
    
- /getUserBalanceAction
    

Nouns, not verbs.