# Day 6 — Next.js Health Payload

**Difficulty:** Easy
**Type:** Next.js / TypeScript
**Scoring:** Weighted (Prompt Quality 60pts | Correctness 20pts | Efficiency 20pts)

---

## Challenge

Write `apiHealthPayload` that returns `{status:'ok',service,version}`.

**Example:**
```
apiHealthPayload('ramadan-api','1.0.0') -> {status:'ok',service:'ramadan-api',version:'1.0.0'}
```

---

## Prompt

**Goal:**
Write `apiHealthPayload(service,version)` returning health object with fixed status `'ok'`.

**Constraints:**
- Two string params: `service`, `version`
- `status` always `'ok'`

**Edge Cases:**
- Any string inputs pass through unchanged

**Output Format:**
- `function apiHealthPayload(service,version){return{status:'ok',service,version};}`

---

## Scoring Strategy

| Factor | Strategy |
|---|---|
| **Prompt Quality (60pts)** | All 4 required sections present |
| **Correctness (20pts)** | Exact function name, correct return shape |
| **Efficiency (20pts)** | Solution embedded in Output Format — generated code is one-liner |
