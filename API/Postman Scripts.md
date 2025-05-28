
> [!The most important]
> const response = pm.response.json();
> 


`console.log('String text');` - shows result in console
`console.clear();` - clears the console

We an use 'let' to declare a variable, like: `let firstName = 'Yaro'` but if we want to change the value of the variable we do not need use let.

**const** means that your variable is constant and wont change.

function name_of_function (paramters){
main block of the function
}


>[!REMINDER]
```
function getRandomNumber(maxValue) {
    let random = Math.random() * maxValue;
    random = Math.floor(random);
    return random;
}
console.log(getRandomNumber(100));

OR

const add = (a,b) => a+b;
console.log(add(55,44));
```

> [!Just A note]
> You use parameters when you **define** a function to specify what kind of data it expects.


> [!One more Reminder]
> ```
> function getRandomEmail(domain){
> 
> emailName = Math.random().toString(36).substring(7);
> 
> return `${emailName}@${domain}`;
>   
> }
> 
> console.log(getRandomEmail('outlook'))
> ```


> [!NOTE]
> 
```
 const announceBreakfast = () => {
 
     console.log('Breakfast done');
 
 };

function makeBreakfast(callbackFunction) {
 
     console.log('Starting to make');
 
     callbackFunction();
      console.log('Serving coffee');
 
 }
 
 makeBreakfast(announceBreakfast);
```

`const response = pm.response.json();` - change js object into json text.
```
let json = JSON.stringify(person);
let personNew = JSON.parse(json);
console.log(personNew.firstName);
```
Object in JS and accessing specific component in that object
![[Pasted image 20241205131857.png]]

To add item to the array use ==.push== command.

**HTTP Status Code Validation**
Check if the response has the expected HTTP status code:
```
pm.test("Status code is 200", function () {
    pm.response.to.have.status(200);
});
```

**Response Body Validation**
**Check if a field exists**
Validate that a specific field is present in the JSON response:
```
pm.test("Response has 'closed' field", function () {
    let response = pm.response.json();
    pm.expect(response).to.have.property('closed');
});
```
Ensure a specific field has the correct value:
```
pm.test("Closed field is false", function () {
    let response = pm.response.json();
    pm.expect(response.closed).to.be.false; // Example for boolean

});

```
Validate that a field is of a certain data type:
```
pm.test("Field 'id' is a number", function () {
    let response = pm.response.json();
    pm.expect(response.id).to.be.a('number');
});
```

Verify that an array field has a certain length:
```
pm.test("Items array length is greater than 5", function () {
    let response = pm.response.json();
    pm.expect(response.items).to.be.an('array').with.length.greaterThan(5);

});
```
**Response Time Validation**
Check that the response is received within a specific time limit:
```
pm.test("Response time is less than 200ms", function () {
    pm.expect(pm.response.responseTime).to.be.below(200);
});
```
**Header Validation**
**Check if a header exists**
Verify that a specific header is present in the response:
```
pm.test("Content-Type header is present", function () {
    pm.response.to.have.header("Content-Type");
});
```
Ensure a header has the expected value:
```
pm.test("Content-Type is application/json", function () {
    pm.expect(pm.response.headers.get("Content-Type")).to.eql("application/json");
});
```
**Environment and Collection Variables**
**Set an environment variable**
Save a value from the response into an environment variable:
```
let response = pm.response.json();
pm.environment.set("userId", response.id);
```
**Set a collection variable**
```
let response = pm.response.json();
pm.collectionVariables.set("token", response.token);
```
**Get a variable**
Access and use an environment or collection variable:
```
let userId = pm.environment.get("userId");
pm.expect(userId).to.not.be.null;
```

**Chai Assertion Library Functions**
Postman uses **Chai.js** for assertions, so you can leverage these common assertions:
**Equality**
Check if two values are equal:
```
pm.expect(response.name).to.eql("John Doe");
```
**Boolean Assertions**
```
pm.expect(response.active).to.be.true;
pm.expect(response.closed).to.be.false;
```
**Includes**
Check if an array or string includes a value:
```
pm.expect(response.items).to.include("apple");
pm.expect(response.message).to.include("success");
```
**Comparison**
pm.expect(response.age).to.be.above(18);
pm.expect(response.price).to.be.below(100);


**Working with Response Data**
**Parsing JSON Response**
Access specific fields from the JSON body:
```
let response = pm.response.json();
console.log(response.name);
pm.expect(response.name).to.eql("John Doe");
```

**Parsing Plain Text Response**
If the response body is plain text, parse it as a string:
```
let response = pm.response.text();
pm.expect(response).to.include("Success");
```

**Loops for Array Validation**
Iterate over an array in the response to validate each item:
```
let response = pm.response.json();

pm.test("Validate all items are active", function () {
    response.items.forEach((item) => {
        pm.expect(item.active).to.be.true;
    });
});
```


**forEach**
```
const fruits = ["apple", "banana", "mango"];
fruits.forEach((fruit) => {
    console.log(fruit);
});
```

**.find**
![[Pasted image 20241205201457.png]]


> [!NOTE] About IF statement
> if (a) {}
> If in if statement in brackets there is an variable it always will by considered truthy
