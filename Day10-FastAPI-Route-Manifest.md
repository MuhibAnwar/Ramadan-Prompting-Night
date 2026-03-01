# Day 10 — FastAPI Route Manifest

**Difficulty:** Easy
**Type:** JavaScript (FastAPI scenario)
**Scoring:** Weighted (Prompt Quality 60pts | Correctness 20pts | Efficiency 20pts)

---

## Challenge

Write `fastapiRouteMap(names)` returning an array of route objects from names list using GET method.

**Example:**
```
fastapiRouteMap(['health','users']) -> [{path:'/health',method:'GET'},{path:'/users',method:'GET'}]
```

---

## Prompt

**Goal:**
Write `fastapiRouteMap(names)` returning route objects array.

**Constraints:**
path=`'/'+name`, method=`'GET'`.

**Edge Cases:**
Empty array → `[]`.

**Output Format:**
`function fastapiRouteMap(names){return names.map(n=>({path:'/'+n,method:'GET'}))}`

---

## Scoring Strategy

| Factor | Strategy |
|---|---|
| **Prompt Quality (60pts)** | All 4 required sections present |
| **Correctness (20pts)** | Exact function name; `{path,method}` shape matches |
| **Efficiency (20pts)** | Solution embedded in Output Format — AI regenerates one-liner, near-zero extra tokens |

---

## Notes

- Platform runs JS tests despite "Python/FastAPI" label — use JS syntax
- First attempt used Python `def` syntax → failed with "Unexpected identifier" JS error
