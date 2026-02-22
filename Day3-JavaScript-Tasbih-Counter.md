# Day 3 — JavaScript Tasbih Counter

**Difficulty:** Easy
**Type:** JavaScript / Logic
**Scoring:** Weighted (Prompt Quality 60pts | Correctness 20pts | Efficiency 20pts)

---

## Challenge

Write a JavaScript function `tasbihSessionStats(target, count)` that returns an object with the total target and the remaining count, where remaining is never below zero.

**Example:**
```
tasbihSessionStats(100, 45) → {total: 100, remaining: 55}
tasbihSessionStats(100, 110) → {total: 100, remaining: 0}
```

---

## Prompt

**Goal:**
Write a JavaScript function `tasbihSessionStats(target, count)` that returns session stats for a tasbih counter.

**Constraints:**
- `remaining = target - count`, minimum value is 0
- Function name must be exactly `tasbihSessionStats`

**Edge Cases:**
- `count >= target` → `remaining = 0`
- `count = 0` → `remaining = target`

**Output Format:**
- Function name: `tasbihSessionStats`
- Returns `{total: target, remaining: Math.max(0, target - count)}`
- Example: `tasbihSessionStats(100, 45)` → `{total: 100, remaining: 55}`

---

## Scoring Strategy

| Factor | Strategy |
|---|---|
| **Prompt Quality (60pts)** | All 4 required sections present, clear and structured |
| **Correctness (20pts)** | Exact function name, correct return shape, example matches expected output |
| **Efficiency (20pts)** | Formula embedded directly in Output Format — minimal generated code tokens |
