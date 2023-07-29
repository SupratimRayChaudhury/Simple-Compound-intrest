# Simple-Compound-intrest
It helps to calculate the simple and compound intrest 
while True:
 print("Enter C for Compound Interest/Enter S for Simple interest. e for exit.")
 i=input()
 if i=="S":
   p=float(input("Enter Principal value ="))
   r=float(input("Enter rate of Intrest ="))
   t=float(input("Enter Time Period="))
   s=(p)*(r)*(t)/100
   print("your Interest at the end",int(t),"years will be",u"\u20B9"+str(round(s))+"/-","then the total amount have to pay =",p+s)  
 elif i=="C":
   p=float(input("Enter Principal value ="))
   r=float(input("Enter rate of Intrest ="))
   t=float(input("Enter Time Period="))
   n=int(input("Enter number of times interest applied per time period="))
         
   c=p*(1+r/(n*100))**(n*t)
   print("your Interest at the end",int(t),"years will be",u"\u20B9"+str(round(c))+"/-","then the total amount have to pay =",p+c)
 elif i=="e":
     break
 else:
     print("Invalid Input")
