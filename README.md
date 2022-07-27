# easy-math-test
import random
 
ans = int(input("도달할 점수 : "))
num = 0 
wrg = int(ans/5)

if wrg == 0 :
    wrg = + 1
    print("your life" ,wrg)
    while  num < ans:
        a = random.randint(1,10)
        b = random.randint(1,10)
        c = ["+", "-",  "*"]
        n = random.randint(0,2)
        print(a,c[n],b)
        re = int(input("정답은? :"))

        if n == 0  :
            if a+b == re :
                print("The answer is :",a+b)
                num = num + 1   
                print("당신의 점수는", num)
            else :  
             print("The answer is :",a+b)
             print("your wrong!")
             wrg = wrg-1
             print("The rest of your life :", wrg)
        if n == 1  :
            if a - b == re :
                print("The answer is :",a-b)
                num = num + 1
                print("당신의 점수는", num)
            else : 
                print("The answer is :",a-b)
                print("your wrong!")
                wrg = wrg -1
                print("The rest of your life :", wrg)
        if n == 2 :
            if a * b == re :
                print("The answer is :",a*b)
                num = num + 1   
                print("당신의 점수는", num)
            else :
                print("The answer is :",a*b)
                print("your wrong!")
                wrg = wrg -1
                print("The rest of your life :", wrg)
        if wrg == 0 :
            print("oh...GG go to study..;;;")
            break
else:   
    print ("your life",wrg) 
    while  num < ans:
        a = random.randint(1,10)
        b = random.randint(1,10)
        c = ["+", "-", "*"]
        n = random.randint(0,2)
        print(a,c[n],b)
        re = int(input("정답은? :"))

        if n == 0  :
            if a+b == re :
                print("The answer is :",a+b)
                num = num + 1   
                print("당신의 점수는", num)
            else :  
             print("The answer is :",a+b)
             print("your wrong!")
             wrg = wrg-1
             print("The rest of your life :", wrg)
        if n == 1  :
            if a - b == re :
                print("The answer is :",a-b)
                num = num + 1
                print("당신의 점수는", num)
            else : 
                print("The answer is :",a-b)
                print("your wrong!")
                wrg = wrg -1
                print("The rest of your life :", wrg)
        if n == 2 :
            if a * b == re :
                print("The answer is :",a*b)
                num = num + 1   
                print("당신의 점수는", num)
            else :
                print("The answer is :",a*b)
                print("your wrong!")
                wrg = wrg -1
                print("The rest of your life :", wrg)
        if wrg == 0 :
            print("oh...GG go to study..;;;")
            break
        
if num == ans :
    print("your genius")
