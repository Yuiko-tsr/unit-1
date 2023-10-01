# Crypto Wallet

# Criteria A: Planning

## Problem definition

Ms. Sato is a local trader who is interested in the emerging market of cryptocurrencies. She has started to buy and sell electronic currencies, however at the moment she is tracking all his transaction using a ledger in a spreadsheet which is starting to become burdensome and too disorganized. It is also difficult for Ms Sato to find past transactions or important statistics about the currency. Ms Sato is in need of a digital ledger that helps her track the amount of the cryptocurrency, the transactions, along with useful statistics. 

Apart for this requirements, Ms Sato is open to explore a cryptocurrency selected by the developer.

An example of the data stored is 

| Date | Description | Category | Amount  |
|------|-------------|----------|---------|
| Sep 23 2022 | bought a house | Expenses | 10 BTC |
| Sep 24 2022 | food for house celebration | Food | 0.000001 BTC |

## Proposed Solution
Design statement:
I will design and make an electronic ledger for a client who is Ms. Sato, a cryptocurrency trader interested in the emerging market of cryptocurrencies. The ledger will be about tracking cryptocurrency transactions and is constructed using the software Python. It will take approximately one month to make and will be evaluated according to the criteria outlined in the success criteria, including functionality, usability, and multilingual support.

Binance Coin (BNB) is a cryptocurrency issued by the Binance exchange and trades with the BNB symbol. Binance Exchange is the largest cryptocurrency exchange in the world, with a volume of $8.3 billion as of June 2023.

Benefits: 
- BNB uses an Auto-Burn system to reduce its total supply to 100,000,000 BNB, which offers greater transparency and predictability to the BNB community.
- Users of Binance Coin receive a discount in transaction fees on the Binance Exchange as an incentive.
- Binance Coin is a great utility token because of the current landscape of the crypto world and the progress of Binance.

Citations
- https://www.investopedia.com/terms/b/binance-coin-bnb.asp
- https://cointelegraph.com/learn/what-is-binance-coin-bnb-and-how-does-it-work
- https://www.binance.com/en/bnb
- https://tradersunion.com/interesting-articles/what-is-binance-coin/

Why Python:
* User-Friendly Interface: Python allows for the creation of user-friendly, terminal-based interfaces that are intuitive and easy to navigate. This ensures that Ms. Sato can efficiently manage her cryptocurrency transactions without a steep learning curve.
* Customization: Python provides the flexibility to tailor the software to Ms. Sato's specific requirements. Developers can design the ledger to include the features she needs, such as tracking cryptocurrency amounts, recording transactions, and displaying essential statistics.
* Data Handling: Python excels at data manipulation and analysis, making it suitable for managing transaction records and providing Ms. Sato with meaningful statistics. Python's libraries, such as Pandas and Matplotlib, will enable the software to organize and visualize her transaction data effectively.
* Ease of Maintenance: Python's clean and readable syntax simplifies software maintenance and updates. As Ms. Sato's cryptocurrency preferences evolve, the software can be easily adapted to support new cryptocurrencies or additional features.

## Success Criteria
1. The electronic ledger is a text-based software (Runs in the Terminal).
2. The electronic ledger display the basic description of the cyrptocurrency selected.
3. The electronic ledger allows to enter, withdraw and record transactions.
4. The electronic ledger allows the user to change currency to yen.
5. The electronic ledger allows the user to make a graph of past transactions. 
6. The electronic ledger allows the user to see the profit they made from their first input.
7. The electronic ledger can be viewed in one other language.

