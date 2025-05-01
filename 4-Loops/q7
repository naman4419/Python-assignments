def factorial(n):
    fact=1
    for i in range(1,n+1):
        fact=fact*i
    return fact

def ncr(n,r):
    return factorial(n)//(factorial(r)*factorial(n-r))
def npr(n,r):
    return factorial(n)//factorial(n-r)

n = int(input("Enter value of n: "))
r = int(input("Enter value of r: "))
if r > n:
    print("r should be less than or equal to n")
else:
    print(ncr(n,r))
