# 🐍 Python OOP: Abstract Class & Method Example

## 🎯 AIM

To create an **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle`.

## 🧠 ALGORITHM

1. **Import ABC module**:
   - Use `from abc import ABC, abstractmethod` to define abstract classes and methods.

2. **Create Abstract Class `Shape`**:
   - Define an abstract method `calculate_area()` with `@abstractmethod`.

3. **Create Subclass `Rectangle`**:
   - Set default values for `length` and `breadth`.
   - Override `calculate_area()` to compute the rectangle area.

4. **Create Subclass `Circle`**:
   - Set default value for `radius`.
   - Override `calculate_area()` to compute the circle area.

5. **Create Objects & Call Methods**:
   - Instantiate `Rectangle` and `Circle`.
   - Call their `calculate_area()` methods.

## 💻 Program

    def calculate_area(self):
        pass

class Rectangle(Shape):           
    def __init__(self, length=5, breadth=3):
        self.length = length
        self.breadth = breadth

    def calculate_area(self):
        area = self.length * self.breadth
        print(f"Area of Rectangle: {area}")

class Circle(Shape):
    def __init__(self, radius=4):
        self.radius = radius

    def calculate_area(self):
        area = 3.1416 * self.radius * self.radius
        print(f"Area of Circle: {area:.2f}")

rect = Rectangle()
circ = Circle()

rect.calculate_area()
circ.calculate_area()

## Output

<img width="1339" height="688" alt="Screenshot 2025-10-20 212232" src="https://github.com/user-attachments/assets/36185612-56ef-4106-bcb4-96e00a9e42a0" />

## Result

Thus To create an **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle`.
Hence the code has been executed successfully.

# 🐍 Python OOP: Encapsulation with Private Members

## 🎯 AIM

To implement **Encapsulation** in Python by defining a class `Rectangle` with **private member variables** `__length` and `__breadth`.

## 🧠 ALGORITHM

1. **Define the Class**:
   - Create a class `Rectangle` with two private attributes: `__length` and `__breadth`.

2. **Initialize Variables**:
   - Use the `__init__()` constructor to set initial values for `__length` and `__breadth`.

3. **Print Values**:
   - Display the private variables from within the class to demonstrate access.

4. **Instantiate the Object**:
   - Create an object of the `Rectangle` class to trigger the constructor.

## 💻 Program

class Rectangle:                                
    def __init__(self, length, breadth):
        self.__length = length
        self.__breadth = breadth
        self.display_values()

    def display_values(self):
        print(f"Length: {self.__length}")
        print(f"Breadth: {self.__breadth}")

rect = Rectangle(10, 5)

## Output

<img width="1495" height="324" alt="Screenshot 2025-10-20 212700" src="https://github.com/user-attachments/assets/5ac5cb85-ef9f-4708-b342-17e6950badca" />

## Result

Thus To implement **Encapsulation** in Python by defining a class `Rectangle` with **private member variables** `__length` and `__breadth`.
Hence the code has been executed successfully.

# 🐟 Method Overriding-Fish and Shark Class Inheritance in Python

## 🧠 AIM:
To write a Python program that demonstrates class inheritance by creating a parent class `Fish` with a method `type`, and a child class `Shark` that overrides the `type` method.

## 📋 ALGORITHM:

1. Define the `Fish` class with a method named `type()` that prints `"fish"`.
2. Define the `Shark` class as a subclass of `Fish`, and override the `type()` method to print `"shark"`.
3. Create an instance of the `Fish` class named `obj_goldfish`.
4. Create an instance of the `Shark` class named `obj_hammerhead`.
5. Use a `for` loop to iterate over both objects.
6. Within the loop, call the `type()` method using the loop variable.
7. Output will demonstrate method overriding: printing `"fish"` and `"shark"` accordingly.

## 💻 PROGRAM:

class Fish:                       
    def type(self):
        print("fish")

class Shark(Fish):
    def type(self):
        print("shark")
obj_goldfish = Fish()
obj_hammerhead = Shark()
for fish in (obj_goldfish, obj_hammerhead):
    fish.type()
    
## OUTPUT

<img width="1214" height="309" alt="Screenshot 2025-10-20 212940" src="https://github.com/user-attachments/assets/4632e9e8-7e02-4d26-8cd2-80de2cc1070d" />

## RESULT

Thus To write a Python program that demonstrates class inheritance by creating a parent class `Fish` with a method `type`, and a child class `Shark` that overrides the `type` method.
Hence the code has been executed successfully.

# 🐍 Python OOP: Operator Overloading (Less Than `<`)

## 🎯 AIM

To write a Python program that demonstrates **operator overloading** by overloading the **less than (`<`)** operator using a custom class.

## 🧠 ALGORITHM

1. **Create Class `A`**:
   - Define the `__init__()` method to initialize the object with a value `a`.

2. **Overload the `<` Operator**:
   - Define the `__lt__()` method with logic:
     - If `self.a < o.a`, return `"ob1 is less than ob2"`
     - Else, return `"ob2 is less than ob1"`

3. **Create Objects**:
   - Instantiate two objects `ob1` and `ob2` with values.

4. **Use `<` Operator**:
   - Use `print(ob1 < ob2)` to trigger the overloaded behavior.

## 💻 Program

class A:                            
    def __init__(self, a):
        self.a = a

    def __lt__(self, o):               
        if self.a < o.a:
            return "ob1 is less than ob2"
        else:
            return "ob2 is less than ob1"

ob1 = A(10)             
ob2 = A(20)

print(ob1 < ob2)                    

## Output

<img width="1447" height="416" alt="Screenshot 2025-10-20 213159" src="https://github.com/user-attachments/assets/27da301b-7933-4574-b0c6-64615e024f19" />

## Result

Thus To write a Python program that demonstrates **operator overloading** by overloading the **less than (`<`)** operator using a custom class.
Hence the code has been executed successfully.

# # 🐍 Python OOP: Polymorphism with Classes

## 🎯 AIM

To create two specific classes — `Beans` and `Mango`. Then, create a **generic function** that can accept any object and determine its **type** (Fruit or Vegetable) and **color**, using polymorphism.

## 🧠 ALGORITHM

1. **Create Class `Beans`**:
   - Define `type()` method that prints `"Vegetable"`.
   - Define `color()` method that prints `"Green"`.

2. **Create Class `Mango`**:
   - Define `type()` method that prints `"Fruit"`.
   - Define `color()` method that prints `"Yellow"`.

3. **Define Generic Function `func(obj)`**:
   - Call `obj.type()` and `obj.color()` — this works with both `Beans` and `Mango` objects, showcasing **polymorphism**.

4. **Create Objects**:
   - Instantiate `Beans` and `Mango`.
   - Pass them to `func()` and execute the program.

## 💻 Program

class Beans:                        
    def type(self):
        print("Vegetable")

    def color(self):
        print("Green")

class Mango:                
    def type(self):
        print("Fruit")

    def color(self):
        print("Yellow")

def func(obj) :
    obj.type()
    obj.color()

bean_obj = Beans()              
mango_obj = Mango()

func(bean_obj)
func(mango_obj)

## Output

<img width="1315" height="640" alt="Screenshot 2025-10-20 213505" src="https://github.com/user-attachments/assets/bdc6aacf-8ee1-482f-9ef8-65523d4461c7" />

## Result

Thus To create two specific classes — `Beans` and `Mango`. Then, create a **generic function** that can accept any object and determine its **type** (Fruit or Vegetable) and **color**, using polymorphism.
Hence the code has been executed successfully.
