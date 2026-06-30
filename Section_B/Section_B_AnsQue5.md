## **Q5. Loop and Function Reasoning**

**Write a Python function on paper named readiness_score that accepts attendance percentage, diary entries, and task count. It should return a score out of 100 using your own logical weightage. Use at least one if/elif/else block.**

```python
def readiness_score(attendance_pct, diary_entries, tasks_completed):
    score = (attendance_pct * 0.5) + (diary_entries * 2) + (tasks_completed * 3)

    if attendance_pct < 50:
        score -= 10
    elif attendance_pct >= 90:
        score += 5
    else:
        score += 0

    return min(score, 100)
```
