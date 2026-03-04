# Day 13 — Node Rate Limit Counter

**Difficulty:** Medium
**Type:** Backend Node.js
**Scoring:** Weighted (Prompt Quality 60pts | Correctness 20pts | Efficiency 20pts)

---

## Challenge

Write `applyRateLimit(count, limit)` returning whether a request is allowed for `count <= limit`.

**Example:**
```
applyRateLimit(3,5) -> true
```

---

## Prompt

**Goal:**
Node `applyRateLimit(count,limit)` → boolean.

**Constraints:**
Return true if count<=limit, false otherwise.

**Edge Cases:**
count===limit→true; count>limit→false.

**Output Format:**
`const applyRateLimit=(count,limit)=>count<=limit;`

---

## Scoring Strategy

| Factor | Strategy |
|---|---|
| **Prompt Quality (60pts)** | All 4 required sections present |
| **Correctness (20pts)** | Exact function name `applyRateLimit`; returns boolean matching `count<=limit` |
| **Efficiency (20pts)** | Solution embedded in Output Format — AI regenerates one-liner, near-zero extra tokens |

---

## Notes

- `count<=limit` covers equality (count===limit → true) and under-limit naturally
- Arrow function one-liner keeps token count minimal
- No imports or extra logic needed
