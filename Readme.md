# Task 1:

## Bugs table

#### a. Find bugs as many as you can , write it down in form smth. like this. (Required 5)

| Id    | Description                                                                                                    | Step for reproduce                                                                                                                                                                                                                                                                                                              | Severity | Priority | Image                                                                                               |
|-------|----------------------------------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------|----------|-----------------------------------------------------------------------------------------------------|
| 1     | Checking for entering a negative number in the field for the deposit                                           | 1. Open page [Link](https://www.globalsqa.com/angularJs-protractor/BankingProject/#/login)<br/>2. Customer login<br/> 3. Select Harry Potter and click login<br/> 4. Click Deposit and write down negative amount<br/> 5. An error should be displayed stating that you cannot enter negative amount after click Deposit button | Major    | Medium   | ![img_6.png](photos/img_6.png)                                                                      |
| 2     | Checking for entering different special characters in the fields for the first name, last name and postal code | 1. Open page [Link](https://www.globalsqa.com/angularJs-protractor/BankingProject/#/login)<br/>2. Bank manager login<br/> 3. Click button Add Customer<br/> 4. Enter in field different special symbols<br/> 5. Click Add Customer for save                                                                                     | Critical | High     | ![img_7.png](photos/img_7.png)                                                                      |
| 3     | Different text for "Welcome" and username                                                                      | 1. Open page [Link](https://www.globalsqa.com/angularJs-protractor/BankingProject/#/login)<br/>2. Customer login<br/> 3. Select user and click login<br/>                                                                                                                                                                       | Low      | Low      | ![img_8.png](photos/img_8.png)                                                                      |
| 4     | Amount in transaction is clickable but not have logic                                                          | 1. Open page [Link](https://www.globalsqa.com/angularJs-protractor/BankingProject/#/login)<br/>2. Customer login<br/> 3. Select user and click login<br/> 4. Click transaction button<br/> 5. Click Amount                                                                                                                      | Low      | Low      | ![img.png](photos/img_12.png)                                                                       |
| 5     | Incorrect outline on button                                                                                    | 1. Open page [Link](https://www.globalsqa.com/angularJs-protractor/BankingProject/#/login)<br/>2. Customer login<br/> 3. Select user and click login<br/> 4. Click Deposit button 5. Outline is incorrect                                                                                                                       | Low      | Low      | ![img_11.png](photos/img_11.png)                                                                    |
| 6     | Reset button in transaction delete user balance                                                                | 1. Open page [Link](https://www.globalsqa.com/angularJs-protractor/BankingProject/#/login)<br/>2. Customer login<br/> 3. Select user and click login<br/> 4. Click transaction button<br/> 5. Click Reset button 6. Balance is null                                                                                             | Blocker  | High     | User balance 10: ![img.png](photos/img_9.png) </br> User balance 0: ![img_1.png](photos/img_10.png) |

#### b. Input Xpath or Css selector (or both on your choice) for next elements(Do not use search by text):

- i. ![img.png](photos/img.png)
  Answer: ```CSS SELECTOR: .btn.logout ```
- ii. ![img_1.png](photos/img_1.png)
  Answer: ```XPATH: //select[@id='accountSelect'] ```
- iii. ![img_2.png](photos/img_2.png)
  ANSWER: ```XPATH: //input[contains(@class,'form-control ng-pristine')]```
- iv. ![img_3.png](photos/img_3.png)
  ANSWER: ```XPATH: //input[contains(@class,'form-control ng-pristine')]```
- v. ![img_4.png](photos/img_4.png)
  ANSWER: ```XPATH: (//button[@ng-click='deleteCust(cust)'][normalize-space()='Delete'])[2]```
- vi. ![img_5.png](photos/img_5.png)
  ANSWER: ```XPATH: //input[@ng-model='fName']```

# Task 2 (select one or more to implement)

#### Make Selenium + Python test with test case on your choice:

1. Customer Login - select Ron Weasly - Select another account - Deposit 100 $ - Transaction check-find deposit
   transaction - check that amount is correct - Logout - Site: Link here
2. Customer Login - select Harry Potter - Withdraw 100 $ - Transaction failed check - Deposit 100 $ - Transaction
   success check-find two deposit transaction - check that amount is correct - Logout - Site: Link here
3. Bank manager login - add new customer - find new customer in Customers tab - add new account for that new
   customer - Customer login - user can log in - new account present - Site: Link here
4. Select Category phones - Add to cart - Find in cart - Place order - Input data - Purchase - Site: Link here
