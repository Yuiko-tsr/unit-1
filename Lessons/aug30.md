'''
my_info = [20, "bob", "bob.square@pants.com", "deepsea"]

index = 0
for item in my_info:
    print(f"Item {index}: {item}")
    index = index + 1

count_vowels = 0
number = 0
for letter in my_info[2]:
    number = number + 1
    #if letter == "a" or letter=="e" or letter=="o" or letter=="u" or letter=="i":
        #count_vowels = count_vowels + 1
    if letter in "aiueo":
        count_vowels += 1

percentage = count_vowels/number*100

print(f"Perentage of vowel in email is {round(percentage)}%")
print(f"The number of vowels in the email is {count_vowels}")
print(f"The number of letters in the email is {number}")

# print all the numbers form 1:2023

number = 0

for i in range(1,2024): #range(start, end, step)
    print(f"year{number}")
    number += 1

for year in range(0,2024):
    print(f"year{year}")

for odd_number in range(1,1000,2):
    print(odd_number)

for i in range(100):
    print(i%3)

memes = ["lol", "omg", "atp"]
for i in range(100):
    print(memes[i%3], end="-")
'''
number = 21
for i in range(1, 21):
    if number%i ==0:
        print(i)


