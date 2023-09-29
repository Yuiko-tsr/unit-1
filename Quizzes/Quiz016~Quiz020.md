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
