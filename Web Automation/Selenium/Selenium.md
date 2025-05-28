* For every browser we need separate driver. Like Google Chrome driver. Browser communicates with driver, transfers all actions.
* Chrome driver: seleninium with the java sends json info to browser driver, browser driver sends it to browser itself, then browser gives the response by HTTP method back to driver
* We need to create an object of the class in the class file
* WebDriver is interface
`driver.close()`- close the browser

```
`driver.close()`- close the browser
----------------------------------------------

//Firefox


System.setProperty("webdriver.gecko.driver", "/Users/rahulshetty/Documents/geckodriver");

WebDriver driver1 = new FirefoxDriver();

//Microsoft Edge

System.setProperty("webdriver.edge.driver", "/Users/rahulshetty/Documents/msedgedriver");

WebDriver driver2 = new EdgeDriver();

driver.get("https://rahulshettyacademy.com");

System.out.println(driver.getTitle());

System.out.println(driver.getCurrentUrl());

driver.close();

//driver.quit();

driver.switchTo().alert().accept()/dismisss(); - accept or dismiss alerts
}
--------------------------------------------------------------------

SELECT FROM A STATIC DROPDOWN

WebElement dropdownElement = driver.findElement(By.id("ctl00_mainContent_DropDownListCurrency"));
Select dropdown = new Select(dropdownElement);
dropdown.selectByVisibleText("USD")
____________________________________________________________________

dropdown.selectByIndex(3); - static dropdown select using index
Thread.sleep(1000); - wait before execution
dropdown.selectByValue(3); - static dropdown select using value
____________________________________________________________________
WebDriver w - new WebDriverWait(drivewr, 5);
w.until(ExpectedConditions.visibilityOfElementLocated) - Explicit wait method, Conditions may be changed
```
- Locators: ID, Xpath, CSS Selector, name, Class Name, Tag Name, Link Text, Partial Link Text
- ![[Pasted image 20241101200035.png]]
- Use // if you want to choose Xpath locator
- Use the :nth-chind(№) to sign uniqu index to the CSS locator
- input[type*='pass'] - dynamic CSS selector
- //button[contains(@class,'submit')] - regular expression
- absolute and relative Xpath? - **Absolute XPath**: Use only if you are sure the HTML structure will remain unchanged or if you have no other choice.
- **Relative XPath**: Preferred for most use cases, especially in dynamic web applications, as it is more flexible and less likely to break with minor HTML structure changes.
- //div[@id='ctl00_mainContent_ddl_originStation1_CTNR'] //a[@value='MAA'] - when you have dynamic drop down and info may change, you use parent child structure to target your locator

> [!NOTE]
> - Check again file base_java


* for ==(Type variable : collection)== - enhanced or for each for loop, s designed to iterate over every element in a collection (like a `List`, `Set`, or array) without using an index.
* To check if checkbox is selected 
  `if (checkbox.isSelected()) { System.out.println("Checkbox is checked."); } else { System.out.println("Checkbox is not checked."); }`
  OR
  `Assert.assertTrue(checkbox.isSelected(), "The checkbox should be checked.");`
- Example how to handle static dropdown 
  `Select s=new Select(d.findElement(By.xpath("//select[@id='exampleFormControlSelect1']")));`
	`s.selectByVisibleText("Female");`

- SSL
  `ChromeOptions options = new ChromeOptions();`
  `options.setAcceptInsecureCerts(true);`
  `WebDriver driver = new ChromeDriver(options);`
![[SSL_CODE.rtf]]

- `SoftAssert a = new SoftAssert();`: This initializes a `SoftAssert` object from the TestNG framework. Soft assertions allow all assertions within the loop to be evaluated and collected, rather than stopping at the first failure.
- `HttpURLConnection conn = (HttpURLConnection)new URL(url).openConnection();`: This creates an HTTP connection to the URL obtained from the `href` attribute.

> [!NOTE] NOTE
> CHeck Test1


**Implicit Wait**
• **What It Does**: Waits for a specified time for all elements to appear before throwing an exception.
• **Scope**: Applies globally to the WebDriver instance.
• **Usage**:`driver.manage().timeouts().implicitlyWait(Duration.ofSeconds(10));`
• ==**Key Point**: Once set, it applies to every findElement() or findElements() call.==

> [!NOTE] Remember
> •**Best Use Case**: At the **start of the script**, after initializing the WebDriver instance.


**Explicit Wait**
• **What It Does**: Waits for a specific condition (e.g., element to be clickable or visible) on a targeted element before proceeding.
• **Scope**: Applied to a specific element or condition.
• **Usage**:`WebDriverWait wait = new WebDriverWait(driver, Duration.ofSeconds(10));`
`WebElement element = wait.until(ExpectedConditions.visibilityOfElementLocated(By.id("elementID")));`
==• **Key Point**: Explicit waits are more flexible and precise.==

> [!NOTE] Remember
> • **Best Use Case**: Immediately before interacting with **specific dynamic elements** that may require extra time to load or appear.


| **Condition**                   | **Purpose**                                                                |
| ------------------------------- | -------------------------------------------------------------------------- |
| visibilityOfElementLocated      | Waits for the element to be visible on the page.                           |
| elementToBeClickable            | Waits for the element to be clickable (visible and enabled).               |
| presenceOfElementLocated        | Waits for the element to be present in the DOM, but it may not be visible. |
| textToBePresentInElementLocated | Waits for specific text to appear in the element.                          |
| invisibilityOfElementLocated    | Waits until the element becomes invisible or is removed from the DOM.      |

> [!PRACTISE]
> https://www.uitestingplayground.com/
