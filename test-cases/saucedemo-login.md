&#x09;

Test Cases for https://www.saucedemo.com/





|ID|Title|Preconditions|Test data|Steps|Expected result|Actual result|Status|
|-|-|-|-|-|-|-|-|
|TC\_01|Login with valid credentials|User is on the login page<br />Account exists and is not locked|user: standard\_user<br />passwrd: secret\_sauce|1. Open saucedemo.com <br />2. Enter user name as standard\_user<br /> 3. Enter the  password as secret\_sauce<br /> 4. Click Login|User lands on the Products page|User lands on the Products page|Pass|
|TC\_02|Login with Wrong password|User is on the login page<br />Account exists and is not locked|user: standard\_user<br />passwrd: secret\_sauceabc|1. Open saucedemo.com<br />2. Enter user name as standard\_user<br /> 3. Enter the  password as secret\_sauceabc<br /> 4. Click Login|An error message showing <br />Epic sadface: Username and password do not match any user in this service|Epic sadface: Username and password do not match any user in this service|Pass|
|TC\_03|Login with empty password|User is on the login page Account exists and is not locked|user: standard\_user<br />passwrd:|1. Open saucedemo.com<br />2. Enter user name as standard\_user<br /> 3. Enter no  password <br /> 4. Click Login|An error message showing <br />Epic sadface: Password is required|Epic sadface: Password is required|Pass|
|TC\_04|Login with Locked-out user|User is on the login page Account exists and is locked|user:<br />locked\_out\_user<br />passwrd: secret\_sauce|1. Open saucedemo.com<br />2. Enter user name as locked\_out\_user<br /> 3. Enter the  password as secret\_sauce<br /> 4. Click Login|An error message showing <br />Epic sadface: Sorry, this user has been locked out.|Epic sadface: Sorry, this user has been locked out.|Pass|
|TC\_05|Checking if username is Case sensitive|User is on the login page Account exists and is not locked|user: Standard\_user<br />passwrd: secret\_sauce|1. Open saucedemo.com<br />2. Enter user name as Standard\_user<br /> 3. Enter the  password as secret\_sauce<br /> 4. Click Login|An error message showing <br />Epic sadface: Username and password do not match any user in this service|Epic sadface: Username and password do not match any user in this service|Pass|
|TC\_06|Login time for performance\_glitch\_user|User is on the login page Account exists and is not locked|user:<br />performance\_glitch\_user<br />passwrd: secret\_sauce|1. Open saucedemo.com<br />2. Enter user name as performance\_glitch\_user<br /> 3. Enter the  password as secret\_sauce<br /> 4. Click Login|User lands on the Products page with in 4ms|User lands on the Products page but taking longer than usual around 250ms|Fail|
|TC\_07|Empty fields field username|Account exists<br />and User is on the login page|user:<br />password:|1. Open saucedemo.com<br />2. Enter no username<br />3. Click Login|An error message showing <br />Epic sadface: Username is required|Epic sadface: Username is required|Pass|
|TC\_08|Testing landing page visuals|User is on the login page Account exists and is not locked|user:<br />visual\_user<br />passwrd:<br />secret\_sauce|1. Open saucedemo.com<br />2. Enter user name as visual\_user<br /> 3. Enter the  password as secret\_sauce<br /> 4. Click Login|should be same as standard\_user|shopping cart out of alignment|Fail|
|TC\_09|Testing product page|Should be on the Products page|user:<br />problem\_user<br />passwrd:<br />secret\_sauce|add products to cart after first 2 items cant add 3rd and 4th and 6th|should be able to add as many as we need and remove|can't add or remove items|Fail|



