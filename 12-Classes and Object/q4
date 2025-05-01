
import math

class RegularShape:
    def __init__(self):
        self.shape = ""
        self.dimensions = {}

    def accept_data(self):
        print("Choose a regular shape:")
        print("1. Square")
        print("2. Rectangle")
        print("3. Circle")
        print("4. Triangle (Equilateral)")
        choice = int(input("Enter your choice (1/2/3/4): "))

        if choice == 1:
            self.shape = "square"
            side = float(input("Enter the side of the square: "))
            self.dimensions['side'] = side

        elif choice == 2:
            self.shape = "rectangle"
            length = float(input("Enter the length: "))
            width = float(input("Enter the width: "))
            self.dimensions['length'] = length
            self.dimensions['width'] = width

        elif choice == 3:
            self.shape = "circle"
            radius = float(input("Enter the radius of the circle: "))
            self.dimensions['radius'] = radius

        elif choice == 4:
            self.shape = "triangle"
            side = float(input("Enter the side of the equilateral triangle: "))
            self.dimensions['side'] = side

        else:
            print("Invalid choice.")

    def area(self):
        if self.shape == "square":
            s = self.dimensions['side']
            return s * s

        elif self.shape == "rectangle":
            l = self.dimensions['length']
            w = self.dimensions['width']
            return l * w

        elif self.shape == "circle":
            r = self.dimensions['radius']
            return math.pi * r * r

        elif self.shape == "triangle":
            s = self.dimensions['side']
            return (math.sqrt(3) / 4) * s * s

        else:
            return 0

    def perimeter(self):
        if self.shape == "square":
            s = self.dimensions['side']
            return 4 * s

        elif self.shape == "rectangle":
            l = self.dimensions['length']
            w = self.dimensions['width']
            return 2 * (l + w)

        elif self.shape == "circle":
            r = self.dimensions['radius']
            return 2 * math.pi * r

        elif self.shape == "triangle":
            s = self.dimensions['side']
            return 3 * s

        else:
            return 0

shape = RegularShape()
shape.accept_data()

print("\nShape:", shape.shape.capitalize())
print("Area:", round(shape.area(), 2))
print("Perimeter/Circumference:", round(shape.perimeter(), 2))
