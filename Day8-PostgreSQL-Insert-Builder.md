# Day 8 — PostgreSQL Insert Query Builder

**Difficulty:** Easy
**Type:** PostgreSQL / JavaScript
**Scoring:** Weighted (Prompt Quality 60pts | Correctness 20pts | Efficiency 20pts)

---

## Challenge

Write `buildStudentsInsertSQL(id, name, email)` returning a PostgreSQL INSERT string for one student row.

**Example:**
```
buildStudentsInsertSQL(1,'Sara','sara@giaic.com') -> "insert into students (id,name,email) values (1,'Sara','sara@giaic.com');"
```

---

## Prompt

**Goal:**
Return SQL insert string for students table row.

**Constraints:**
Lowercase SQL; no spaces in column/value lists.

**Edge Cases:**
id unquoted; name/email single-quoted.

**Output Format:**
`function buildStudentsInsertSQL(id,name,email){return \`insert into students (id,name,email) values (${id},'${name}','${email}');\`;}`

---

## Scoring Strategy

| Factor | Strategy |
|---|---|
| **Prompt Quality (60pts)** | All 4 required sections present |
| **Correctness (20pts)** | Exact function name; output matches expected string exactly |
| **Efficiency (20pts)** | Solution embedded in Output Format — generated code is one-liner, near-zero extra tokens |
