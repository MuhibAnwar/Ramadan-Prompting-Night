# Day 18 — Theme Preference Resolver

**Difficulty:** Medium
**Type:** Frontend Tailwind (JS tests on platform)
**Scoring:** Weighted (Prompt Quality 60pts | Correctness 20pts | Efficiency 20pts)

---

## Challenge

Write `themePreference(u,s)` returning user preference if valid (`light`/`dark`), else system preference.

**Example:**
```
themePreference('dark','light') -> 'dark'
```

---

## Prompt

**Goal:**
Write `themePreference(u,s)` returning `u` if valid, else `s`.

**Constraints:**
Valid values are `'light'` or `'dark'` only.

**Edge Cases:**
Invalid/unknown `u` → return `s`.

**Output Format:**
`function themePreference(u,s){return['light','dark'].includes(u)?u:s}`

---

## Scoring Strategy

| Factor | Strategy |
|---|---|
| **Prompt Quality (60pts)** | All 4 required sections present |
| **Correctness (20pts)** | Exact function name; returns correct string value |
| **Efficiency (20pts)** | Solution embedded in Output Format — near-zero extra tokens |

---

## Notes

- `['light','dark'].includes(u)` cleanly validates both allowed values in one check
- Invalid `u` (null, undefined, 'system', etc.) falls through to `s`
