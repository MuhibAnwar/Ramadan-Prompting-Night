# Day 11 — TypeScript Signup Validation Engine

**Difficulty:** Medium
**Type:** Frontend + TypeScript
**Scoring:** Weighted (Prompt Quality 60pts | Correctness 20pts | Efficiency 20pts)

---

## Challenge

Write `validateSignup` returning error array for missing name, invalid email, or password length < 8.

**Example:**
```
validateSignup({name:'',email:'a',password:'123'}) -> ['name required','invalid email','password too short']
```

---

## Prompt

**Goal:**
TS `validateSignup({name,email,password})` → string[] errors.

**Constraints:**
name falsy→'name required'; invalid email→'invalid email'; password.length<8→'password too short'.

**Edge Cases:**
valid→[]; multiple errors all returned in order.

**Output Format:**
`const validateSignup=({name,email,password})=>[...(!name?['name required']:[]),...(!/\S+@\S+\.\S+/.test(email)?['invalid email']:[]),...(password.length<8?['password too short']:[])];`

---

## Scoring Strategy

| Factor | Strategy |
|---|---|
| **Prompt Quality (60pts)** | All 4 required sections present |
| **Correctness (20pts)** | Exact function name `validateSignup`; returns `string[]` matching expected messages |
| **Efficiency (20pts)** | Solution embedded in Output Format — AI regenerates one-liner, near-zero extra tokens |

---

## Notes

- `!name` catches empty string `''` (falsy) for the name check
- `/\S+@\S+\.\S+/` regex catches missing `@` or domain
- Spread ternaries collect only triggered errors, preserving order: name → email → password
