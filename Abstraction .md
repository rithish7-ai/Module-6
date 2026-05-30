# 🐍 Python OOP: Abstract Class & Method Example

## 🎯 AIM

To create an **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle`.

---

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

---

## 💻 Program
```
from abc import ABC, abstractmethod
class type_shape(ABC):
    @abstractmethod
    def area(self):
        pass

class Rectangle(type_shape):
    def __init__(self, width, height):
        self.width = width
        self.height = height

    def area(self):
        return self.width * self.height

class Square(type_shape):
    def __init__(self, side):
        self.side = side

    def area(self):
        return self.side * self.side

class Circle(type_shape):
    def __init__(self, radius):
        self.radius = radius

    def area(self):
        return 3.14 * self.radius * self.radius

class Triangle(type_shape):
    def __init__(self, base, height):
        self.base = base
        self.height = height

    def area(self):
        return 0.5 * self.base * self.height

rect = Rectangle(6, 4)
circ = Circle(7)
sq = Square(4)
tri = Triangle(5, 4)

print(f"Area of a rectangle: {rect.area()}")
print(f"Area of a circle: {circ.area()}")
print(f"Area of a square: {sq.area()}")
print(f"Area of a triangle: {tri.area()}")

```
## Output
<img width="625" height="353" alt="445658899-ca7a3bd3-1b51-4a03-a103-368e1a0bb2a7" src="https://github.com/user-attachments/assets/0d627d4b-5fcb-40e2-9801-846417181712" />

## Result
Thus,the Python program To create an abstract class named Shape with an abstract method calculate_area, and implement this method in two subclasses: Rectangle and Circle is created successfully.