## Justification of Program
* Basic Description Display: The software will provide users with a basic description of Binance Coin, sourced from reputable references like Investopedia and Binance's official website.
* Transaction Management: Users will be able to enter, withdraw, and record Binance Coin transactions, ensuring an accurate and up-to-date ledger.
* Currency Conversion: An optional feature will allow users to convert their portfolio value to yen, helping users understand their holdings in their preferred currency.
* Transaction History Graphs: The software will enable users to create visual graphs of their past transactions, providing insights into their trading performance.
* Profit Calculation: Users will have the ability to see the profit or loss made from their initial input, helping them assess the success of their Binance Coin investments.
* Multilingual Support: To cater to a global user base, the software will offer language options beyond English, enhancing accessibility.

# Criteria B: Design

## System Diagram
<img width="482" alt="Screen Shot 2023-10-01 at 20 35 04" src="https://github.com/Yuiko-tsr/unit-1/assets/134657923/7e5c80ea-253e-4238-be46-bef84fe81a53">

**Fig. 1** Image of system diagram

## Flow Diagrams
<img width="475" alt="Screen Shot 2023-09-14 at 13 49 01" src="https://github.com/Yuiko-tsr/unit-1/assets/134657923/46274dff-34dd-46c6-963c-625ca43e8e50">

** Fig. 2** This is the flow diagram for the login system

## Record of Tasks
|    | Planned Action                                                              | Planned Outcome                                                                                                                                                                     | Time estimate | Target completion date | Criterion |
|----|-----------------------------------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|------------------------|-----------|
| 1  | Create system diagram                                                       | To have a clear idea of the hardware and software requirements for the proposed solution                                                                                            | 10min         | Sep 13                 | B         |
| 2  | Create a Login System                                                       | To have a flow diagram and the code for the login system                                                                                                                            | 30min         | Sep 14                 | B,C       |
| 3  | Discuss with Client on Success Criteria                                     | To have an understanding of what the client is expecting from the program                                                                                                           | 10min         | Sep 18                 | A         |
| 4  | Begin creating "Select Language", "Menu" and "Sign in"                      | To allow users to navigate in both English and Japanese, create an account, login without showing the password, enter and withdraw bitcoin, understand what bitcoin is and sign out | 90 min        | Sep 19                 | B,C       |
| 5  | Create the options and move them to the library.py to make the code clearer | To allow users to enter/withdraw,calculate the profit.                                                                                                                              | 30 min        | Sep 20                 | B,C       |
| 6  | Create the change currency and view past transaction functions.             | To allow users to view past transactions and see their profit in different currencies.                                                                                              | 50 min        | Sep 21                 | B,C       |
| 7  | Allow the change language to happen                                         | To allow users to nagigate in English, Japanese, Chinese and Spanish                                                                                                                | 40 min        | Sep 27                 | B,C       |
| 8  | Fill in the criteria C in order to have detailed documentation.             | For Dr. Ruben to be able to understand each code and reason of code and create flow diagrams.                                                                                       | 40 min        | Sep 27                 | B,C       |
| 9  | Add color so it is easier to view.                                          | To allow users to visually see what the actions are.                                                                                                                                | 20 min        | Sep 28                 | B,C       |
| 10 | Conduct testing in class                                                    | To confirm that each code works and functions well and to make it more useful for the user.                                                                                         | 10 min        | Sep 29                 | B,C       |
| 11 | Add the forgot password function (inspired by Victor)                       | To allow users to gain their password if they forget.                                                                                                                               | 30 min        | Sep 30                 | B,C       |
| 12 | Create System Diagram and flowchart                                         | To allow other coders to understand the system.                                                                                                                                     | 20 min        | Oct 1                  | B         |

