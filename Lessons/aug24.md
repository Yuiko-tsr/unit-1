#Quiz 002

user_A = input("please input number A")
user_B = input("please input number B")

while True:
    if user_A.isdigit():
        A = int(user_A)
        break
    else:
        print("please enter valid number A")

while True:
    if user_B.isdigit():
        B = int(user_B)
        break
    else:
        print("please enter valid number B")

if (A==20) or (B==20) or (A+B==20):
    print("True")
else:
    print("False")

#First practice question with the if statement
user_input = input("please input a number")
while True:
    if user_input[1:].isdigit():
        number = int(user_input)
        break
    else:
        print("please input a valid number")

if number >= 0:
    print("number is a positive number")
else:
    print("number is a negative number")

#use of multiple if statements

A = int(input("please input number A"))
B = int(input("please input number B"))
C = int(input("please input number C"))

if A > B:
    if A > C:
        if B > C:
            print(A,B,C)
        else:
            print(A,C,B)
    else:
        print(C,A,B)
elif B > C:
    if A > C:
        print(B,A,C)
    else:
        print(B,C,A)
else:
    print(C,B,A)
