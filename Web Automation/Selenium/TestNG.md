To build a framework in TestNG. First of all we create a testNG project, then some classes, in classes we create methods with **@Test**. We can execute all tests from xml file. 
  We can exclude or include needed tests using exclude or include methods.
  If I want to run some tests I can use Name if the method + (.*).

| **Annotation** | **Description**                                                           |
| -------------- | ------------------------------------------------------------------------- |
| @Test          | Marks a method as a test method to be executed by TestNG.                 |
| @BeforeMethod  | Executes before each test method in the current class.                    |
| @AfterMethod   | Executes after each test method in the current class.                     |
| @BeforeClass   | Executes once before the first test method in the current class.          |
| @AfterClass    | Executes once after all test methods in the current class are executed.   |
| @BeforeTest    | Executes before any test method in the <test> tag of the TestNG XML file. |
| @AfterTest     | Executes after all test methods in the <test> tag of the TestNG XML file. |
| @BeforeSuite   | Executes once before all tests in the entire suite.                       |
| @AfterSuite    | Executes once after all tests in the entire suite.                        |
|                |                                                                           |
To Execute specific tests, we need to write mark them like this right under the class name ==@Test(groups=("Name of the group"))== . Groups block goes right after test name in XML file.
```
<groups>
	<run>
		<include name ="group name"/>
	</run>
</groups>
```

`@Test(dependsOnMethods={"example1", "example2"})`is used in **TestNG** to define dependencies between test methods. This means that the test method will only run **after** the specified methods (example1 and example2) have successfully completed.

`@Test(timeOut=4000)` as a Thread.sleep gives a pause of time

Parameter in class we need to pass String and variable in the method
`<parameter name="URL" value="qaclickacademy.com"/>`in XML
```
@Parameters({"URL"})
@Test
public void MobileLogincarLoan(String urlname) {
System.out.println("MobileLogincarLoan");
System.out.println("urlname");
}
```
 **@Test(enabled = false)** - enable attribute can skip the test from execution if put it like false.


> [Important rule]
> When you execute the child class, the methods annotated with @BeforeMethod and @AfterMethod in the parent class are executed because **TestNG supports inheritance of annotations and methods** from parent classes.

Data provider


**ASSERTIONS**
**1. assertTrue(condition)**
• **Usage**: To confirm that something exists, is visible, or meets a condition.
`Assert.assertTrue(driver.getTitle().contains("Dashboard"), "Page title does not contain 'Dashboard'");`

**2. assertFalse(condition)**
• **Usage**: To confirm that something does not exist, is not visible, or does not meet a condition.
`Assert.assertFalse(driver.findElement(By.id("errorMessage")).isDisplayed(), "Error message should not be visible");`

**3. assertEquals(actual, expected)**
• **Usage**: To compare text, numbers, or other values.
`Assert.assertEquals(driver.getTitle(), "Login Page", "Page title mismatch");`

**4. assertNotEquals(actual, expected)**
• **Usage**: To ensure a value is different from the expected one.
`Assert.assertNotEquals(userRole, "Guest", "User role should not be 'Guest'");`

**5. assertNull(object)**
• **Usage**: To confirm that an object is not initialized or does not exist.
`Assert.assertNull(driver.findElement(By.id("nonexistentElement")), "Element should be null");`

**Using @DataProvider**
• The @DataProvider annotation is used to supply multiple sets of data to a test method.
• Ideal for **iterative testing**, where the same test logic needs to be executed for multiple data sets.

![[Снимок экрана 2024-11-22 в 15.34.36 1.png]]

![[Снимок экрана 2024-11-22 в 17.19.39.png]]


**Types of Parameterization in TestNG:**
**Using @Parameters (from XML)**
Test data is passed from the **TestNG XML file** to the test methods.
Useful for providing environment-specific values (e.g., URLs, usernames, or passwords).
You define parameters in the XML file using the `<parameter>` tag.

```
XML
<!DOCTYPE suite SYSTEM "https://testng.org/testng-1.0.dtd">
<suite name="Parameterization Suite">
  <test name="Login Test">
    <parameter name="username" value="testUser" />
    <parameter name="password" value="securePass123" />
    <classes>
      <class name="com.test.LoginTest" />
    </classes>
  </test>
</suite>
```




