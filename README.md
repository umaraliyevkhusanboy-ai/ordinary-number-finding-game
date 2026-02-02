# ordinary-number-finding-game
#foundation number finding game on python
from time import sleep


hidden_number = 17
find = False
number_try = 0
print("raqam topish oyini")
sleep(2)
print("oynaymizmi ? ")
sleep(2)
ask = input("ha yoki yoq??? : ")
if ask == "ha":
    print("unda boshladik")
else:
    print("ok unda xayr ")  
for i in range(3,0,-1):
    sleep(2)
    print(i)
print("men 1 dan 20 ga qadar son oyladim uni toping ")
while not find:
    number_try = number_try + 1
    guess = int(input("raqamni kiriting :"))

    if guess == hidden_number:
        print(f"togri topdingiz urunishlar soni :{number_try}")
        sleep(2)
        find = True
    elif guess < hidden_number:
        print("bundan kattaroq raqam kiriting ")
    else:
        print("bundan kichikroq raqam kiriting ")
