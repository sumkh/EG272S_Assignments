### Python Fundamentals & Data Structures

#### **1. Basic Syntax & Operations**
*   **Variable Assignment:**
    *   `a = 100` (Single assignment).
    *   `a, b = 1, 2` (Multiple assignment).
    *   `a, b = b, a + b` (Swapping/updating values; if `a,b=1,2`, then `b` becomes 3).
*   **Printing & Formatting:**
    *   `print("Hello World")`.
    *   `.format()` method: `print("{} + {} = {}".format(a, b, c))`.
    *   f-strings: `print(f"My name is {name}")`.
*   **Arithmetic Operators:** `+`, `-`, `*`, `/`, `**` (Exponent), `%` (Modulus), `//` (Floor Division).
*   **Compound Operators:** `a += 5` (Equivalent to `a = a + 5`).

#### **2. Strings**
*   **Concatenation:** `c = a + b`.
*   **Manipulation Functions:**
    *   `c.upper()` (e.g., "hello" \\(\rightarrow\\) "HELLO").
    *   `c.capitalize()` (e.g., "france" \\(\rightarrow\\) "France").
    *   `c.replace('World', 'Alfred')`.
    *   `a.strip()` (Removes whitespace: `' Hello'.strip()` \\(\rightarrow\\) "Hello").
*   **Searching & Counting:**
    *   `a.split()` (Splits "Today is sunny" into `['Today', 'is', 'sunny']`).
    *   `" is ".join(list)` (Joins list items into a string).
    *   `a.find('nice')` (Returns the starting index of the substring).
    *   `c.count('a')` (Counts occurrences of 'a' in string `c`).

#### **3. Lists (Mutable Collections)**
*   **Creation:** `a =` or `a = ['Physics', 91]`.
*   **Slicing:** `a[1:3]` (items at index 1 and 2), `a[1:]` (index 1 to end), `a[:-1]` (all except last).
*   **Modification:**
    *   `a.append(10)` (Add 10 to the end).
    *   `a.insert(2, 99)` (Insert 99 at index 2).
    *   `a.remove(1)` (Remove the value 1).
    *   `del a` (Delete item at index 1).
    *   `a.pop(1)` (Remove and return item at index 1).
*   **Ordering & Copying:**
    *   `a.sort()` (Sorts list in place).
    *   `c = a.copy()` (Creates a separate copy of list `a`).
*   **Math Functions:** `sum(a)`, `min(a)`, `max(a)`, `len(a)`, `a.count(x)`.

#### **4. Other Data Structures**
*   **Tuples (Immutable):** `a = (1, 2, 3)`.
*   **Dictionaries (Key-Value):** `capitals = {'France': 'Paris', 'Italy': 'Rome'}`.
*   **Sets (Unique Items):** `a = {2, 3, 4}` (Automatically removes duplicates).

---

### Control Flow, Functions, and Libraries

#### **5. Comparison, Logic, and Membership**
*   **Comparison:** `==` (equal), `!=` (not equal), `>`, `<`, `>=`, `<=`.
*   **Membership:** `if 'A' in letters:` (Checks if 'A' exists in the list).
*   **Logical:** `x or y`, `x and y`, `not x`.

#### **6. Control Flow**
*   **Conditionals:**
    ```python
    if a < b:
        print("smaller")
    elif a > b:
        print("larger")
    else:
        print("same")
    ```
*   **Ternary Operator:** `discount = 25 if order_total > 200 else 0`.
*   **Loops:**
    *   `while (a < 10):`.
    *   `for i in a:` (Iterates through list `a`).
    *   `for i in range(1, 6):` (Iterates 1 through 5).
*   **Loop Tools:**
    *   `enumerate(person)`: `for i, name in enumerate(person):` (Tracks index `i` and value `name`).
    *   `zip(a, b)`: `for i, j in zip(person, height):` (Iterates both lists simultaneously).
*   **Interrupts:** `break` (stalls/ends loop), `continue` (skips current iteration).
*   **Loop with Else:** `else:` block executes if the loop finishes without a `break`.

#### **7. Functions & Exceptions**
*   **Syntax:** `def f(x): return x * x`.
*   **Arguments:**
    *   Multiple: `def f(x, y): z = x + y; return z`.
    *   Default: `def f(a=20, b=5): return a * b`.
    *   Named: `f(b=8)` (Specifically assigns value to parameter `b`).
    *   Variable: `def sum(a, *b):` (Accepts any number of arguments into `b`).
*   **Lambda:** `f = lambda x, y: 10 * x + y`.
*   **Exception Handling:**
    ```python
    try:
        a = int(input('Enter integer:'))
    except ValueError:
        print("Not an integer!")
    else:
        print("You entered", a)
    finally:
        print("Try again")
    ```

#### **8. Modules, Files, and OS**
*   **Imports:** `import math`, `import math as m`, `from math import sin, pi`.
*   **Common Modules:**
    *   `math.sqrt(x)`, `math.ceil(10.3)`, `math.floor(47.9)`.
    *   `time.sleep(5)` (Pause for 5 seconds).
    *   `random.choice()`.
*   **File I/O:**
    *   `f = open('file.txt', 'w')` (Open for writing).
    *   `f.write("text\n")`, `f.close()`.
    *   `with open("file.txt", 'r') as f:` (Best practice: auto-closes file).
*   **OS Module:** `os.getcwd()`, `os.mkdir(path)`, `os.listdir(path)`.
*   **Cloud:** `from google.colab import drive; drive.mount('/content/drive')`.

#### **9. Data Science Libraries**
*   **Numpy:** `a1 = np.array()`.
*   **Matplotlib:** `plt.plot(x, y)`, `plt.show()`.
*   **Pandas:**
    *   `df = pd.read_csv('data.csv')`.
    *   Filter: `print(df[df.Students > 70])`.
    *   Locate: `df.loc['name'].bmi`.