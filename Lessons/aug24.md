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

#Create a program that organizes from largest to smallest three heights in cms entered by the user.
def extract_height(input_str):
    height_str = ''.join(filter(str.isdigit, input_str))
    if height_str:
        return int(height_str)
    return None

while True:
    height_1 = input("Please enter the first height: ")
    height1 = extract_height(height_1)
    if height1 is not None:
        break
    else:
        print("Please input a valid height.")

while True:
    height_2 = input("Please enter the second height: ")
    height2 = extract_height(height_2)
    if height2 is not None:
        break
    else:
        print("Please input a valid height.")

while True:
    height_3 = input("Please enter the third height: ")
    height3 = extract_height(height_3)
    if height3 is not None:
        break
    else:
        print("Please input a valid height.")

if height1 > height2:
    if height1 > height3:
        if height2 > height3:
            print(f"{height1}cm, {height2}cm, {height3}cm")
        else:
            print(f"{height1}cm, {height3}cm, {height2}cm")
    else:
        print(f"{height3}cm, {height1}cm, {height2}cm")
elif height2 > height3:
    if height1 > height3:
        print(f"{height2}cm, {height1}cm, {height3}cm")
    else:
        print(f"{height2}cm, {height3}cm, {height1}cm")
else:
    print(f"{height3}cm, {height2}cm, {height1}cm")
