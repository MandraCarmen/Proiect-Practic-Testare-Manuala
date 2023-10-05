# Proiect-Practic-Testare-Manuala
The scope of the final project for ITF Manual Testing Course is to use all gained knowledge throught the course and apply them in pratice, using a live application

Application under test: [Demoblaze](https://www.demoblaze.com/index.html#)

API Documentation: link to API documentation if exists or N/A

**The final project will be split into 2 sections: [Testing section]() and [SQL section]()**

Tools used:

**<h1>Functional specifications </h1>**

<h3>For the Sign up section</h3>

- On the sign-up page, I should see input fields for entering my username and password.

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

[Test execution report](https://itfclasses.atlassian.net/projects/CM?selectedItem=com.thed.zephyr.je__test-metric-project-level)

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

Functional test cases were created in Zephyr Squad. Based on the analysis of the specifications, the test design techniques used for generating test cases are: Specification-Based and Exploratory Testing

Test cases: 
  - Verify that the user can create an account by filling out all the input fields
  - Verify that the user cannot create an account by filling out only the 'Username' input field and an error message is displayed
  - Verify that an error message is displayed when entering an invalid username in the text input
  - Verify that the user cannot create an account by filling out only the 'Password' input field and an error message is displayed
  - Verify that an error message is displayed when entering an invalid password in the text input
  - Verify that a registered user cannot create another account using the same email address
  - Verify that the user cannot create an account by leaving all the input field empty

  - Verify that a non-user cannot send a message
  - Verify that the user cannot send a message by filling out an invalid email account
  - Verify that the user cannot send a message through the contact form if the user leaves all the fields blank
  - Verify that the user can send a message through the contact form by filling out all the blank fields
  - Verify that if the user writes more than 1000 words in the message section an error message is displayed
  - Verify that if the user writes any special characters in the ' message' section an error message is displayed

The test cases with steps can be viewed here: [Zephyr Test Steps (Jira).pdf](https://github.com/MandraCarmen/Proiect-Practic-Testare-Manuala/files/12818494/Zephyr.Test.Steps.Jira.pdf)

**<h2>1.5 Test Implementation</h2>**

The following elements are needed to be ready before the test execution phase begins:

  - The website is up and running
  - All the necesarry examples are ready
  - Acces granted to Jira an Zephyr
    
**<h2>1.6 Test Execution</h2>**

  - Test cases are executed on the created test Cycle summary: [cycle summary.pdf](https://github.com/MandraCarmen/Proiect-Practic-Testare-Manuala/files/12818577/cycle.summary.pdf)

  - Bugs have been created based on the failed tests. The complete bug reports can be found here: [bug report.pdf](https://github.com/MandraCarmen/Proiect-Practic-Testare-Manuala/files/12818610/bug.report.pdf)
      - [Sign up] Sign up succesfully with invalid email
      - [Sign up] Sign up succesfully with invalid password
      - [Send message through the contact link] Send a message by leaving all the fields empty
      - [Send message through the contact link] Send a message with more than 1000 alphanumeric characters
      - [Send message through the contact link] Send a message with special characters
      - [Send message through the contact link] Message sent by a non-user

**<h2>1.7 Test Completion</h2>**

  - Exit criteria was evaluated and not passed
  - The traceability matrix was generated and can be found here: [traceability matrix.pdf](https://github.com/MandraCarmen/Proiect-Practic-Testare-Manuala/files/12818712/traceability.matrix.pdf)

  - Test execution chart was generated, the final report shows the presence of 7 bugs from the total of 13 test that were executed, this means that 53,85% from the total number of test failed so the exit criteria is not passed and the bugs need to be fixed and then retested
  - The test execution report can be found here: [test execution report.pdf](https://github.com/MandraCarmen/Proiect-Practic-Testare-Manuala/files/12818708/test.execution.report.pdf)

 
 **<h1>2 SQL section</h2>**
