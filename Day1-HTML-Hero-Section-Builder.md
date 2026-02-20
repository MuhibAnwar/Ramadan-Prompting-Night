# Day 1 — HTML Hero Section Builder

**Difficulty:** Easy
**Type:** Frontend / HTML-CSS
**Scoring:** Weighted (Prompt Quality 60pts | Correctness 20pts | Efficiency 20pts)

---

## Challenge

Write a function `renderRamadanHero` that returns a semantic HTML string with a title and CTA button.

**Example:**
```
renderRamadanHero("Ramadan Prompting Nights", "Join Now")
// → "<section><h1>Ramadan Prompting Nights</h1><button>Join Now</button></section>"
```

---

## Prompt

**Goal:**
Write a JavaScript function `renderRamadanHero(title, cta)` that returns a semantic HTML string containing the title in an `<h1>` and CTA in a `<button>`, wrapped in a `<section>`.

**Constraints:**
- Function name must be exactly `renderRamadanHero`
- Return a plain string; no DOM manipulation
- No extra whitespace, classes, or attributes in the HTML
- Output structure must be: `<section><h1>{title}</h1><button>{cta}</button></section>`

**Edge Cases:**
- Empty string inputs should still return valid HTML with empty tags
- Do not escape or modify the input strings

**Output Format:**
```js
function renderRamadanHero(title, cta) {
  return `<section><h1>${title}</h1><button>${cta}</button></section>`;
}
```

---

## Scoring Strategy

| Factor | Strategy |
|---|---|
| **Prompt Quality (60pts)** | All 4 required sections present, clear and structured |
| **Correctness (20pts)** | Exact function name and output shape explicitly specified |
| **Efficiency (20pts)** | Minimal tokens — no fluff, no repeated scenario text |
