# 🐉 Draco's Snack Shop — Conditional Statements Problem
 
## The Story
 
Draco the dragon runs a snack shop in the Enchanted Forest. Every day, adventurers come to buy snacks — but Draco has rules! He only accepts gold coins, and some snacks cost more than others. Help Draco write a program that checks if an adventurer can afford their snack!
 
---
 
## The Variables
 
| Variable | Type | Description |
|---|---|---|
| `gold_coins` | `int` | How many gold coins the adventurer has |
| `snack_price` | `int` | The price of the snack they want |
| `is_member` | `bool` | `True` if they have a Draco's Club card (gets 5 coins off!) |
 
---
 
## The Problem
 
Fill in the blanks to complete Draco's snack checker program:
 
```python
gold_coins = 20
snack_price = 15
is_member = True
 
if is_member _______ True:
    snack_price = snack_price - 5
 
_______ gold_coins >= snack_price:
    _______("You can buy the snack! 🎉")
_______:
    print("Not enough coins... 😢")
```
 
**Word bank:** `if` &nbsp; `else` &nbsp; `print` &nbsp; `==` &nbsp; `!=` &nbsp; `input` &nbsp; `elif`
 
---
 
## Answer Key
 
```python
gold_coins = 20
snack_price = 15
is_member = True
 
if is_member == True:          # == checks if two values are equal
    snack_price = snack_price - 5
 
if gold_coins >= snack_price:  # if starts a conditional check
    print("You can buy the snack! 🎉")  # print() shows text
else:                          # else handles the other case
    print("Not enough coins... 😢")
```
 
---
 
## Sample Input & Output
 
### Case 1 — Club member with enough coins ✅
 
**Input:**
```python
gold_coins = 20
snack_price = 15
is_member = True
```
 
**Step-by-step trace:**
- `is_member == True` → discount applied: 15 − 5 = **10**
- `gold_coins >= snack_price` → 20 >= 10 → **True**
**Output:**
```
You can buy the snack! 🎉
```
 
---
 
### Case 2 — Non-member with exact coins ✅
 
**Input:**
```python
gold_coins = 15
snack_price = 15
is_member = False
```
 
**Step-by-step trace:**
- `is_member == True` → False, no discount
- `gold_coins >= snack_price` → 15 >= 15 → **True**
**Output:**
```
You can buy the snack! 🎉
```
 
---
 
### Case 3 — Not enough coins, no membership ❌
 
**Input:**
```python
gold_coins = 9
snack_price = 15
is_member = False
```
 
**Step-by-step trace:**
- `is_member == True` → False, no discount
- `gold_coins >= snack_price` → 9 >= 15 → **False**
**Output:**
```
Not enough coins... 😢
```
 
---
 
### Case 4 — Member but still too poor ❌
 
**Input:**
```python
gold_coins = 3
snack_price = 15
is_member = True
```
 
**Step-by-step trace:**
- `is_member == True` → discount applied: 15 − 5 = **10**
- `gold_coins >= snack_price` → 3 >= 10 → **False**
**Output:**
```
Not enough coins... 😢
```
 
---
 
## Summary Table
 
| Case | `gold_coins` | `snack_price` | `is_member` | Effective Price | Output |
|---|---|---|---|---|---|
| 1 | 20 | 15 | `True` | 10 | You can buy the snack! 🎉 |
| 2 | 15 | 15 | `False` | 15 | You can buy the snack! 🎉 |
| 3 | 9 | 15 | `False` | 15 | Not enough coins... 😢 |
| 4 | 3 | 15 | `True` | 10 | Not enough coins... 😢 |
 
---
 
## Bonus Challenge 🌟
 
What would be printed if `gold_coins = 12`, `snack_price = 15`, and `is_member = True`?  
Work through the steps yourself before running the code!
 
---
 
*Concepts covered: `if`, `else`, comparison operators (`==`, `>=`), `print()`, boolean values (`True`/`False`)*
