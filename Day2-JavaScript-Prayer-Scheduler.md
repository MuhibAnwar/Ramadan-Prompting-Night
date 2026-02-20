# Day 2 — JavaScript Prayer Scheduler

**Difficulty:** Easy
**Type:** JavaScript / Logic
**Scoring:** Weighted (Prompt Quality 60pts | Correctness 20pts | Efficiency 20pts)

---

## Challenge

Write a JavaScript function `nextPrayerIndex(currentMinutes, prayerMinutes)` that receives the current time in minutes and a sorted array of prayer times in minutes, returning the index of the next upcoming prayer. If all prayers have passed, return `0` for next-day rollover.

**Example:**
```
nextPrayerIndex(700, [300, 600, 900, 1100]) → 2
// 300 passed, 600 passed, 900 is next → index 2
```

---

## Prompt

**Goal:**
Write a JavaScript function `nextPrayerIndex(currentMinutes, prayerMinutes)` that returns the index of the first element in `prayerMinutes` greater than `currentMinutes`.

**Constraints:**
- `prayerMinutes` is a non-empty sorted ascending array of integers
- `currentMinutes` is a non-negative integer
- Use a single linear scan; no sorting needed

**Edge Cases:**
- If all prayer times ≤ `currentMinutes`, return `0` (next-day rollover)

**Output Format:**
- Function name: `nextPrayerIndex`
- Returns a single integer (the index)
- Example: `nextPrayerIndex(700, [300,600,900,1100])` → `2`

---

## Scoring Strategy

| Factor | Strategy |
|---|---|
| **Prompt Quality (60pts)** | All 4 required sections present, clear and structured |
| **Correctness (20pts)** | Exact function name, correct return type, example matches expected output |
| **Efficiency (20pts)** | Minimal tokens (~65 prompt tokens) — concise, no fluff |
