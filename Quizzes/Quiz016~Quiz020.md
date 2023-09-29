# Quiz016:
## Question:

Fig. 1 Image of question of Quiz 016

## Answer:
```.py
def averagelength(word: list) -> int:
    count_specific = 0
    count = 0
    for w in word:
        count+=1
        for i in w:
            count_specific += 1

    return count_specific/count

out = averagelength(["hello","main"])
print(out)
out = averagelength(["Peru","France","Nepal"])
print(out)
out = averagelength(["Computer Science","Art"])
print(out)
out = averagelength(["one","two"])
print(out)
```
<img width="463" alt="Screen Shot 2023-09-29 at 13 08 53" src="https://github.com/Yuiko-tsr/unit-1/assets/134657923/fb4c2e2b-5a03-4e9d-afa8-f21f78f85fe6">

Fig. 2 Image of my answer of Quiz016
## Running Code:
<img width="1170" alt="Screen Shot 2023-09-29 at 13 09 48" src="https://github.com/Yuiko-tsr/unit-1/assets/134657923/7f3d929c-41e5-48d8-97e6-60f717dc27f4">

Fig. 3 Image of code running of Quiz 016
