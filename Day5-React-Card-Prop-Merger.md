# Day 5 — React Card Prop Merger

**Difficulty:** Easy
**Type:** React / JavaScript
**Scoring:** Weighted (Prompt Quality 60pts | Correctness 20pts | Efficiency 20pts)

---

## Challenge

Write `mergeCardProps` to merge default and custom props. Custom values override defaults.

**Example:**
```
mergeCardProps({title:'Day 1',badge:'Easy'},{badge:'Done'}) -> {title:'Day 1',badge:'Done'}
```

---

## Prompt

**Goal:**
Write `mergeCardProps` that merges two card prop objects, custom overrides defaults.

**Constraints:**
- Two params: `defaults` object, `custom` object
- Custom values take priority over defaults
- Do not mutate either input

**Edge Cases:**
- `custom` empty → return copy of `defaults`
- `defaults` empty → return copy of `custom`
- Overlapping keys → `custom` value wins

**Output Format:**
- Function: `function mergeCardProps(defaults, custom) { return {...defaults, ...custom}; }`
- Returns: merged plain object
- Example: `mergeCardProps({title:'Day 1',badge:'Easy'},{badge:'Done'})` → `{title:'Day 1',badge:'Done'}`

---

## Scoring Strategy

| Factor | Strategy |
|---|---|
| **Prompt Quality (60pts)** | All 4 required sections present, clear and structured |
| **Correctness (20pts)** | Exact function name, correct return shape, example matches expected output |
| **Efficiency (20pts)** | Implementation embedded in Output Format — generated code is one-liner |
