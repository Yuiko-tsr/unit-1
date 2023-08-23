#intro.py
"""
Hashtags and three quotation marks act as a comment
"""

my_name = "Yuiko Tsuruno"
"""
Name of a valuable cannot have spaces

when giving a valuable it must be in quotation marks
"""
my_email = "yuikotsuruno@gmail.com"

is_student = True # This is a boolean True:1 or False:0

my_age = 16 # This is an integer

my_height = 154.9 # This is a float

# Show messages with print()
print(my_name)
print(my_email, my_age, end="") # Means that the next print will not be on a new line
print(my_height)


# f-string allows the conversion of text and valuables
print(f"Welcome {my_name}, your email is {my_email} :)))")
print("Welcome", my_name, "your email is", my_email)

#input
position = input("Please enter your position")
salary = int(input("Please enter your salary JPY"))
#inputs are usually text so you have to convert the input to something like an integer

print(f"Your position is {position} and salary is {salary}")

# # Validating correct inputs from user
# while True:
#     user_input = input("Please enter your graduation year: ")
#     if user_input.isdigit():
#         year = int(user_input)
#         break
#     else:
#         print("Invalid input. Please enter a valid year.")
#
# first_name = input("Please enter your first name ")
# title_case_first_name = first_name.title()
#
# last_name = input("Please enter your last name")
#
# email = f"{year}.{title_case_first_name}.{last_name}@uwcisak.jp"
# print(email)

while True:
    input_email = input("Please enter your email: ")
    if "@" in input_email:
        email = input_email
        break
    else:
        print("Invalid email. Please enter a valid email.")

if email.endswith("@uwcisak.jp"):
    print("User is at UWCISAK")
else:
    print("User is not at UWCISAK")
