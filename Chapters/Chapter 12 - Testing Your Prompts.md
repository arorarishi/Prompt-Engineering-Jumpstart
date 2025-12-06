# **Chapter 12 — Testing Your Prompts**

## _“A prompt is only good if it works every time — not just once.”_

---

## 🎯 **Why This Chapter Matters**

Most people treat prompting like magic.
Professionals treat prompting like **engineering**.

And engineering means **testing**.

This chapter teaches you how to:

- validate whether your prompt is reliable
- check for inconsistencies
- catch hidden failure modes
- stress-test your prompt across variations
- make your outputs stable and predictable

If you want your prompts to work for **clients**, **teams**, or **automation**, this is a mandatory skill.

---

## 🧪 **SECTION 1: The Three Types of Prompt Tests**

To test a prompt properly, you must evaluate:

- **1. Reliability**
  Does it give consistent results across multiple runs?

- **2. Accuracy**
  Does it correctly use the context and instructions?

- **3. Robustness**
  Does it remain stable even if inputs change slightly?

Most prompts fail on **robustness**, not accuracy.

---

## 🔄 **SECTION 2: The Reliability Test**

Run the exact same prompt **3–5 times**.
Check if the outputs are:

- structurally consistent
- stylistically consistent
- respecting all constraints

### ✔ Good sign

All runs follow the same format and rules.

### ❌ Red flags

- missing sections
- random deviations
- unexpected tone changes

### Template:

```
Run this prompt 3 times and compare all outputs.
Identify inconsistencies, tone shifts, or rule violations.
```

---

## 🎯 **SECTION 3: The Accuracy Test**

Accuracy = Did the model follow your instructions _exactly_?

Check for:

- hallucinated facts
- missing constraints
- ignored examples
- deviations from required format
- wrong tone

### Quick checklist:

✔ Did it use the context?
✔ Did it avoid adding new information?
✔ Did it follow the structure exactly?

### Template:

```
Evaluate if this output follows ALL instructions.
List:
- Correct behaviors
- Missed instructions
- Violations
```

---

## 🛡️ **SECTION 4: The Robustness Test (Most Important)**

This test simulates **real-world messy inputs**.

### You test your prompt by giving:

- longer input
- shorter input
- slightly ambiguous input
- noisy input
- edge-case input

This is where weak prompts break.

### Example variations:

- missing fields
- typos
- incomplete sentences
- unexpected formatting

### Template:

```
Test this prompt with:
1. Long input
2. Short input
3. Messy or noisy input
4. Edge-case input

List where the prompt breaks and how to improve it.
```

---

## 🧩 **SECTION 5: Stress Testing with Adversarial Inputs**

This is pro-level validation.

Introduce **slight distortions** and see if your instructions still hold.

Examples:

- give it a tricky paragraph
- add contradictory statements
- include irrelevant details
- remove punctuation
- test with different languages

### Goal:

See if the prompt **prioritizes the right rules** without getting confused.

---

## 🔧 **SECTION 6: A/B Testing Your Prompt**

Compare two versions of a prompt:

- Version A: simple
- Version B: structured
- Version C: with examples

Ask the model:

```
Compare the performance of Prompt A and Prompt B.
Which one:
- follows instructions better?
- gives fewer hallucinations?
- has clearer structure?
```

This is how you quickly find the winning design.

---

## 🧠 **SECTION 7: The “Minimum Effective Prompt” Check**

A strong prompt is **simple but powerful**.

After building a prompt, always ask:

```
Remove 20% of the prompt.
Did anything break?
```

If yes → too fragile
If no → more efficient

This helps prevent bloated prompts.

---

## 📐 **SECTION 8: Scoring Your Prompt (The 10-Point Framework)**

Score each output on:

| Criteria                | Score (1–10) |
| ----------------------- | ------------ |
| Followed instructions   | ⬜           |
| Accuracy                | ⬜           |
| Structure               | ⬜           |
| Tone                    | ⬜           |
| Robustness              | ⬜           |
| No hallucination        | ⬜           |
| Completeness            | ⬜           |
| Clarity                 | ⬜           |
| Consistency across runs | ⬜           |
| Overall usefulness      | ⬜           |

A production-ready prompt should score **8/10 or higher**.

---

## 🧭 **SECTION 9: The “Golden Validation Prompt”**

Use this meta-prompt to test ANY prompt:

```
Review the following prompt as if you are a prompt engineer.

Evaluate:
1. Completeness
2. Clarity
3. Constraint strength
4. Potential failure modes
5. Robustness
6. Hallucination risks

Provide a score from 1–10 and recommendations for improvement.

Prompt:
[PASTE YOUR PROMPT HERE]
```

This is a powerful automatic evaluator.

---

## 📌 **Chapter Summary**

You learned how to:

- test for reliability
- test for accuracy
- test for robustness
- stress-test with messy inputs
- run A/B comparisons
- evaluate a prompt with the 10-point framework
- simplify and strengthen prompts

Testing transforms a prompt from “works once” → **works every time**.

---

## 🎯 **Exercises**

1. Take any prompt from earlier chapters → test it 3 times.
2. Break your prompt deliberately → fix it.
3. A/B test two designs for the same task.
4. Apply the 10-point scoring system.

---
