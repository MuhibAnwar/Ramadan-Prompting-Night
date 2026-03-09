# Day 16 — Docker Compose Service Summary

**Difficulty:** Medium
**Type:** Docker (JS tests on platform)
**Scoring:** Weighted (Prompt Quality 60pts | Correctness 20pts | Efficiency 20pts)

---

## Challenge

Write `composeServicesSummary(c)` returning sorted service names from a compose-like object.

**Example:**
```
composeServicesSummary({services:{api:{},web:{},db:{}}}) -> ['api','db','web']
```

---

## Prompt

**Goal:**
Write `composeServicesSummary(c)` returning sorted array of service names.

**Constraints:**
Extract keys from `c.services`; sort alphabetically.

**Edge Cases:**
Empty `services:{}` → `[]`.

**Output Format:**
`function composeServicesSummary(c){return Object.keys(c.services).sort()}`

---

## Scoring Strategy

| Factor | Strategy |
|---|---|
| **Prompt Quality (60pts)** | All 4 required sections present |
| **Correctness (20pts)** | Exact function name; sorted string array matches |
| **Efficiency (20pts)** | Solution embedded in Output Format — near-zero extra tokens |

---

## Notes

- Platform runs JS tests — use JS syntax
- `Object.keys().sort()` default sort is lexicographic (alphabetical for strings) — matches requirement
- One-liner keeps generated code tokens minimal
