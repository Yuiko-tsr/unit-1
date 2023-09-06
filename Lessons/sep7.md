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

title = "Welcome to Conbini"
welcome = frame_maker(msg=title, symbol="#", spaces=10)
print(welcome)

#Menu
items = ["onigiri", "bread", "chips"]
prices = [500, 200, 150]

#               Menu
#1. Onigiri.........................¥500
#2. Bread...........................¥200
print("MENU".center(57,'-'))
for it in range(len(items)):
    print(f"{it+1}. {items[it].title().ljust(50, '.')}¥{prices[it]}")

order = []
ordering = True
total=0
while ordering:
    selection=input(f"Please enter an item(1-{len(items)}):")
    available=""
    for i in range(len(items)):
        available += str(i+1)

    while not (selection.isdigit() and selection in available):
        selection = input(f"Error, Please enter an item(1-{len(items)}):")

    order.append(int(selection)-1)
    total +=prices[int(selection)-1]
    for it in range(len(items)):
        count = 0
        for o in order:
            if o == it:
                count +=1
        if count>0:
            final_total=0
            total_price = prices[it]*count
            print(f"{items[it].title().ljust(20)} x {count} = ¥{total_price}")
    answer = input("Is this the last item?(Y/N)")
    while not answer in "yYnN":
        answer = input("Error, Is this the last item?(Y/N)")

    if answer in "yY":
        ordering=False
#print the total, plus tax(10%) inside the frame
print(frame_maker(msg=f"You pay ¥{total*1.1:.2f}", spaces=50, symbol="."))
