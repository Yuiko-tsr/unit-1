# Crypto Wallet

![](22ROOSE-master768.gif)  
<sub>Illustration for Glenn Harvey</sub>

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
I will to design and make a ———— for a client who is ———. The ——– will about ———— and is constructed using the software ———. It will take  ———- to make and will be evaluated according to the criteria ———.

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
Why inter

## Success Criteria
1. The electronic ledger is a text-based software (Runs in the Terminal).
2. The electronic ledger display the basic description of the cyrptocurrency selected.
3. The electronic ledger allows to enter, withdraw and record transactions.
4. The electronic ledger allows the user to change current to yen.
5. The electronic ledger allows the user to make a graph of past transactions. 
6. The electronic ledger allows the user to see the profit they made from their first input.
7. The electronic ledger does not show the password when typed.

# Criteria B: Design

## System Diagram

## Flow Diagrams


## Record of Tasks
| Task No | Planned Action                                                | Planned Outcome                                                                                                 | Time estimate | Target completion date | Criterion |
|---------|---------------------------------------------------------------|-----------------------------------------------------------------------------------------------------------------|---------------|------------------------|-----------|
| 1       | Create system diagram                                         | To have a clear idea of the hardware and software requirements for the proposed solution                        | 10min         | Sep 24                 | B         |

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
