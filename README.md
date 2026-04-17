A Hybrid Test Automation Framework built using Selenium WebDriver + Java + TestNG, designed to demonstrate scalable UI automation practices using a real-world e-commerce application.

This framework follows industry-standard design patterns such as Page Object Model (POM), Data-Driven Testing, and Modular Architecture, making it suitable for both learning and enterprise-level extension.

Key Features : 
  Selenium WebDriver-based UI automation
  Hybrid Framework (POM + Data-Driven + Utilities)
  TestNG for test execution and management
  Externalized test data (Excel / Properties)
  Reusable utility methods
  Configurable environment setup
  Logging & reporting support
  Scalable and maintainable structure

Tech Stack Used

 Language        | Java                                    
 Automation Tool | Selenium WebDriver                      
 Test Framework  | TestNG                                  
 Build Tool      | Maven                                   
 Design Pattern  | Page Object Model (POM)                 
 Data Handling   | Apache POI                              
 Reporting       | Extent Reports
 Logging         | Log4j                                   


Project folder structure
│
├── src/main/java/
│   ├── pageObjects/        # Page classes (POM)
│   ├── testBase/           # Base setup (WebDriver init, config)
│   ├── utilities/          # Reusable utilities (Excel, waits, etc.)
│
├── src/test/java/
│   ├── testCases/          # Test classes
│   ├── testData/           # Test data sources
│
├── src/test/resources/
│   ├── config.properties   # Environment configuration
│   ├── testData files      # Excel / JSON data
│
├── testng.xml              # Test execution suite
├── pom.xml                 # Maven dependencies
├── README.md               # Project documentation


Framework Design

This is a Hybrid Framework, combining:
🔹 Page Object Model (POM)
Each web page is represented as a class
Web elements + actions encapsulated together
Improves maintainability and reusability
🔹 Data-Driven Testing
Test data stored externally (Excel / Properties)
Same test logic runs with multiple datasets
🔹 Utility Layer
Common reusable methods:
Waits
WebDriver utilities
Excel handling
Screenshot capture
🔹 Base Class
Centralized WebDriver setup
Browser initialization
Common setup/teardown logic

Setup Instructions
1. Prerequisites
Java (JDK 8 or above)
Maven
IDE (IntelliJ / Eclipse)
Browser (Chrome / Firefox)


Test Execution Flow : 
TestNG triggers test execution
Base class initializes WebDriver
Page Objects interact with UI
Test data is fetched externally
Assertions validate results
Reports generated after execution

Utilities Included
WebDriver reusable methods
Excel reader utility
Screenshot capture on failure
Wait helpers (implicit/explicit)

