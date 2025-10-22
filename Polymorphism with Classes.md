# # 🐍 Python OOP: Polymorphism with Classes

## 🎯 AIM

To create two specific classes — `Beans` and `Mango`. Then, create a **generic function** that can accept any object and determine its **type** (Fruit or Vegetable) and **color**, using polymorphism.

---

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

---

## 💻 Program


class Beans:
    def type(self):
        return "Vegetable"

    def color(self):
        return "Green"

class Mango:
    def type(self):
        return "Fruit"

    def color(self):
        return "Yellow"

def show_details(obj):
    print("Type:", obj.type())
    print("Color:", obj.color())

b = Beans()
m = Mango()

print("Details of Beans:")
show_details(b)

print("\nDetails of Mango:")
show_details(m)

## Output
<img width="576" height="316" alt="image" src="https://github.com/user-attachments/assets/a7b3aca1-cf43-44da-b800-147a1dd0d617" />

## Result
The python program has written successfully.
