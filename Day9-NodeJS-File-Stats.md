# Day 9 — Node.js File Stats

**Difficulty:** Easy
**Type:** Node.js / JavaScript
**Scoring:** Weighted (Prompt Quality 60pts | Correctness 20pts | Efficiency 20pts)

---

## Challenge

Write `nodeFileStats(s)` returning `{lines, words}` for a text block.

**Example:**
```
nodeFileStats('a b\nc d e') -> {lines:2, words:5}
```

---

## Prompt

**Goal:**
`nodeFileStats(s)` returns `{lines,words}` count from string.

**Constraints:**
Split `\n` for lines; whitespace for words.

**Edge Cases:**
Empty string → `{lines:0,words:0}`.

**Output Format:**
`const nodeFileStats=s=>({lines:s?s.split('\n').length:0,words:s.trim().split(/\s+/).filter(Boolean).length})`

---

## Scoring Strategy

| Factor | Strategy |
|---|---|
| **Prompt Quality (60pts)** | All 4 required sections present |
| **Correctness (20pts)** | Exact function name; `{lines,words}` shape matches |
| **Efficiency (20pts)** | Solution embedded in Output Format — AI regenerates one-liner, near-zero extra tokens |
