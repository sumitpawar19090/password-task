# password-task
import random 
import string

paslength=int(input("inter the password size you want to creat"))

print(''' select the choice: 1. number 2.letter 3. special characters ''') 
charachter="" 
while (True): 
    choice =int (input("enter the choice")) 
    if choice == 1: charachter+= string.ascii_letters 
    elif choice == 2: charachter+= string.digits 
    elif choice == 3: charachter += string.punctuation 
    elif choice == 4: break 
    else : print("plese fill the currect output")
password=[]
for i in range(paslength):

    randomchar=random.choice(charachter)

    password.append(randomchar)
print("the random password is "+ "".join(password))


    
