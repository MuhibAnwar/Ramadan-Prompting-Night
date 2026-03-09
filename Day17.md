# Day 17 — Full-Stack Notes Transformer

**Difficulty:** Medium
**Type:** Next.js full stack (JS tests on platform)
**Scoring:** Weighted (Prompt Quality 60pts | Correctness 20pts | Efficiency 20pts)

---

## Challenge

Write `notesApiTransform(n)` converting note strings to `{id,text}` objects with ids starting at 1.

**Example:**
```
notesApiTransform(['a','b']) -> [{id:1,text:'a'},{id:2,text:'b'}]
```

---

## Prompt

**Goal:**
Write `notesApiTransform(n)` mapping string array to `{id,text}` objects.

**Constraints:**
`id` starts at 1, increments by 1; `text` is the original string.

**Edge Cases:**
Empty array → `[]`.

**Output Format:**
`function notesApiTransform(n){return n.map((t,i)=>({id:i+1,text:t}))}`

---

## Scoring Strategy

| Factor | Strategy |
|---|---|
| **Prompt Quality (60pts)** | All 4 required sections present |
| **Correctness (20pts)** | Exact function name; `{id,text}` shape with 1-based ids matches |
| **Efficiency (20pts)** | Solution embedded in Output Format — near-zero extra tokens |

---

## Notes

- Platform runs JS tests — use JS syntax
- `map((t,i)=>({id:i+1,text:t}))` — index is 0-based so +1 gives 1-based ids
- Empty array handled automatically by `.map()` returning `[]`
