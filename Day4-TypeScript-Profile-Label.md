# Day 4 — TypeScript Profile Label

**Difficulty:** Easy
**Type:** TypeScript / Logic
**Scoring:** Weighted (Prompt Quality 60pts | Correctness 20pts | Efficiency 20pts)

---

## Challenge

Write a TypeScript function `typedProfileSummary` that returns `"<name> (<role>)"`. If role is missing, use `Student`.

**Example:**
```
typedProfileSummary({name:"Aisha",role:"Mentor"}) -> "Aisha (Mentor)"
typedProfileSummary({name:"Ali"}) -> "Ali (Student)"
```

---

## Prompt

**Goal:**
Write TypeScript `typedProfileSummary` returning `"<name> (<role>)"` string from a profile object.

**Constraints:**
- Input object: `name: string`, optional `role?: string`
- Default role is `"Student"` when absent

**Edge Cases:**
- `role` missing/undefined → use `"Student"`
- `role` present → use as-is

**Output Format:**
- Function: `typedProfileSummary({name, role="Student"}: {name:string,role?:string}): string`
- Returns: `` `${name} (${role})` ``
- Example: `typedProfileSummary({name:"Aisha",role:"Mentor"})` → `"Aisha (Mentor)"`

---

## Scoring Strategy

| Factor | Strategy |
|---|---|
| **Prompt Quality (60pts)** | All 4 required sections present, clear and structured |
| **Correctness (20pts)** | Exact function name, correct return shape, example matches expected output |
| **Efficiency (20pts)** | Full implementation embedded in Output Format — generated code is one-liner |
