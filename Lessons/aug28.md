#         arugments(inputs)
#def name (               )
#            output
#   return [variables]
<img width="581" alt="Screen Shot 2023-08-28 at 8 06 14" src="https://github.com/Yuiko-tsr/unit-1/assets/134657923/7f48635f-199b-4c6c-89a9-12702b4d0239">
________________________
#ex) 
#def square(X:int)
#  return X*X
________________________
                  #*input to the function different from the inpur we ask from the user
#def largerInteger(A:int, B:int):int:
#    output="A"
#    if A<B:
#        output="B"
#    return output
#    
#r = largerInteger(2021,15)
#print(r)
________________________
'''
def DNAtranslator(in_protein: str) -> str:
    out_protein = ""
    for protein in in_protein:
        if protein == "A":
            out_protein += "T"
        elif protein == "G":
            out_protein += "C"
        elif protein == "T":
            out_protein += "A"
        elif protein == "C":
            out_protein += "G"
        else:
            out_protein += ""

    return out_protein


input_sequence = "AGBCT"
output_sequence = DNAtranslator(input_sequence)
print(output_sequence)

def mystery_box1(word:str, flip_case:bool) -> str:
    output = ""
    for letter in word:
        output = letter + output
    if flip_case == True:
        output = output.lower()

    return output
test=mystery_box1(word="Hello", flip_case=True)
print(test)


def mystery_box2(input:str) -> tuple:
    if "@" in input:
        delimiter = "@"

        parts = input.split(delimiter)
        user_name = parts[0]
        after = "@" + parts[1]

        user = user_name.replace(".", " ")
        names = user.split()
        first_name = names[0].capitalize()
        last_name = "".join(names[1:]).capitalize()

    return first_name,last_name,after

input="john.doe@gmail.com"
output = mystery_box2(input)
print(output)
'''
