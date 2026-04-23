Application programming interface, which allows two different apps (written with different languages) communicate with each other. Typically in 99% used for a client-server applications. 
This interface give user limited (as an example) a access to the data (or operations with data) on a sever side, without full exposure to the data (in security reasons of course). So that 2 different apps can communicate with each other and without security risks.

<u>Example</u>: You have a Udemy account, and you use it from phone and from laptop. App and website were created with different languages, but they have one backend and you stay synchronized while using 2 devices. That's because of an API which allows 2 different softwares to communicate with the server. 

Cool feature that there are a lot of public API, meaning that anybody can use them, and as they are public, there is no need for security precausions or auth and it means that they are easier to use/implement. 

**POST vs PUT**
POST is used to create a new resource on a backend (like a new user, add new item to the catalog and so on). Meaning endpoint will look like url/movies and inside the body (JSON) there will be a all data that is needed like: title, year, janre, time, actors and so on. When you hit POST couple of times it will create same resource couple of times.
But PUT is used to replace already **existed** resource. And the endpoint is url/movies/id (because we need to identify the resource we will be updating) and hitting PUT multiple times we wont create a new resource, just update existed multiple times by replacing it with a new one. 