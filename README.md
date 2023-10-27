# Proiect-Practic-Testare-Manuala
The scope of the final project for ITF Manual Testing Course is to use all gained knowledge throught the course and apply them in pratice, using a live application

Application under test: [Demoblaze](https://www.demoblaze.com/index.html#)

API Documentation: link to API documentation if exists or N/A

**The final project will be split into 2 sections: [Testing section]() and [SQL section]()**

Tools used: Jira and Zephyr Squad

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

The Test Plan is designed to describe all details of testing for the Sign-up and Contact module from the **Demoblaze** application

The plan identifies the items to be tested, the features to be tested, the types of testing to be performed, the personnel responsible for testing, the resources and schedule required to complete testing, and the risks associated with the plan

**1.1.1 Roles assigned to the project and persons allocated**

Carmen Mandra will test: Sign up, Contact 


**1.1.2 Entry criteria defined**
  - access to the testing tools is granted
  - the testing team has undergone the proper training
  - the business specifications have been acknowledged
  - we have a testing environment up and running


**1.1.3 Exit criteria defined**
  - 50% of tests are passed
  - no Critical issues have Open status


**1.1.4 Test scope**
  - **Test in scope:**
    1.	Create account by using the Sign up module. Testing the possibility of creating an account by using a positive and a negative test, verifying that an existing user cannot create a new account
    2.	Send a message to the seller by using the Contact form. Testing to see if the Contact form works as it is intended in the business specifications

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
      - working with a third party site for the payments because the payment site cannot be tested, it might have bugs and it might fail thus impacting our end-to-end functionality of the web site
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
The entry criteria defined in the Test Planning phase have been achieved and the test process can continue.

**<h2>1.2 Test Monitoring and Control</h2>**

It will be done by generating periodic reports that reflect the current status of the test.

The report generated at the end of the sprint:

[Test execution report](https://itfclasses.atlassian.net/projects/CM?selectedItem=com.thed.zephyr.je__test-metric-project-level)

![test execution report](https://github.com/MandraCarmen/Proiect-Practic-Testare-Manuala/assets/133394952/89dc7672-430d-44b5-b04a-dafe8ae5ae36)

![test execution by cycle](https://github.com/MandraCarmen/Proiect-Practic-Testare-Manuala/assets/133394952/61e9a306-062c-46d2-8f60-f414c800cff2)

**<h2>1.3 Test Analysis</h2>**

The testing process will be executed based on the above requirements for the ***Sign up***. The following test conditions were found:

   - Verify that username field accepts alphanumeric characters. Username should only allow the following format: firstname.lastname@domain.com. “FirstName”, “LastName” and “Domain”.

  - The Password should be between 8 and 16 characters long. It should be encrypted.

  - After entering the required information, I should be able to submit the sign-up form.

  - If any required field from the Sign up section (email and password) is left empty or contains invalid data, appropriate error messages should be displayed.

  - Check that an error message is returned when user tries to register with existing username / email

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
  - Verify that an error message is displayed when entering an invalid password in the text input, a too short one
  - Verify that an error message is displayed when entering an invalid password in the text input, a too long one
  - Verify that an error message is returned when the user tries to register with existing username / email
  - Verify that the user cannot create an account by leaving all the input field empty

  - Verify that a non-user cannot send a message
  - Verify that the user cannot send a message by filling out an invalid email account
  - Verify that the user cannot send a message through the contact form if the user leaves all the fields blank
  - Verify that the user can send a message through the contact form by filling out all the blank fields
  - Verify that if the user writes more than 1000 words in the message section an error message is displayed
  - Verify that if the user writes any special characters in the ' message' section an error message is displayed

The test cases with steps can be viewed here: [Zephyr Test Steps (Jira).pdf](https://github.com/MandraCarmen/Proiect-Practic-Testare-Manuala/files/13188078/Zephyr.Test.Steps.Jira.pdf)


**<h2>1.5 Test Implementation</h2>**

The following elements are needed to be ready before the test execution phase begins:

  - The website is up and running
  - All the necesary username, passwords and contact messages examples are ready
  - Acces granted to Jira an Zephyr
    
**<h2>1.6 Test Execution</h2>**

  - Test cases are executed on the created test Cycle summary: [ZFJ - Html Report for Executions.pdf](https://github.com/MandraCarmen/Proiect-Practic-Testare-Manuala/files/13188138/ZFJ.-.Html.Report.for.Executions.pdf)


  - Bugs have been created based on the failed tests. The complete bug reports can be found here: [bug report.pdf](https://github.com/MandraCarmen/Proiect-Practic-Testare-Manuala/files/13188086/bug.report.pdf)

      - [Sign up] Sign up succesfully with invalid email - there was an account created with an invalid password, that did not contain just alphanumeric characters: [[#CM-29] [Sign up] Sign up succesfully with invalid email.pdf](https://github.com/MandraCarmen/Proiect-Practic-Testare-Manuala/files/13188179/CM-29.Sign.up.Sign.up.succesfully.with.invalid.email.pdf)

      - [Sign up] Sign up succesfully with a too long password - an account was created with a password longer than 16 characters: [[#CM-39] [Sign up] Sign up succesfully with a too long password.pdf](https://github.com/MandraCarmen/Proiect-Practic-Testare-Manuala/files/13188190/CM-39.Sign.up.Sign.up.succesfully.with.a.too.long.password.pdf)

      - [Sign up] Sign up succesfully with a too long password, with a too short one - an account was created with a password longer than 8 characters: [[#CM-30] [Sign up] Sign up succesfully with invalid password, a too short one.pdf](https://github.com/MandraCarmen/Proiect-Practic-Testare-Manuala/files/13188198/CM-30.Sign.up.Sign.up.succesfully.with.invalid.password.a.too.short.one.pdf)

      - [Send message through the contact link] Send a message by leaving all the fields empty - the message was succesfully sent even though all the fields were left empty: [[#CM-33] [Send message through the contact link] Send a message by leaving all the fields empty.pdf](https://github.com/MandraCarmen/Proiect-Practic-Testare-Manuala/files/13188214/CM-33.Send.message.through.the.contact.link.Send.a.message.by.leaving.all.the.fields.empty.pdf)

      - [Send message through the contact link] Send a message with more than 1000 alphanumeric characters- the message is successfully sent, even though it contained more that 1000 alphanumeric characters: [[#CM-34] [Send message through the contact link] Send a message with more than 1000 alphanumeric characters.pdf](https://github.com/MandraCarmen/Proiect-Practic-Testare-Manuala/files/13188227/CM-34.Send.message.through.the.contact.link.Send.a.message.with.more.than.1000.alphanumeric.characters.pdf)

      - [Send message through the contact link] Send a message with special characters - the message is successfully sent, even though it contained special characters: [[#CM-35] [Send message through the contact link] Send a message with special characters.pdf](https://github.com/MandraCarmen/Proiect-Practic-Testare-Manuala/files/13188238/CM-35.Send.message.through.the.contact.link.Send.a.message.with.special.characters.pdf)

      - [Send message through the contact link] Message sent by a non-user -  the message is successfully sent, even though the user was not registered: [[#CM-37] [Send message through the contact link] Message sent by a non-user.pdf](https://github.com/MandraCarmen/Proiect-Practic-Testare-Manuala/files/13188255/CM-37.Send.message.through.the.contact.link.Message.sent.by.a.non-user.pdf)

      - [Send message through the contact link] Message sent with an invalid email - the message is successfully sent, even though the email was invalid: [[#CM-36] [Send message through the contact link] Send a message with an invalid email.pdf](https://github.com/MandraCarmen/Proiect-Practic-Testare-Manuala/files/13188268/CM-36.Send.message.through.the.contact.link.Send.a.message.with.an.invalid.email.pdf)

        
**<h2>1.7 Test Completion</h2>**

  - Exit criteria was evaluated and not passed because we have more that 50% of the written test failed.
  - The traceability matrix was generated and can be found here: ![tracebility matrix](https://github.com/MandraCarmen/Proiect-Practic-Testare-Manuala/assets/133394952/e3770092-fa32-470c-b06a-b188956f1985)
  - Test execution chart was generated, the final report shows the presence of 8 bugs from the total of 14 test that were executed, this means that 57,14% from the total number of test failed so the exit criteria is not passed and the bugs need to be fixed and then retested
  - The test execution report can be found here: ![test execution](https://github.com/MandraCarmen/Proiect-Practic-Testare-Manuala/assets/133394952/f6b1c931-b687-4503-bb08-a2bf9530d2f9)
  - All the test were written with regards of the business specifications
  - For the Sign up section there were 8 test written and 3 have failed thus creating 3 bugs. The bugs have a medium priority and that means they do effect the final user because even though an account was created, it was done by using invalid credentials and there problems might occur later on when using the web-site (on log in, on adding to chart, on completing an order, sending a message). They do not affect the applications performance or ability to run
  - For the Contact section there were 6 test written and 5 have failed thus creating 5 bugs. 4 bugs have a low priority, 1 has a medium priority and that means the have a relatively low effect on the user. The performance of the application it is not affected in any way, the only problem might be that the messages can be sent by anyone, even though they are not users, and that can mean there might be a lot of messages coming in.
  - For the next update to the site, I would recommend that the bugs that were found in this cycle are fixed


 
