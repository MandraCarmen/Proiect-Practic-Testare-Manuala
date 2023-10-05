# Proiect-Practic-Testare-Manuala
The scope of the final project for ITF Manual Testing Course is to use all gained knowledge throught the course and apply them in pratice, using a live application

application under test: [Demoblaze](https://www.demoblaze.com/index.html#)

API Documentation: link to API documentation if exists or N/A

**The final project will be split into 2 sections: [Testing section]() and [SQL section]()**

Tools used:

**<h1>Functional specifications </h1>**

<h3>For the Sign up section</h3>

-On the sign-up page, I should see input fields for entering my username and password.

- The username field should allow alphanumeric characters and have a minimum and maximum length requirement. Username should only allow the following format: firstname.lastname@domain.com. “FirstName”, “LastName” and “Domain” should contain only alphanumerical characters.

- The password field should have a minimum length requirement and hide the entered characters for security. Password should be between 8 and 16 characters long. It must contain at least one number, one capital letter, one special character. Password should be displayed as encrypted.

- After entering the required information, I should be able to submit the sign-up form.

- If any required field is left empty or contains invalid data, appropriate error messages should be displayed.

- If the entered username or email address is already registered, an error message should indicate that the account already exists.

- Upon successful submission of the sign-up form, I should receive a confirmation message
  

<h3>For the Contact section</h3>

- As a registered user I should be able to contact the store through the contact form

- As a non-registered user I shouldn’t be able to contact the store through the contact form

- The Contact Email field should allow only the following format: firstnamelastname@domain.com

- The Contact Name field should allow only the following format: First Name Last Name

- The Message box should allow only alphanumerical characters (maximum 1000)


**<h1>Testing section </h1>**

**<h2>1.1 Test Planning </h2>**

The Test Plan is designed to describe all details of testing for the X module from the **Demoblaze** application

The plan identifies the items to be tested, the features to be tested, the types of testing to be performed, the personnel responsible for testing, the resources and schedule required to complete testing, and the risks associated with the plan

**1.1.1 Roles assigned to the project and persons allocated**

Carmen Mandra will test: Sign up, Contact 


**1.1.2 Entry criteria defined**
  - smoke test passed (being the most basic type of test, this is a very important entry criteria in the process of testing)
  - testing environment is up and running


**1.1.3 Exit criteria defined**
  - 50% of tests are passed
  - no Critical issues have Open status


**1.1.4 Test scope**
  - **Test in scope:**
    1.	Create account by using Sign up
    2.	Add to cart (product)
    3.	Contact

  - **Test not in scope:**
    - Non-functional testing like stress, performance is beyond scope of this project
    - No QA support for mobile applications developed. Only web applications will be tested
    - Automation testing is beyond scope
    - Home Button
    - Product description
    - About us Button
    - Categories
    - Previous/ Next Buttons
    - Log in
    - Complete order

**1.1.5 Risks detected:**
  - Projects risks:
      - limited experince for the testing team
      - few people to execute the tests and a short amount of time
      - no experince with e-commerce pages
      - working with a third party site for the payments
      - having just one Browser to test on to
      - the requirements are not very detailed and clear
      - limited acces to testing resources
      
  - Product risks:
      - user data (user accounts, open carts) might be impacted with update tests
      - security risks for the completion of the order (personal data, card data)
      - stability risks (crashes, disconnects, etc)
      - IE, Mozilla, Firefox browsers might have performance issues
      - the web page pagination could be impacted when opened on mobile devices
      - stress conditions might impact the web application
      - new browser might not be supported
      - dependence on revision and update of products
      - delivery problems


**1.1.6 Evaluating entry criteria**
The entry criterias defined in the Test Planning phase have been achieved and the test process can continue.

**<h2>1.2 Test Monitoring and Control</h2>**

It will be done by generating periodic reports that reflect the current status of the test.

The report generated at the end of the sprint:
[Test execution report]([https://www.example.com/my%20great%20page](https://itfclasses.atlassian.net/projects/CM?selectedItem=com.thed.zephyr.je__test-metric-project-level))

**<h2>1.3 Test Analysis</h2>**

The testing process will be executed based on the above requirements for the ***Sign up***. The following test conditions were found:

   - On the sign-up page, I should see input fields for entering my username and password.

  - The username field should allow alphanumeric characters and have a minimum and maximum length requirement. Username should only allow the following format: firstname.lastname@domain.com. “FirstName”, “LastName” and “Domain” should contain only alphanumerical characters.

  - The password field should have a minimum length requirement and hide the entered characters for security. Password should be between 8 and 16 characters long. It must contain at least one number, one capital letter, one special character. Password should be displayed as encrypted.

  - After entering the required information, I should be able to submit the sign-up form.

  - If any required field is left empty or contains invalid data, appropriate error messages should be displayed.

  - If the entered username or email address is already registered, an error message should indicate that the account already exists.

  - Upon successful submission of the sign-up form, I should receive a confirmation message

The testing process will be executed based on the above requirements for the ***Contact***. The following test conditions were found:
  - As a registered user I should be able to contact the store through the contact form

  - As a non-registered user I shouldn’t be able to contact the store through the contact form

  - The Contact Email field should allow only the following format: firstnamelastname@domain.com

  - The Contact Name field should allow only the following format: First Name Last Name

  - The Message box should allow only alphanumerical characters (maximum 1000)
    

**<h2>1.4 Test Design</h2>**

Functional test cases were created in Zephyr Squad. Based on the analysis of the specifications, the test design techniques used for generating test cases are:

Test cases: -> enter here test cases or at least the titles

The test cases with steps can be viewed here: [test_cases.pdf]()

**<h2>1.5 Test Implementation</h2>**

The following elements are needed to be ready before the test execution phase begins:

  - enter here what needs to be ready for the test execution to begin
 
**<h2>1.6 Test Execution</h2>**

  - Test cases are executed on the created test Cycle summary(or Test Run): [cycle_summary_execution.pdf]()
  - Bugs have been created based on the failed tests. The complete bug reports can be found here: [created_bugs.pdf]()
    - enter here bug titles

**<h2>1.7 Test Completion</h2>**

  - Exit criteria was evaluated and passed
  - The traceability matrix was generated and can be found here: [Traceability_matrix.csv]()
  - Test execution chart was generated, the final report shows.... -> describe the final report
 -> enter here test execution report/chart
 
 **<h1>2 SQL section</h2>**
