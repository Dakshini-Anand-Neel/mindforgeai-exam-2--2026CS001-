# **SECTION B: HANDWRITTEN PYTHON FUNDAMENTALS**

## **Q3. Variables, Memory and Identity**

**(Explanation of Memory Behavior and Relationship between Values and Object Identity)**

Let's trace the memory behavior for the given code:

```python
a = 25
b = a
c = 25
names = ["Asha", "Riya"]
same_names = names
same_names.append("Neha")
```
### Variables, Memory and Identity

* `a = 25` makes `a` point to the integer object `25` already present in Python's small integer memory pool.
* `b = a` makes `b` point to the same object as `a`.
* `c = 25` also points to the same integer object.
* `names = ["Asha", "Riya"]` creates a new list object, and `names` points to it.
* `same_names = names` creates another reference to the same list.
* `same_names.append("Neha")` updates the original list, so both `names` and `same_names` become `["Asha", "Riya", "Neha"]`.