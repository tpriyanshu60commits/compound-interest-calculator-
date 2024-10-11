# compound-interest-calculator-
principle = 0
time = 0
rate = 0

while principle <=0:
    principle = int(input("enter the principle amount - "))
    if principle<=0:
        print("principle can't be less than or equal to zero")
    
while time<=0:
    time = int(input("enter the time required - "))
    if time<=0:
        print("time can't be less than or equal to zero")
        
while rate<=0:
    rate = int(input("enter the rate - "))
    if rate <=0:
        print("rate can't be less than or equal to zero")
        
total = principle * pow((1+ rate/100 ),time)
print(f"the total amount is {total:.2f}")
