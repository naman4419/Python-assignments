
import math

class Solid:
    def __init__(self):
        self.shape = ""
        self.dimensions = {}

    def accept_data(self):
        print("Choose the solid shape:")
        print("1. Cube")
        print("2. Sphere")
        print("3. Cylinder")
        choice = int(input("Enter your choice (1/2/3): "))

        if choice == 1:
            self.shape = "cube"
            side = float(input("Enter the side of the cube: "))
            self.dimensions['side'] = side

        elif choice == 2:
            self.shape = "sphere"
            radius = float(input("Enter the radius of the sphere: "))
            self.dimensions['radius'] = radius

        elif choice == 3:
            self.shape = "cylinder"
            radius = float(input("Enter the radius of the cylinder: "))
            height = float(input("Enter the height of the cylinder: "))
            self.dimensions['radius'] = radius
            self.dimensions['height'] = height

        else:
            print("Invalid choice.")
    
    def surface_area(self):
        if self.shape == "cube":
            side = self.dimensions['side']
            return 6 * side * side

        elif self.shape == "sphere":
            r = self.dimensions['radius']
            return 4 * math.pi * r * r

        elif self.shape == "cylinder":
            r = self.dimensions['radius']
            h = self.dimensions['height']
            return 2 * math.pi * r * (r + h)

        else:
            return 0

    def volume(self):
        if self.shape == "cube":
            side = self.dimensions['side']
            return side ** 3

        elif self.shape == "sphere":
            r = self.dimensions['radius']
            return (4/3) * math.pi * r ** 3

        elif self.shape == "cylinder":
            r = self.dimensions['radius']
            h = self.dimensions['height']
            return math.pi * r ** 2 * h

        else:
            return 0

solid = Solid()
solid.accept_data()
print("\nShape:", solid.shape.capitalize())
print("Surface Area:", round(solid.surface_area(), 2))
print("Volume:", round(solid.volume(), 2))
