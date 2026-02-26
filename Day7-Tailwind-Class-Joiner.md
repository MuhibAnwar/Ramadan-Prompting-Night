# Day 7 — Tailwind Class Joiner

**Difficulty:** Easy
**Type:** JavaScript
**Scoring:** Weighted (Prompt Quality 60pts | Correctness 20pts | Efficiency 20pts)

---

## Challenge

Write `tailwindClassMerger` that joins only truthy class names with a single space.

**Example:**
```
tailwindClassMerger(['p-4','','bg-black',null,'text-white']) -> "p-4 bg-black text-white"
```

---

## Prompt

**Goal:**
Filter array, join truthy items with `' '`.

**Constraints:**
- Array of strings/nulls/falsy

**Edge Cases:**
- Empty string, `null` → excluded

**Output Format:**
`function tailwindClassMerger(c){return c.filter(Boolean).join(' ');}`

---

## Scoring Strategy

| Factor | Strategy |
|---|---|
| **Prompt Quality (60pts)** | All 4 required sections present |
| **Correctness (20pts)** | Exact function name, returns joined string |
| **Efficiency (20pts)** | Solution embedded in Output Format — generated code is one-liner |
