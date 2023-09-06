'''
for i in range(1,10001):
    if i%7 ==0:
        print(f"{i} is multiple of 7")
        if i%6==0:
            print(f"{i} is a multple of 6 and 7")
'''

count=0
num=1
while count <500:
    if num%7 ==0 and num%6==0:
        count += 1
    num+=1
print(f"we counted up to {num} to find 500 multiples of 6 and 7")
<img width="703" alt="Screen Shot 2023-09-06 at 11 29 39" src="https://github.com/Yuiko-tsr/unit-1/assets/134657923/ccae3392-8606-4ec0-9e51-a7c4a48d2396">

def frame_maker(msg:str, symbol:str, spaces:int) -> str:
    height = 5
    width = 2+2*spaces+len(msg)
    red = "\33[4;31m"
    end_code="\033[00m"

    topline= symbol*width
    middle_line= symbol+" "*(width-2) +symbol
    message_line= symbol+ " "*spaces + msg.upper() + " "*spaces + symbol

    banner=f"{topline}\n{middle_line}\n{red}{message_line}{end_code}\n{middle_line}\n{topline}"

    return banner

title = "A Cool Game"
cover_game = frame_maker(msg=title, symbol="#", spaces=10)
print(cover_game)

#The guessing number game
#Pick a random number 1-100
import random
secret_number= random.randint(1,100)
#ask the user for a number, indicate if it is bigger or smaller than secret number
guess_number = int(input("Guess the secret number from 1 to 100"))
count=1
while guess_number !=secret_number:
    if guess_number < secret_number:
        print("smaller")
    else:
        print("bigger")
    guess=int(input("Please try another guess:"))
    count += 1

print(f"You won, it took {count} times to guess the secret number")
#count how many tries it took the user
