# task0

# Qs 1
def product_or_sum(n1,n2):
    product=n1*n2
    if(product<=1000):
        return product
    else:
        return n1+n2
   
n1=int(input("Enter the first number"))
n2=int(input("Enter the second number"))

result=product_or_sum(n1,n2)
print("The result is", result)

# Qs 2
n=input("Enter a number to calculate sum of all natural numbers till that number")
n=int(n)
sum=0
for num in range(0,n+1,1):
    sum=sum+num
print("Sum of first",n, "numbers is:", sum)

# Qs 3
num=int(input("Enter any number"))
n=0
while(num>0):
    num=num//10
    n=n+1
print("Number of digits in the given number is %d" %n)

# Qs 4
def EvenIndexChar(str):
    for i in range(0,len(str)-1,2):
        print("index[",i,"]", str[i] )
inputStr = input("Enter String ")
print("Orginal String is ", inputStr)

print("Printing only even index chars")
EvenIndexChar(inputStr)

# Qs 5
n1=int(input("Enter first number"))
n2=int(input("Enter second number"))
print("Prime numbers between", n1, "and", n2, "are:")
for num in range(n1,n2+1):
    if num > 1:
       for i in range(2, num):
           if (num % i) == 0:
               break
       else:
           print(num)

# Qs 6
def fibonacci(n):
    if n == 1:
        return 1
    elif n == 0:
        return 0
    else:
        return fibonacci(n-1) + fibonacci(n-2)
 
num = int(input("Enter an integer: \t"))
for i in range(num):
    print(fibonacci(i))
