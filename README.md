# RestAssured BDD Framework

Due to my company policies, i can't share the real project details here. So created a sample RestAssured BDD framework with Cucumber and TestNG for API automation testing.

## Folder Structure

```
RestAssuredBDDFramework/
├── src/
│   ├── main/java/utils/ConfigReader.java
│   └── test/java/
│       ├── stepdefinitions/UserSteps.java
│       ├── runners/TestRunner.java
│       ├── hooks/Hooks.java
│       ├── endpoints/UserEndpoints.java
│       ├── payloads/UserPayload.java
│       ├── assertions/UserAssertions.java
│       ├── requestSpec/RequestSpecFactory.java
│       └── responseSpec/ResponseSpecFactory.java
│
├── src/resources/features/user.feature
├── pom.xml
├── testng.xml
└── README.md
```

## Tools Used

- Java
- RestAssured
- Cucumber (BDD)
- TestNG
- Maven

## How to Run

1. Import the project as a Maven project in your IDE.
2. Update the `pom.xml` with correct dependencies.
3. Run the tests using `TestRunner` or through `testng.xml`.
4. Cucumber HTML reports will be generated in the `target` folder.

## Purpose of Files

- **ConfigReader**: Reads config properties.
- **UserSteps**: Step definitions using Gherkin.
- **UserEndpoints**: Stores API endpoint paths.
- **UserPayload**: Contains request body POJOs.
- **UserAssertions**: Contains response validations.
- **Hooks**: Handles setup and teardown.
- **Request/ResponseSpecFactory**: Centralized spec builder for API requests/responses.
- **user.feature**: BDD scenarios for user API.
