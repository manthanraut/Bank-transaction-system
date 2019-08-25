# Bank-transaction-gateway system
This is a simple bank transaction system which is made by using Python language wherein a user is allowed to credit or debit cash from his account and simultaneously checks is the entered details are correct or not .

# Project 1 - Bank Transaction Gateway

Following is the **structure** of the excel file containing information about your bank’s users.

| Sr. No. |   User Id   |      A/c No.      |        Full Name         |  User Email   | A/c Balance | A/c Status |
|---------|-------------|-------------------|--------------------------|---------------|-------------|------------|
|    1    | 19091022001 | 2019091022IND0345 |        Karan Shah        | abc@gmail.com |     500     |   Active   |
|    2    | 19091022002 | 2019091022IND1453 |        Manan Jain        | def@gmail.com |     1000    |   Active   |
|    3    | 19091022003 | 2019091022IND5647 |        Kunal Patil       | xyz@gmail.com |     300     |   Active   |
|    4    | 19091022004 | 2019091022IND3455 |        Ajay Ranade       | jkl@gmail.com |     450     |   Active   |
|    5    | 19091022005 | 2019091022IND9823 |       Tushar Shinde      | pqr@gmail.com |     1560    |   Active   |

Workbook Name - **SITIP19-KIIT-Python-FinalProject1-Workbook.xlsx**

Worksheet Name - **UserDetails**

The project task is as follows:

### Stage 1 : User Validity

- Ask user to enter Full Name or User ID
- If Full Name / User ID not there then tell invalid User
- If it exists, then ask user to enter Bank Account Number
- If A/c number doesn't exist, then tell invalid user
- If both are correct, then proceed to Stage 2
- Give user three tries. If invalid input is given in all three tries then change account status from Active to Blocked and print Account Blocked and print quit program in Stage 1

### Stage 2: OTP Generation and Validity

- Through code generate a 4 digit random OTP number
- Send this OTP to that User via email
- Then ask user to enter OTP from mail. Match this OTP with one generated in code.
- If OTP matches then go to Stage 3. Else say Invalid OTP. 
- Give user three tries. If wrong OTP in all three tries then change account status from Active to Blocked and print Account Blocked and print quit program in Stage 2

### Stage 3 : Choice of Transaction

- Ask user which type of transaction he wishes to do. ‘C’ for credit money and ‘D’ for debit money
- If User enters any other input here then handle error and print Invalid Input. Again give user three tries and if all wrong then change account status from Active to Blocked and print Account Blocked and print quit program in Stage 3
- If correct input then print current balance
- Then ask user for amount to be credited or debited
- Add or subtract amount entered by user to the current account balance and print the final account balance and write the same to account balance cells in excel workbook.
- Print “Successful Transaction of Rs.______ completed”
- Also Print a proper mini-statement of the balance and display it.
