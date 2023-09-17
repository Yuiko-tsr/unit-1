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

Justification for Proposed Structure:
* Basic Description Display: The software will provide users with a basic description of Binance Coin, sourced from reputable references like Investopedia and Binance's official website.
* Transaction Management: Users will be able to enter, withdraw, and record Binance Coin transactions, ensuring an accurate and up-to-date ledger.
* Currency Conversion: An optional feature will allow users to convert their portfolio value to yen, helping users understand their holdings in their preferred currency.
* Transaction History Graphs: The software will enable users to create visual graphs of their past transactions, providing insights into their trading performance.
* Profit Calculation: Users will have the ability to see the profit or loss made from their initial input, helping them assess the success of their Binance Coin investments.
* Multilingual Support: To cater to a global user base, the software will offer language options beyond English, enhancing accessibility.

# Criteria B: Design

## System Diagram

## Flow Diagrams
<img width="475" alt="Screen Shot 2023-09-14 at 13 49 01" src="https://github.com/Yuiko-tsr/unit-1/assets/134657923/46274dff-34dd-46c6-963c-625ca43e8e50">

** Fig. 1** This is the flow diagram for the login system

## Record of Tasks
| Task No | Planned Action        | Planned Outcome                                                                          | Time estimate | Target completion date | Criterion |
|---------|-----------------------------------------|------------------------------------------------------------------------------------------|---------------|------------------------|-----------|
| 1       | Create system diagram                   | To have a clear idea of the hardware and software requirements for the proposed solution | 10min         | Sep 13                 | B         |
| 2       | Create a Login System                   | To have a flow diagram and the code for the login system                                 | 30min         | Sep 14                 | B,C       |
| 3       | Discuss with Client on Success Criteria | To have an understanding of what the client is expecting from the program                | 10min         | Sep 18                 | A         |
# Criteria C: Development

## Login System
My client requires a system to protect the private data. I thought about using a login system to accomplish this requirement using a if condition and the open command to work with a csv file. More description of the code....
```.py
def simple_login(user:str, password:str)->bool:
    '''
    Simple authentication, needs fle user.csv
    :param user: string
    :param password: string
    :return: True/False if user is in database
    '''
    with open("user.csv") as file:
        database = file.readlines()
    output = False
    for line in database:
        line_cleaned = line.strip() #remove \n
        user_pass = line_cleaned.split(",")
        if user == user_pass[0] and password == user_pass[1]:
            output = True
            break

    return output

```

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
