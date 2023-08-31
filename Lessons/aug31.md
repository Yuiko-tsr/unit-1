def sum_letters(text:str) -> int:
    alphabet = "abcdefghijklmnopqrstuvwxyz"
    sum_total = 0

    for let in text.lower():
        index = -1
        for i in range(len(alphabet)):
            if let == alphabet[i]:
                index = i + 1
                sum_total += index
    return sum_total

case1 = sum_letters(text="Math")
print(case1)
<img width="791" alt="Screen Shot 2023-08-31 at 15 01 59" src="https://github.com/Yuiko-tsr/unit-1/assets/134657923/3c05b56b-96ac-4ce9-b0aa-c2a53f3e5ef9">

