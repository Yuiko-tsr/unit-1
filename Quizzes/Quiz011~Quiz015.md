# Quiz011:
## Question:

Fig. 1 Image of question of Quiz 011

## Answer:
<img width="469" alt="Screen Shot 2023-09-14 at 13 09 55" src="https://github.com/Yuiko-tsr/unit-1/assets/134657923/6562e248-9bde-495a-845e-5fd5e8ac45a3">

Fig. 2 Image of answer of Quiz011
```py
def mulTable(N:int):
    number=""
    if 2 <= N < 10:
        for i in range(1,10):
            number += f"{N} x {i} = {N*i}\n"
    return(number)
out = mulTable(2)
print(out)
```
## Running Code:
<img width="1179" alt="Screen Shot 2023-09-14 at 13 08 45" src="https://github.com/Yuiko-tsr/unit-1/assets/134657923/7e95a1fe-6964-49a4-ac6f-2e6f49e930d4">

Fig. 3 Image of code running of Quiz 011

## Flowchart:
Fig. 4 Image of flowchart of Quiz 011

# Quiz012:
## Question:

Fig. 5 Image of question of Quiz 012

## Answer:
```py
def mystery(A:int, B:int):
    return(A*B-(B-A))

out=mystery(A=2, B=6)
print(out)
out1=mystery(A=4, B=10)
print(out1)
out2=mystery(A=10, B=10)
print(out2)
out3=mystery(A=70, B=50)
print(out3)
```
## Running Code:
<img width="1155" alt="Screen Shot 2023-09-18 at 8 15 25" src="https://github.com/Yuiko-tsr/unit-1/assets/134657923/48868ff6-03a2-4c2b-9038-d1b968e08183">

Fig. 6 Image of code running of Quiz 012

## Flowchart:
Fig. 7 Image of flowchart of Quiz 012

# Quiz013:
## Question:

Fig. 8 Image of question of Quiz 013

## Answer:
```py
def mysteryTwo(A:int, B:int):
    return(A*A)+B
out = mysteryTwo(A=10,B=4)
print(out)
out = mysteryTwo(A=37,B=3)
print(out)
out = mysteryTwo(A=58,B=2)
print(out)
out = mysteryTwo(A=60,B=5)
print(out)
```
## Running Code:
<img width="1196" alt="Screen Shot 2023-09-20 at 9 31 46" src="https://github.com/Yuiko-tsr/unit-1/assets/134657923/33df0829-ca60-4925-90a0-6c4ad325ddde">

Fig. 9 Image of code running of Quiz 013

## Flowchart:
Fig. 10 Image of flowchart of Quiz 013

# Quiz014:
## Question:

Fig. 11 Image of question of Quiz 014

## Answer:
```py
def blackBoxThree(given:str):
    vars = []
    for i in range(26):
        vars.append(0)
    alpha = "abcdefghijklmnopqrstuvwxyz"
    message = " "
    for k in range(len(given)):
        letter = given[k].lower()
        if letter == " ":
            message += " "
        for i in range(len(alpha)):
            if letter == alpha[i]:
                vars[i] += 1
                message += f"{vars[i]}"
    return(message)

out = blackBoxThree(given="hello world")
print(out)
out = blackBoxThree(given="aaaaAABB")
print(out)
out = blackBoxThree(given="abABabAB")
print(out)
out = blackBoxThree(given="Create a Function")
print(out)
```

Fig. 12 Image of my answer of Quiz014
## Running Code:
<img width="1198" alt="Screen Shot 2023-09-27 at 11 22 41" src="https://github.com/Yuiko-tsr/unit-1/assets/134657923/c50a5f27-0426-4e87-af6e-fe34ca2f47c9">

Fig. 13 Image of code running of Quiz 014

## Flowchart:
Fig. 14 Image of flowchart of Quiz 014
