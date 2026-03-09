# Day 15 — FastAPI Task Payload Normalizer

**Difficulty:** Medium
**Type:** Python/FastAPI (JS tests on platform)
**Scoring:** Weighted (Prompt Quality 60pts | Correctness 20pts | Efficiency 20pts)

---

## Challenge

Write `taskCrudPayload(t)` normalizing task input to `{title,done}` with default `done:false`.

**Example:**
```
taskCrudPayload({title:'Review PR'}) -> {title:'Review PR',done:false}
```

---

## Prompt

**Goal:**
Write `taskCrudPayload(t)` returning normalized `{title,done}` object.

**Constraints:**
`done` defaults to `false` if missing/undefined.

**Edge Cases:**
`done:true` preserved; missing `done` → `false`.

**Output Format:**
`function taskCrudPayload(t){return{title:t.title,done:t.done??false}}`

---

## Scoring Strategy

| Factor | Strategy |
|---|---|
| **Prompt Quality (60pts)** | All 4 required sections present |
| **Correctness (20pts)** | Exact function name; `{title,done}` shape matches |
| **Efficiency (20pts)** | Solution embedded in Output Format — AI regenerates one-liner, near-zero extra tokens |

---

## Notes

- Platform runs JS tests despite "Python/FastAPI" label — use JS syntax (confirmed from Day 10)
- `??` (nullish coalescing) handles `undefined`/`null` for `done`, while preserving explicit `false`
- One-liner keeps generated code tokens minimal
