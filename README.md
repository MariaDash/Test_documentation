# Test_documentation    
## [Testing Web Forms](https://github.com/MariaDash/Testing-web-forms/tree/main)
## Web documentation:
## 1. <a href="https://docs.google.com/spreadsheets/d/1i-XT_SBZujUgM5tyZ_HL-ElV8_Fxj3E10RV9rNS1JP4/edit?usp=drive_link">Test-cases</a>
## 2. <a href="https://docs.google.com/spreadsheets/d/1xVo-V7IS4pBtwQkDM1oXWfUAnqjA2wouOo-2pCHDif0/edit?usp=drive_link">Bug Reports</a>
## Mobile Documentation:
## 1. <a href="https://docs.google.com/spreadsheets/d/1KdNTA0hFw6A5MpJC4s6eHADl7M2IUhNn/edit?usp=sharing&ouid=103971371528254064968&rtpof=true&sd=true">Bug Report</a>
## 2. <a href="https://docs.google.com/spreadsheets/d/1WjB6RFr5Pk_GUD2tnbYydGwPaWzpmXaM/edit?usp=drive_link&ouid=103971371528254064968&rtpof=true&sd=true">Test-case</a>
## 3. <a href="https://docs.google.com/spreadsheets/d/1BVT8OtNYTwFA50-1MKVJTuhFsKiYJ_x5/edit?usp=drive_link&ouid=103971371528254064968&rtpof=true&sd=true">Smoke Check-list</a>
## 4. <a href="https://docs.google.com/spreadsheets/d/1YJkm-fq_NL46XQMU88O-kISBW6wQzw3hyYvd6NdSazs/edit?usp=sharing">Regression Check-list</a>
## 5. <a href="https://docs.google.com/spreadsheets/d/19ZKYW2-6BPo7Xjjx36I8UmrdIdyoLoAnSYCsbhybjdM/edit?usp=sharing">End-to-end Check-list</a>
## 6. <a href="https://docs.google.com/spreadsheets/d/1A1_sfrPJLDW837DM_dZoGsilZgupPuKsjh8K_b2lRq0/edit?usp=sharing">Critical Path Check-list</a>
## 7. <a href="https://docs.google.com/spreadsheets/d/1w5R3sC1zuYE_EIC17DfbwusxE8WHl01xMHJl7ibGlns/edit?usp=sharing">Update Check-list</a>
### The main activities related to End-to-End testing:
+ Studying the requirements for end-to-end testing
+ Test environment setup and hardware/software requirements
+ Description of all processes of the system and its subsystems
+ Description of roles and responsibilities for all systems
+ Methodology and testing standards
+ End-to-end tracking of requirements and development of test cases
+ Input and output data for each system.
### The end-to-end testing framework includes three parts:
+ Creating Custom Functions
+ Conditioning
+ Creation of test cases

## Let's consider each of them in detail.
### 1. Creating Custom Functions
As part of building custom functions, the following steps must be taken:

+ List the functions of the system and their interrelated components;

+ List the inputs, actions, and outputs for each feature or function;

+ Define relationships between functions;

+ Determine if a function is reusable or independent.

For example, consider a scenario where you log into your bank account and transfer money from your account to an account at another bank (third party subsystem):

+ Log in to the banking system.

+ Check the account balance.

+ Transfer a certain amount from your account to another bank account (third-party subsystem).

+ Check current account balance.

+ Exit the application.

### 2. Building Conditions Based on Custom Functions
As part of building conditions, the following actions are performed:
+ Building a set of conditions for each defined custom function;
+ Conditions include sequence, time, and data conditions.
For example, checking additional conditions such as:

Authorization page

+ Invalid username and password
+ Verification with valid username and password
+ Password strength check
+ Checking Error Messages

Remaining amount

+ Check the current balance after 24 hours (If the transfer is sent to another bank)
+ Check the error message if the transfer amount is greater than the current balance.

Create a test script
+ Building a test script for a specific custom function

In our case:

+ Sign in
+ Check your bank account balance
+ Transfer the amount of the bank account balance

### 3. Creating multiple test cases

Create one or more test cases for each specific scenario. Test cases can include each condition as a separate test case.
End-to-End Testing Metrics:
The following are some of the metrics used to evaluate end-to-end testing progress.

Test case preparation status: shows the actual progress of the test case preparation compared to the planned one.

Weekly testing progress. Gives detailed information about the completion of the test for the week in percentage. Failed, Failed, and Passed Tests vs. Tests Scheduled to Run.

Defect Status and Details - Shows the percentage of open and closed defects on a weekly basis. In addition, the distribution of defects by week, depending on the severity and priority.

Environment Availability - Total availability hours / total hours scheduled per day for testing.

End-to-End Testing vs System Testing

|End-to-End testing|System testing|
|:--|:--|
|Checks the software system as well as related subsystems|Verifies only the software system against requirements specifications|
|Checks the entire end-to-end flow of processes|Checks the functionality and functions of the system|
|All interfaces and server systems are considered for testing|Functional and non-functional testing are considered|
|Runs after system testing is complete|Executed after integration testing|
|End-to-end testing involves testing external interfaces, which is difficult to automate. Hence, manual testing is preferable|To test the system, you can perform both manual and automated testing|

End-to-end testing is the process of testing a software system along with its subsystems. The biggest difficulty with this type of testing is that it is necessary to have enough information about the entire system, as well as about interconnected subsystems.
