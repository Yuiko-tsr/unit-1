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
I will design and make an **electronic ledger** for a client who is **Ms. Sato**, a **cryptocurrency trader** interested in the **emerging market of cryptocurrencies**. The ledger will be about **tracking cryptocurrency transactions** and is constructed using the software **Python**. It will take approximately **one month** to make and will be evaluated according to the criteria outlined in the success criteria, including functionality, usability, and multilingual support.

**Binance Coin (BNB)** is a cryptocurrency issued by the Binance exchange and trades with the BNB symbol. Binance Exchange is the largest cryptocurrency exchange in the world, with a volume of $8.3 billion as of June 2023.

**Benefits:**
- BNB uses an Auto-Burn system to reduce its total supply to 100,000,000 BNB, which offers greater transparency and predictability to the BNB community.
- Users of Binance Coin receive a discount in transaction fees on the Binance Exchange as an incentive.
- Binance Coin is a great utility token because of the current landscape of the crypto world and the progress of Binance.

**Why Python:**
* **User-Friendly Interface:** Python allows for the creation of user-friendly, terminal-based interfaces that are intuitive and easy to navigate. This ensures that Ms. Sato can efficiently manage her cryptocurrency transactions without a steep learning curve.
* **Customization:** Python provides the flexibility to tailor the software to Ms. Sato's specific requirements. Developers can design the ledger to include the features she needs, such as tracking cryptocurrency amounts, recording transactions, and displaying essential statistics.
* **Data Handling:** Python excels at data manipulation and analysis, making it suitable for managing transaction records and providing Ms. Sato with meaningful statistics. Python's libraries, such as Pandas and Matplotlib, will enable the software to organize and visualize her transaction data effectively.
* **Ease of Maintenance:** Python's clean and readable syntax simplifies software maintenance and updates. As Ms. Sato's cryptocurrency preferences evolve, the software can be easily adapted to support new cryptocurrencies or additional features.

## Success Criteria
1. The electronic ledger is a text-based software (Runs in the Terminal).
2. The electronic ledger display the basic description of the cyrptocurrency selected.
3. The electronic ledger allows to enter, withdraw and record transactions.
4. The electronic ledger allows the user to change currency to yen.
5. The electronic ledger allows the user to make a list of past transactions. 
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
<img width="362" alt="Screen Shot 2023-10-01 at 20 35 04" src="https://github.com/Yuiko-tsr/unit-1/assets/134657923/7e5c80ea-253e-4238-be46-bef84fe81a53">

**Fig. 1** Image of system diagram 