## Testing Plan
| Test No | Type of test        | Area Tested           | Outcome of test                                                                                                                                                               | Time estimate | Target completion date | Criterion |
|---------|---------------------|-----------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|---------------|------------------------|-----------|
| 1       | Unit Testing        | Login System          | Confirmed that user can login if they have an account and will not be able to login after 3 attempts.                                                                         | 5min          | Sep 18                 | B         |
| 2       | Unit Testing        | Enter/Withdraw        | Confirm that user can enter/withdraw as well as that the data is inputed into their personal csv.                                                                             | 10min         | Sep 22                 | B         |
| 3       | Unit Testing        | Profit Calculater     | Confirm that the profit calculated is the same and that the currency converted is accurate.                                                                                   | 10min         | Sep 23                 | B         |
| 4       | Unit Testing        | View Past Transaction | Confirm that the past transactions are visually pleasant as well as they are accurate.                                                                                        | 10min         | Sep 24                 | B         |
| 5       | Unit Testing        | Sign up               | Confirm that the username is a unique one (that has not been used before) and that the username and password is inputed in to a specific csv with all the users' information. | 10min         | Sep 25                 | B         |
| 6       | Unit Testing        | Message               | Confirm that each message is printed in English properly from the message csv.                                                                                                | 10min         | Sep 26                 | B         |
| 7       | Integration Testing | Sign up and Login     | Confirm that the Sign up and Login functions work well with one another.                                                                                                      | 10min         | Sep 27                 | B         |
| 8       | Unit Testing        | Change Language       | Confirm that users can change language and that each language is displayed accurately.                                                                                        | 20min         | Sep 28                 | B         |
| 9       | System Testing      | General               | Confirm that the system flows with the use of menu.                                                                                                                           | 20min         | Sep 29                 | B         |
| 10      | Userbility Testing  | General               | Confirming that the system is friendly for the users                                                                                                                          | 10min         | Sep29                  | B         |

<img width="513" alt="Screen Shot 2023-09-18 at 8 59 01" src="https://github.com/Yuiko-tsr/unit-1/assets/134657923/b0aac5e7-d308-4783-a896-a85101fde8a2">

** Fig. 3 ** This is the evaluation criteria for the unit testing.

# Criteria C: Development

## Login System
As you can see in the flow diagram in **Fig 1**, in the first line I am defining a function called try_login, this function has two inputs of type string, and the output is a boolean representing True if the user logins correctly or false otherwise. This is saved in the variable success. 
Then in line two and three we ask the code to read the lines on file "users.csv" to read mode ('mode='r'') and read all the lines into the 'data' variable as a list of strings. Each string in the 'data' list represents a line from the file. 

The 'try_login' function is designed to check if a given 'name' and 'password' match any user credentials stored in the 'users.csv' file. It does this by iterating through each line in the 'data' list, splitting each line into 'uname' (username) and 'upass' (password) using the ',' delimiter (assuming that the file format is username,password). It then compares 'uname' and 'upass' with the provided 'name' and 'password'. If there is a match, it sets the 'success' variable to True and breaks out of the loop. If no match is found, 'success' remains False.  

The code then proceeds to test the login using a loop. It allows the user three attempts to enter their username and password correctly. The initial input for 'in_name' and 'in_pass' is taken outside the loop. If they continue to fail the login, a message will appear saying "sayonara" while if they are successful a message will appear saying "welcome".
```.py
def try_login(name:str, password:str)->bool:
    with open('users.csv',mode='r') as f:
        data = f.readlines()
    success = False

    for line in data:
        uname = line.split(',')[0]
        upass = line.split(',')[1].strip()
        if uname == name and upass == password:
            success = True
            break
    return success

### testing
attempts = 3
in_name = input("Enter your user name:")
in_pass = input("Enter your password:")
result = try_login(name=in_name,password=in_pass)
while result == False and attempts > 1:
    in_name = input("[Error try again] Enter your user name:")
    in_pass = input("[Error try again] Enter your password:")
    result = try_login(name=in_name, password=in_pass)
    attempts -= 1

if result == False:
    print("Sayonara")
    exit(1) #1 is the code for exit without error

# the program continues here if it does close
print("Welcome")

#the rest of your program
```
# Video of the Program 
[Video of the Program](https://drive.google.com/file/d/1gUIQnzA8aQQ_K1IwTqDpziolSwVDi2Je/view?usp=sharing)
