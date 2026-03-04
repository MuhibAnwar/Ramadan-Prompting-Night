# Day 12 — React Dashboard Widget Mapper

**Difficulty:** Medium
**Type:** React / Next.js
**Scoring:** Weighted (Prompt Quality 60pts | Correctness 20pts | Efficiency 20pts)

---

## Challenge

Write `dashboardCardLayout` to map metric values into standardized card objects `{label,value,trend}`.

**Example:**
```
dashboardCardLayout({users:20,active:16}) -> [{label:'users',value:20,trend:'up'},{label:'active',value:16,trend:'up'}]
```

---

## Prompt

**Goal:**
Return JS-notation string [{label,value,trend}] per metric.

**Constraints:**
trend:'up'(>0),'down'(<0),'neutral'(=0).

**Edge Cases:**
0→neutral,{}→'[]'.

**Output Format:**
`function dashboardCardLayout(o){return '['+Object.entries(o).map(([l,v])=>"{label:'"+l+"',value:"+v+",trend:'"+(v>0?'up':v<0?'down':'neutral')+"'}").join(',')+']'}`

---

## Scoring Strategy

| Factor | Strategy |
|---|---|
| **Prompt Quality (60pts)** | All 4 required sections present |
| **Correctness (20pts)** | Exact function name `dashboardCardLayout`; returns JSON string matching expected shape |
| **Efficiency (20pts)** | Solution embedded in Output Format — AI regenerates one-liner, near-zero extra tokens |

---

## Notes

- Initial attempt returned an array — tests failed with `[object Object],[object Object]` (string coercion by test runner)
- Fix: wrap result in `JSON.stringify(...)` to return a string
- `value>0` handles both zero and negatives as `'down'`
- `Object.entries` preserves insertion order of keys
