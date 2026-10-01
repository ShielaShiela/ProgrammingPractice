# Python Counting Exercises

These exercises practice:

- Lists
- `for` loops
- `if` conditions
- Counters
- Simple string and number checks

---

## Exercise 1 — Library Late Returns

A school librarian has a list showing how many days each borrowed book is overdue.

```python
overdue_days = [0, 3, 7, 1, 10, 0, 5]
```

A book is considered **late** if it is overdue by at least **3 days**.

### Task

Count how many books are late.

### Sample Input

```text
[0, 3, 7, 1, 10, 0, 5]
```

### Expected Output

```text
No. of late books: 4
```

### Coding Hint

```python
late_books = 0

for day in overdue_days:
    # Check if day is greater than or equal to 3
    # If yes, add 1 to late_books
```

---

## Exercise 2 — Game High Scores

A player has these scores from several rounds:

```python
scores = [450, 1200, 980, 1500, 300, 1100]
```

A score is considered a **high score** if it is at least **1000 points**.

### Task

Count how many high scores the player achieved.

### Expected Output

```text
No. of high scores: 3
```

### Hint

```python
high_score_count = 0

for score in scores:
    if __________:
        high_score_count += 1
```

Think: *What condition tells us that the score reached 1000?*

---

## Exercise 3 — Online Shop Free Shipping

An online shop recorded the total value of several customer orders.

```python
orders = [34.50, 75.00, 120.50, 49.99, 200.00, 60.00]
```

Customers receive **free shipping** when their order is **$60 or more**.

### Task

Count how many customers qualify for free shipping.

### Expected Output

```text
Customers with free shipping: 4
```

### Coding Guide

```python
free_shipping = 0

for order in orders:
    # Check if order is $60 or more

print(f"Customers with free shipping: {free_shipping}")
```

---

## Exercise 4 — Battery Warning System

A robot checks the battery levels of several devices.

```python
battery_levels = [90, 45, 19, 67, 12, 100, 20]
```

A device needs charging if its battery is **20% or lower**.

### Task

Count how many devices need charging.

### Expected Output

```text
Devices needing charge: 3
```

### Hint

```python
if battery <= ______:
```

---

## Exercise 5 — Rainy Days

The amount of rainfall for seven days is recorded below:

```python
rainfall = [0, 12, 4, 20, 0, 15, 2]
```

A day is considered **rainy** when rainfall is greater than **5 mm**.

### Task

Count the rainy days.

### Expected Output

```text
No. of rainy days: 3
```

### Coding Guide

1. Create a variable called `rainy_days`.
2. Start it at `0`.
3. Loop through `rainfall`.
4. Check whether each amount is greater than `5`.
5. Increase `rainy_days`.
6. Print the result.

---

## Exercise 6 — Detecting VIP Users

A game stores the membership type of its players:

```python
memberships = ["free", "vip", "free", "premium", "vip", "vip", "free"]
```

### Task

Count how many players have `"vip"` membership.

### Expected Output

```text
No. of VIP players: 3
```

### Hint

```python
vip_count = 0

for member in memberships:
    if member == ________:
        vip_count += 1
```

---

## Exercise 7 — Finding Names With the Letter "e"

A teacher has the following student names:

```python
students = ["Emma", "John", "Peter", "Liam", "Grace", "Ryan"]
```

### Task

Count how many names contain the letter `"e"`.

For this exercise, ignore uppercase/lowercase issues.

### Expected Output

```text
Names containing e: 3
```

### Hint

```python
if "e" in name.lower():
```

`.lower()` helps because `"Emma"` starts with a capital `"E"`.

---

## Exercise 8 — Finding Numbers Inside Usernames

A website collected these usernames:

```python
usernames = ["alex", "player123", "maria", "code99", "python", "gamer7"]
```

A username is considered to contain a number if **any character is a digit**.

### Task

Count how many usernames contain at least one number.

### Expected Output

```text
Usernames containing numbers: 3
```

### Hint

```python
for username in usernames:
    for character in username:
        if character.isdigit():
```

Be careful: count each **username only once**, even if it contains several digits.

---

## Exercise 9 — Traffic Speed Monitor

A road camera records these vehicle speeds:

```python
speeds = [45, 62, 80, 51, 90, 58, 73]
```

The speed limit is **60 km/h**.

### Task

Count how many vehicles are speeding.

### Expected Output

```text
Speeding vehicles: 4
```

### Hint

```python
speeding = 0

for speed in speeds:
    if __________:
        speeding += 1
```

---

## Exercise 10 — Restaurant Ratings

Customers gave these restaurant ratings:

```python
ratings = [5, 4, 2, 5, 3, 1, 4, 5]
```

A customer is considered **satisfied** if their rating is **4 or 5**.

### Task

Count how many satisfied customers there are.

### Expected Output

```text
Satisfied customers: 5
```

### Hint

```python
if rating >= 4:
```

---

## Exercise 11 — Warehouse Stock Alert

A shop has the following stock levels:

```python
stock = [25, 3, 17, 5, 0, 30, 8]
```

An item should be reordered when there are **5 or fewer** left.

### Task

Count how many products need to be reordered.

### Expected Output

```text
Products to reorder: 3
```

### Challenge

Also print the stock values that need restocking.

```text
Low stock: 3
Low stock: 5
Low stock: 0
Products to reorder: 3
```

---

## Exercise 12 — Theme Park Ride Requirement

A theme park ride requires visitors to be at least **140 cm tall**.

```python
heights = [135, 150, 142, 120, 160, 139, 145]
```

### Task

Count how many visitors are allowed on the ride.

### Expected Output

```text
Visitors allowed to ride: 4
```

---

## General Coding Pattern

Most exercises follow this pattern:

```python
data = [...]

count = 0

for item in data:
    if CONDITION:
        count += 1

print(f"Result: {count}")
```

The main skill is identifying the correct **condition**.

---

## Challenge Exercise — Pass and Fail Counter

A teacher recorded these test scores:

```python
scores = [95, 45, 78, 52, 88, 30, 67]
```

A student passes if the score is **60 or higher**.

### Task

Count both:

- Students who **passed**
- Students who **failed**

### Expected Output

```text
Passed: 4
Failed: 3
```

### Hint

Try using two counters:

```python
passed = 0
failed = 0

for score in scores:
    if score >= 60:
        # increase passed
    else:
        # increase failed
```
