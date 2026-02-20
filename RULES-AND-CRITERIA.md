# Ramadan Prompting Nights — Rules & Criteria

> Scenario-based prompting competition by **Asharib Ali** for GIAIC Students.
> **30 nights. 30 real-world coding scenarios.**

---

## How to Participate

1. **Write a Structured Prompt** — using all four required components (see below)
2. **Run Tests** — validate AI-generated code against the challenge's test cases
3. **Submit** — scored if code passes

---

## Required Prompt Structure

Every prompt **must** include all four sections to achieve the maximum quality score:

| Section | Description |
|---|---|
| **Goal** | What the code/function should accomplish |
| **Constraints** | Limitations, boundaries, or rules the solution must follow |
| **Edge Cases** | Special or boundary inputs the code must handle correctly |
| **Output Format** | Expected return type, shape, and function name |

---

## Scoring System (Total: 100 points)

| Category | Weight | How It's Measured |
|---|---|---|
| **Prompt Quality** | 60 pts | Structured use of all four sections (Goal, Constraints, Edge Cases, Output Format) |
| **Correctness** | 20 pts | All tests pass, function name matches, output format matches |
| **Efficiency** | 20 pts | Fewer total tokens (prompt tokens + generated code tokens) = higher score |

### Scoring Formula

```
Final Score = (Prompt Quality % × 60) + (Correctness % × 20) + (Efficiency % × 20)
```

### Example Calculation

| Component | Raw Score | Weighted Score |
|---|---|---|
| Prompt Quality | 85/100 | 85% × 60 = **51 pts** |
| Correctness | 100/100 | 100% × 20 = **20 pts** |
| Efficiency | 80/100 | 80% × 20 = **16 pts** |
| **Final Score** | | **87 / 100** |

---

## Correctness Criteria

Code is marked correct only when **all three** of the following are true:

- All test cases pass
- The function name matches the required name exactly
- The output format/shape matches the expected output exactly

---

## Efficiency Criteria

- **Token count = prompt tokens + generated code tokens**
- Example: 42 prompt tokens + 74 code tokens = 116 total tokens
- Lower total token count → higher efficiency score

---

## Key Rules

- Prompts **must** include all four structural elements (Goal, Constraints, Edge Cases, Output Format) for maximum quality score
- Generated code must use the **exact required function name** specified in the challenge
- Output must match the **expected shape/format** precisely
- Scores are tracked on a public leaderboard

---

## Platform

- Website: [https://prompting.asharib.xyz/](https://prompting.asharib.xyz/)
- Built with Next.js + Clerk authentication
- Leaderboard available at `/leaderboard`
