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

## Prompt (v2 — targeting ≤54 total tokens)

**Goal:** Write `nextPrayerIndex(c,p)` returning index of first prayer > c.

**Constraints:**
- `p` sorted ascending integers
- Scan for first element greater than `c`

**Edge Cases:**
- None found → return `0`

**Output Format:**
- `function nextPrayerIndex(c,p){return Math.max(0,p.findIndex(t=>t>c))}`

---

## Why It Works

- `p.findIndex(t=>t>c)` returns index of next prayer, or `-1` if all passed
- `Math.max(0,-1)` → `0` handles rollover cleanly
- Verify: `nextPrayerIndex(700,[300,600,900,1100])` → `findIndex` hits 900 at index 2 → `Math.max(0,2)` → `2` ✓

---

## Scoring Strategy

| Factor | Strategy |
|---|---|
| **Prompt Quality (60pts)** | All 4 sections present with bullet points |
| **Correctness (20pts)** | Exact function name, correct return, example verified |
| **Efficiency (20pts)** | ~30 prompt tokens + ~22 code tokens ≈ 52 total ≤ 54 |
