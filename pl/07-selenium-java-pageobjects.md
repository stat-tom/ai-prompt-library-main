Wciel się w rolę automatyzatora testów i utwórz zautomatyzowany test przy użyciu Selenium i Javy, który automatyzuje i weryfikuje proces logowania do aplikacji.

<dependencies>
    <dependency>
        <groupId>org.junit.jupiter</groupId>
        <artifactId>junit-jupiter-engine</artifactId>
        <version>5.9.2</version>
        <scope>test</scope>
    </dependency>
    <dependency>
        <groupId>org.seleniumhq.selenium</groupId>
        <artifactId>selenium-java</artifactId>
        <version>4.9.1</version>
        <scope>test</scope>
    </dependency>
    <dependency>
        <groupId>io.github.bonigarcia</groupId>
        <artifactId>webdrivermanager</artifactId>
        <version>5.5.3</version>
        <scope>test</scope>
    </dependency>
</dependencies>

private static WebDriver driver;
// Use WebDriverManager to download the driver binaries
// and start the browser server for us.
driver = new ChromeDriver();
@AfterAll
@Test
public void testMessageIsCreated() {
    driver.get("https://automationintesting.online");
}

Jesteś ekspertem w programowaniu w Javie. Przekształć kod HTML ograniczony trzema haszami w obiekt strony Java Selenium z użyciem biblioteki PageFactory i adnotacji @FindBy.
###
<Tutaj wprowadź HTML>
###
<form> ... contact form html ...</form>

Follow-up examples for username/password/login and messages list included.
