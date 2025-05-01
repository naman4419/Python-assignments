
class ComplexNumber:
    def __init__(self,r,i):
        self.r =r
        self.i =i
    
    def __str__(self):
        if self.i >= 0:
            return f"{self.r} + {self.i}i"
        else:
            return f"{self.r} - {-self.i}i"

    
    def __add__(self, other):
        real_part = self.r + other.r
        imaginary_part = self.i + other.i
        return ComplexNumber(real_part,imaginary_part)

    
    def __sub__(self, other):
        real_part = self.r - other.r
        imaginary_part = self.i- other.i
        return ComplexNumber(real_part, imaginary_part)

    
    def __mul__(self, other):
        real_part = (self.r * other.r) - (self.i * other.i)
        imaginary_part = (self.r * other.i) + (self.i * other.r)
        return ComplexNumber(real_part, imaginary_part)

    
    def __truediv__(self, other):
        denominator = other.r ** 2 + other.i ** 2
        real_part = (self.r* other.r+ self.i * other.i) / denominator
        imaginary_part = (self.i * other.r - self.r * other.i) / denominator
        return ComplexNumber(real_part, imaginary_part)
num1 = ComplexNumber(4, 5)
num2 = ComplexNumber(2, -3)

print("Number 1:", num1)
print("Number 2:", num2)

print("\nAddition:", num1+num2)
print("Subtraction:", num1-num2)
print("Multiplication:", num1*num2)
print("Division:", num1/num2)