{in_name} means the user's name and is connected to the user's personal csv with the transaction. Moreover, each of the language_{lang}.csv corresponds to a csv with a certain language (0=English, 1=Japanese, 2=Spanish, 3=Chinese.

## Flow Diagrams
<img width="551" alt="Screen Shot 2023-10-05 at 9 47 58" src="https://github.com/Yuiko-tsr/unit-1/assets/134657923/e426e93a-e325-4af1-9796-af0584909484">

** Fig. 2** This is the flow diagram for the login system (Most complex)

<img width="538" alt="Screen Shot 2023-10-02 at 8 55 10" src="https://github.com/Yuiko-tsr/unit-1/assets/134657923/fb1a2519-1c79-4760-866a-a13b881247a7">

** Fig. 3** This is the flow diagram for the message function (Most important)

<img width="538" alt="Screen Shot 2023-10-02 at 8 45 32" src="https://github.com/Yuiko-tsr/unit-1/assets/134657923/b98fbf51-423e-46e1-be6f-034bdd2885c6">

** Fig. 4** This is the flow diagram for the function for try_login (needed for the code of the login system **Fig. 2**

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
| 13 | Complete the discription of the code                                         | To allow other coders to understand the system.                                                                                                                                     | 20 min        | Oct 1                  | C         |

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

** Fig. 5 ** This is the evaluation criteria for the unit testing.

# Criteria C: Development
## Techniques Used:
1. Functions
2. For/while loops
3. Input Validation
4. If/then/else statements
5. Encryption
6. List Comprehension
7. Global Statement
8. Import getpass, csv, datetime, time (source of getpass: Bernard Lee)
   
## Login System
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
As you can see in the flow diagram in **Fig. 4**, in the first line I am defining a function called try_login, this function has two inputs of type string, and the output is a boolean representing True if the user logins correctly or false otherwise. This is saved in the variable success. 
Then in line two and three we ask the code to read the lines on file "users.csv" to read mode ('mode='r'') and read all the lines into the 'data' variable as a list of strings. Each string in the 'data' list represents a line from the file. 

The 'try_login' function is designed to check if a given 'name' and 'password' match any user credentials stored in the 'users.csv' file. It does this by iterating through each line in the 'data' list, splitting each line into 'uname' (username) and 'upass' (password) using the ',' delimiter (assuming that the file format is username,password). It then compares 'uname' and 'upass' with the provided 'name' and 'password'. If there is a match, it sets the 'success' variable to True and breaks out of the loop. If no match is found, 'success' remains False.  

The code then proceeds to test the login using a loop. It allows the user three attempts to enter their username and password correctly. The initial input for 'in_name' and 'in_pass' is taken outside the loop. If they continue to fail the login, a message will appear saying "sayonara" while if they are successful a message will appear saying "welcome".

## Enter Transaction
```.py
def enter():
    amount_e = input(message(4, lang)) #how much would you like to deposit
    while not amount_e.isdigit():
        amount_e = input(RED+message(5, lang)+RESET)
    date = datetime.date.today()
    line = f"{date},{amount_e}\n"
    time.sleep(1)
    print(GREEN + message(6, lang) + RESET) #Depositing...
    time.sleep(1)
    print(f"{GREEN}{amount_e}{message(7, lang)} {date}{RESET}") #{amount_e} has been deposited on {date}
    with open(f"{in_name}.csv", 'a') as myfile:
        myfile.writelines(line)
```
Above is the function that allows the user to deposit into the transaction. The first line asks the user to input the amount they would like to input and the second and third line makes sure that the input is a valid integer. After that the system loads the date and prints the amount and date of deposit and inserts the information into the user's personal csv.

## Withdraw Transaction
```.py
def withdraw():
    global totalleft
    amount_w = input(message(9, lang)) #how much would you like to withdraw
    while not amount_w.isdigit():
        amount_w = input(f"{RED}{message(10, lang)}{RESET}") #Error, how much would you like to withdraw
    while amount_w <= 0:
        amount_w = input(f"{RED}{message(10, lang)}{RESET}") #Error, how much would you like to withdraw

    totalleft = total_left()

    while amount_w > totalleft:
        amount_w = int(input(RED+message(11, lang)+ RESET)) #Error, you cannot withdraw more than there is in the transaction
    date = datetime.date.today()
    line = f"{date},-{amount_w}\n"
    time.sleep(1)
    print(RED+message(12, lang)+ RESET) #Withdrawing...
    time.sleep(1)
    print(f"{RED}{amount_w}{message(13, lang)} {date}{RESET}") #you withdrawed {amount_w} on {date}
    left = totalleft - amount_w
    print(f"{message(14, lang)} {left} {message(15, lang)}{RESET}") #you have a total of {left} BNB
    with open(f"{in_name}.csv", 'a') as myfile:
        myfile.writelines(line)
```
Above is the function that allows the user to withdraw from the transaction. The user how much they would like to withdraw and the four lines after that makes sure that the input is a valid integer. It also makes sure that there are no minus values. Then the code takes the total amount of Bitcoin in the transaction and the two lines after that makes sure that the withdrawed amount is less than the amount in the transaction. Then the system loads the date and prints the amount and date that has been deposited as well as the amount that is remaining in the transaction. Then the system adds this withdrawal to the transaction history.

## View Profit
```.py
def profit_calculator():
    global profit
    with open(f"{in_name}.csv", mode='r') as f:
        csv_reader = csv.reader(f)
        totalleft = 0
        first_deposit = None
        for line in csv_reader:
            date, amount_str = line
            amount = int(amount_str)
            if first_deposit is None:
                first_deposit = amount
            totalleft += amount

        profit = totalleft - first_deposit
        print(f"{message(60, lang)} {first_deposit} {message(61, lang)} {totalleft}") # your first deposite was {first_deposit} and your total is
        if profit <0:
            print(f"{RED}{message(8, lang)} {profit}{RESET}") #your profit is
        else:
            print(f"{GREEN}{message(8, lang)} {profit}{RESET}") #your profit is
```
Above is the function that allows the user to view their profit. First the code opens the user's personal csv and reads the file. For every line they take the amount and add the amount to the totalleft as well as make the first amount the first_deposit. After that they take the total amount in the transaction and minus the first_deposit to calculate the profit. If the total is positive the message would be printed in green to show that there is profit while if the total is negative the message would be printed in red to show that there is loss.
## Change Currency
```.py
def changecurrency():
    profit_calculator()
    currency = input(f"{message(16, lang)}\n{message(52, lang)}\n{message(53, lang)}\n{message(54, lang)}\n{message(55, lang)}") #which currency would you like to change to
    while not currency in "1,2,3,4":
        currency = input(RED+message(17, lang)+ RESET)
    time.sleep(1)
    if currency == "1":
        print(f"{message(18, lang)}{profit * 220}") #Dollars
    elif currency == "2":
        print(f"{message(19, lang)}{profit * 32400}") #Yen
    elif currency == "3":
        print(f"{message(20, lang)}{profit * 205}") #Euro
    elif currency == "4":
        print(f"{message(21, lang)}{profit * 1600}") #Yuan
```
Above is the function that changes the currency of the profit to allow the user to view understand the amount of their profit more easily. The first line asks which currency the user would like to change to. After the choice has been made the system prints the changed currency accordingly.
## Vieew List of Past Transaction
```.py
def print_table():
    print(f"{message(22, lang)}{' '*8}{message(23, lang)}{' '*2}{message(24, lang)}")
    with open(f"{in_name}.csv", 'r') as f:
        csv_reader = csv.reader(f)
        for row in csv_reader:
            date, amount = row
            amount = int(amount)
            if amount >= 0:
                transaction_type = message(25, lang)
                color = GREEN
            else:
                transaction_type = message(26, lang)
                color =RED
            if transaction_type == message(26, lang):
                amount = abs(amount)
            print(f"{color}{date}{' ' * (12 - len(date))}{transaction_type}{' ' * (20 - len(transaction_type))}{amount}{' ' * (10 - len(str(amount)))}{RESET}")
```
Above is the function that prints the list of the past transactions. The first sentence is the title of each column of the table from the left being date, transaction type and amount. Then the code reads the user's personal csv and takes the date and amount. If the amount is larger than 0 it is a deposit and if it is not it is a withdraw. Therefore for each transacrtion history the system will print the date, whether it is deposit or withdraw and the amount of transaction.

## Change Language
```.py
def message(line_number, lang):
    with open(f"language_{lang}.csv", 'r', newline='') as f:
        csv_reader = csv.reader(f)
        for line_count, row in enumerate(csv_reader, start=1):
            if line_count == line_number:
                return row[0]
```
Above is the function that changes the language setting of the system. As shown in the flow diagram in **Fig. 3** each language has a different csv with each line of the csv corresponding to the same message. Therefore, when the function message() called the system opens the specific language's csv and prints the line_number that has been requested.

## Citations
- https://www.investopedia.com/terms/b/binance-coin-bnb.asp
- https://cointelegraph.com/learn/what-is-binance-coin-bnb-and-how-does-it-work
- https://www.binance.com/en/bnb
- https://tradersunion.com/interesting-articles/what-is-binance-coin/

# Video of the Program 
[Video of the Program](https://drive.google.com/file/d/1WAOCgGRHYOQjKun48W7FLEuTUp6bmzTq/view?usp=sharing)
