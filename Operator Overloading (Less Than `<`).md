# 🐍 Python OOP: Operator Overloading (Less Than `<`)

## 🎯 AIM

To write a Python program that demonstrates **operator overloading** by overloading the **less than (`<`)** operator using a custom class.

---

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

---

## 💻 Program

class Box:
    def __init__(self, volume):
        self.volume = volume
    def __lt__(self, other):
        return self.volume < other.volume
box1 = Box(30)
box2 = Box(50)

if box1 < box2:
    print("Box1 is smaller than Box2")
else:
    print("Box1 is not smaller than Box2")


## Output
<img width="700" height="271" alt="image" src="https://github.com/user-attachments/assets/cdaf011c-2443-4eb3-bf9c-018c87d97bf1" />


## Result
The python program had written successfully. 
