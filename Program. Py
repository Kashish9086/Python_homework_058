'''Write a Python program to create a class called Circle having an Instance member called radius. Provide following methods in Circle class
_Init(): This method should accept an argument and Initialize radius with it
area(): This method should calculate and return Circle's area

• Now create a derived class of Circle called Cylinder having an instance member called height. Provide following methods in Cylinder class
_init_(): This method should initialize Instance members radius and height with the parameter passed.
area(): This method should override Circle's area() to calculate and return area of Cylinder. (formula: 2m2+2mb)
volume(): This method should calculate and return Cylinder's volume(formula: mr2h) '''

import math

class Circle:
    def __init__(self, radius):
        self.radius = radius

    def area(self):
        return math.pi * self.radius ** 2

class Cylinder(Circle):
    def __init__(self, radius, height):
        super().__init__(radius)
        self.height = height

    def area(self):
        # Overriding the area method to calculate the surface area of the cylinder
        circle_area = super().area()
        lateral_area = 2 * math.pi * self.radius * self.height
        return 2 * circle_area + lateral_area

    def volume(self):
        # Calculating the volume of the cylinder
        return math.pi * self.radius ** 2 * self.height

# Example usage:
radius_circle = 5
circle_obj = Circle(radius_circle)
print(f"Circle Area: {circle_obj.area()}")

radius_cylinder = 3
height_cylinder = 8
cylinder_obj = Cylinder(radius_cylinder, height_cylinder)
print(f"Cylinder Area: {cylinder_obj.area()}")
print(f"Cylinder Volume: {cylinder_obj.volume()}")
