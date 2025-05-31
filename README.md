Automation_Exercise_Project 🧪
   
A Selenium-based automation testing framework for the Automation Exercise website. This project automates functional testing of key features like user login, using Java, Selenium WebDriver, TestNG, and Maven. It follows the Page Object Model (POM) design pattern for maintainability and scalability, with comprehensive utilities and test data management.

🚀 Features

Page Object Model (POM): Structured with separate page and test classes for maintainability.
Configurable Setup: Browser and URL settings via config.properties.
TestNG Framework: Structured test execution with testng.xml.
Utility Support: Custom utilities for browser management, JSON handling, and more.
Test Data Management: JSON-based test data for dynamic testing.
Maven Build: Simplified dependency management and test execution.

📋 Prerequisites
Before running the project, ensure you have the following installed:

Java 11+: Required for Selenium and TestNG.
Maven 3.9.6+: For dependency management and test execution.
Google Chrome (v136.0.7103.114): Recommended browser (configurable in config.properties).
Windows/WSL/Linux/Mac: Tested on Windows 10/11 and WSL (Ubuntu).

🛠️ Setup Instructions

Clone the Repository:
git clone https://github.com/MohamedElmezayn/Automation_Exercise_Project.git
cd Automation_Exercise_Project


Install Dependencies:

Ensure Maven is installed (mvn --version).
Run:mvn clean install




Configure the Browser:

Open src/test/resources/config.properties and set the desired browser:browser=chrome
url=https://www.automationexercise.com/


Supported browsers: chrome, firefox.


Run Tests:

Execute all tests using TestNG:mvn test


Run a specific test (e.g., TestCase9):mvn test -Dtest=TestCase9





📂 Project Structure
Automation_Exercise_Project/
├── src/
│   ├── test/
│   │   ├── java/
│   │   │   ├── com/
│   │   │       ├── automationexercise/
│   │   │           ├── pages/          # Page Object Models (e.g., LoginPage.java, HomePage.java)
│   │   │           ├── tests/          # Test cases (e.g., TestCase9.java)
│   │   │           ├── utils/          # Utility classes
│   │   │               ├── BrowserManager.java    # Manages browser instances
│   │   │               ├── JSONReader.java        # Reads JSON test data
│   │   │               ├── SeleniumHelper.java    # Selenium utility methods
│   │   │               ├── Util.java              # General utility functions
│   │   │               └── VerifyDownload.java    # Verifies file downloads
│   │   ├── resources/
│   │       ├── testData/                  # Test data in JSON format
│   │       │   ├── AccountDetails.json    # Account-related test data
│   │       │   ├── ExistingUser.json      # Existing user credentials
│   │       │   ├── MadameBrandProducts.json # Product data
│   │       │   ├── PaymentDetails.json    # Payment-related test data
│   │       │   └── PoloBrandProducts.json # Product data
│   │       ├── allure.properties          # Allure report configuration
│   │       ├── config.properties          # Configuration file (browser, URL)
│   │       └── sample.txt                 # Sample file (placeholder)
│   │       └── testng.xml                 # TestNG suite configuration
├── pom.xml                             # Maven configuration
└── README.md                           # Project documentation

🧪 Test Cases
The project includes the following test case (expandable with more):

TestCase9: A sample test case (details to be added based on implementation).

Additional test cases can be developed under src/test/java/com/automationexercise/tests/.
⚙️ Configuration

Browser Setup: Configured via config.properties (e.g., browser=chrome).
Driver Management: Uses WebDriverManager for automatic driver handling.
Test Data: Managed via JSON files in testData/ for dynamic test inputs.
TestNG Suite: Defined in testng.xml for structured test execution.

🛠️ Utilities

BrowserManager.java: Manages browser initialization and cleanup.
JSONReader.java: Reads and parses JSON test data files.
SeleniumHelper.java: Provides reusable Selenium WebDriver methods.
Util.java: General utility functions for test support.
VerifyDownload.java: Verifies successful file downloads during tests.

💡 Future Improvements

Integrate logging (e.g., Log4j) for detailed debugging.
Add Allure or ExtentReports for enhanced test reporting.
Expand test coverage (e.g., registration, checkout).
Add CI/CD integration with GitHub Actions for automated testing.

📞 Contact
For questions or contributions, reach out to Mohamed Elmezayn or open an issue on this repository.

⭐ If you find this project helpful, please give it a star on GitHub!
