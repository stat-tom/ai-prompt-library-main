Act as a test automation engineer and create a Selenium + Java automated test that automates and verifies the login process.

<dependencies>
    (JUnit, Selenium, WebDriverManager dependencies shown)
</dependencies>

private static WebDriver driver;
// Use WebDriverManager to download driver binaries and start the browser
// Example test structure:
driver = new ChromeDriver();
@AfterAll
@Test
public void testMessageIsCreated() {
    driver.get("https://automationintesting.online");
}

You are a Java expert. Convert the HTML delimited by triple hashes into a Java Selenium Page Object using PageFactory and @FindBy.
###
<form> ... (contact form inputs for name, email, phone, subject, description, and submit button) ...</form>
###

(Follow-up examples and POJO suggestions)
