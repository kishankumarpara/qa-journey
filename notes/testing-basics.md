**Test scenario:** What you want to test, in one line. Example: “Verify the login functionality.”



**Test case:** 

How you test one specific thing, with exact steps and the expected result. One scenario usually has many test cases.



**Field   Example**	

**ID**	TC\_01

**Title**	Login with valid credentials

**Steps**	1. Open the login page. 2. Enter a valid username. 3. Enter the valid password. 4. Click Login.

**Expected result**	User lands on the products page

Other test cases for the same scenario: wrong password, empty username, locked-out user.



**A test plan:** 

The overall document for a project or release. It covers what will be tested and what won’t, the types of testing, tools, who does what, the schedule, the environment, and when testing is considered finished. A tester usually writes test cases daily, while a test plan is written once per project, often by a senior tester or lead.



**Bug life cycle:** 

This is the path a bug follows from discovery to closure. Names vary slightly between companies, but it generally goes:



New: You find a bug and report it with steps, expected vs actual result, and a screenshot.

Assigned: A lead gives it to a developer.

Open / In progress: The developer investigates and works on a fix.

Fixed: The developer says it’s done.

Retest: You test again to confirm it’s really fixed.

Closed: If it’s fixed, the bug is closed.

Reopened: If it still happens, you send it back to the developer. 



**Smoke testing vs regression testing:**



**Smoke testing:** A quick, shallow check right after a new build to see whether the app is stable enough to test further. It covers only the most critical features. Example: Can the app open, can you log in, can you reach the home page? If smoke tests fail, testing stops and the build goes back to developers. Think of it as switching on a new appliance to see whether it smokes.



**regression testing:** A broader check to make sure that new changes haven’t broken things that used to work. Example: A developer changed the checkout page, and you re-test login, cart, and payments to confirm nothing else broke. Regression testing is the main reason companies automate tests, because the same checks are repeated every release.



**Severity vs priority:**



These sound similar but answer different questions.



Severity: How badly the bug affects the system. This is technical, and usually the tester decides it.



Priority: How soon it should be fixed. This is a business decision, often made by the product owner or lead.







&#x09;

