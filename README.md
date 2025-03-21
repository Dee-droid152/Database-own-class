# Database-own-class
# Parent class: Vehicle
class Vehicle:
    def __init__(self, name):
        self.name = name
    
    def move(self):
        pass  # To be implemented by subclasses

# Child class: Car
class Car(Vehicle):
    def move(self):
        print(f"{self.name} is driving 🚗")

# Child class: Plane
class Plane(Vehicle):
    def move(self):
        print(f"{self.name} is flying ✈️")

# Child class: Boat
class Boat(Vehicle):
    def move(self):
        print(f"{self.name} is sailing 🚢")

# Child class: Bicycle
class Bicycle(Vehicle):
    def move(self):
        print(f"{self.name} is pedaling 🚴")

# Creating objects
car = Car("Tesla Model S")
plane = Plane("Boeing 747")
boat = Boat("Titanic")
bicycle = Bicycle("Mountain Bike")

# Using polymorphism
vehicles = [car, plane, boat, bicycle]
for vehicle in vehicles:
    vehicle.move()
