## **Q4. Control Flow Trace**

**(Dry-run for scores 38, 62, 81, and 94)**

**Logic:**

```python
if score < 40:
    band = "Support"
elif score < 70:
    band = "Good"
elif score < 85:
    band = "Excellent"
else:
    band = "Outstanding"
```

**Dry Run:**

1.  **Score = 38**
    *   `if score < 40:` (38 < 40) -> `True`
    *   `band = "Support"`
    *   **Output Band:** "Support"

2.  **Score = 62**
    *   `if score < 40:` (62 < 40) -> `False`
    *   `elif score < 70:` (62 < 70) -> `True`
    *   `band = "Good"`
    *   **Output Band:** "Good"

3.  **Score = 81**
    *   `if score < 40:` (81 < 40) -> `False`
    *   `elif score < 70:` (81 < 70) -> `False`
    *   `elif score < 85:` (81 < 85) -> `True`
    *   `band = "Excellent"`
    *   **Output Band:** "Excellent"

4.  **Score = 94**
    *   `if score < 40:` (94 < 40) -> `False`
    *   `elif score < 70:` (94 < 70) -> `False`
    *   `elif score < 85:` (94 < 85) -> `False`
    *   `else:` -> This block is executed
    *   `band = "Outstanding"`
    *   **Output Band:** "Outstanding"