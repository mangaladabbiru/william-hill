Adding Horse Racing Bet

About Project 
Writing an automated browser-based test on William Hill Australia, online racing
and sports betting website.

Test Scenario
Add a Horse racing bet (any available bet type) to the Bet slip and add a stake
of $10.5. (no need to register/sign-up or login)

Prerequisites
Eclipse
Java
Maven
Cucumber and Selenium dependencies
Chromedriver

Installing
Install Eclipse

Running the tests
Run as JUnit Test by right clicking on the RunnerClass of the project in Eclipse

Break down into end to end tests
  Scenario: To add a horse racing bet to the Bet slip
    Given I navigate to William Hills website
    When I select bet type as racing
    And I select one option 
    And I add a stake of 10.5
    And I select add to bet slip
    And I select Place Bets
    Then I see navigated to Login Page 
    
And coding style tests
The tests test if user is able to add and place Horse racing bet in the William Hills Australia website successfully. This is used to test the functionality of the website.

Project Implementation
The project is built using BDD framework using cucumber. Assertions are made using JUNIT. For implementing design patterns I have declared Global Page Objects in the Page class. There are multiple ways to implement Page Object Pattern, first one is the way I implemented and the other is using @FindBy annotation. This way it will map Page Object properties to fields with matching ids or names.

Built With
BDD and JUNIT - The framework used
Maven - Dependency Management

Authors
Mangala Dabbiru

