# **Chapter 13 — Avoiding Bad Answers (Limitations)**

## _“Good prompting is not only about getting great outputs — it’s also about preventing bad ones.”_

---

## 🎯 **Why This Chapter Matters**

LLMs are powerful, but they are not magical.
They have very real limitations:

- they hallucinate
- they misunderstand vague inputs
- they invent details when the context is weak
- they overconfidently guess
- they sometimes ignore constraints

This chapter teaches you how to **design prompts that avoid bad answers**, prevent mistakes, and minimize hallucinations.

If Chapters 1–12 taught you how to **get good answers**,
Chapter 13 teaches you how to **block the bad ones**.

---

## 🚫 **SECTION 1: The 5 Causes of Bad Answers**

LLMs typically fail because of:

**1. Missing context**
The model fills in gaps with imagination.

**2. Ambiguous questions**
Vague input → vague output.

**3. Overbroad instructions**
General prompts lead to generic answers.

**4. Incorrect assumptions by user**
Models “follow the user’s lead,” even if wrong.

**5. Hallucinations under pressure**
When forced to “give an answer,” the model makes one up.

---

## 🧨 **SECTION 2: The Anti-Hallucination Toolkit**

These simple additions dramatically improve accuracy.

- **1. The “Don’t Make Stuff Up” Clause**

```
If the answer is not in the context, say “I don’t know based on the given information.”
```

- **2. Source Enforcement**

```
Support every claim with text directly from the provided context.
If the context does not support it, exclude it.
```

- **3. Uncertainty Prompting**

```
If uncertain, provide the most likely answer and state your level of confidence.
```

- **4. Proof Requirement**

```
Explain why your answer is correct using the available context only.
```

These four lines eliminate 70% of hallucinations.

---

## 🔍 **SECTION 3: The “Clarify Before Answering” Pattern**

When the user’s input is risky, the model should ask for clarification.

Add:

```
If the question is ambiguous, ask for clarification before answering.
```

This prevents:

- wrong assumptions
- incorrect interpretations
- irrelevant answers

---

## 🧱 **SECTION 4: Boundary Setting**

Tell the model what to **avoid**.

Examples:

```
Do not add examples unless I ask.
Do not assume missing data.
Do not guess names, values, or statistics.
Do not expand or summarize unless instructed.
Do not include external knowledge.
```

Boundary setting = cleaner + safer outputs.

---

## 🧠 **SECTION 5: The “What You Should NOT Do” Block**

Humans respond better when we hear what not to do.
LLMs work the same way.

Add a block like this:

```
What NOT to do:
- Do NOT guess.
- Do NOT invent details.
- Do NOT change the meaning.
- Do NOT add new assumptions.
```

This noticeably sharpens precision.

---

## 🧩 **SECTION 6: Limitation Acknowledgment Prompt**

If the model is likely to struggle, pre-empt the weakness:

```
Before answering, identify any limitations or missing information that affect accuracy.
```

This forces the model to:

- slow down
- think critically
- disclose uncertainty
- reduce hallucinations

---

## 📚 **SECTION 7: Context anchoring**

When using documents / PDFs / transcripts:

```
Cite the exact sentence from context that supports your answer.
```

This locks the model into the text.

---

## 🎛️ **SECTION 8: Output Tuning to Avoid Messy Answers**

Messy answers are a sign of weak prompting.

You can fix this with:

- **✔ Strict formatting**
- **✔ Smaller scope**
- **✔ Precise instructions**
- **✔ Example-based prompting**
- **✔ Step-by-step constraints**

Example:

```
Answer using ONLY this format:
1. What is known
2. What is unknown
3. Final answer
```

---

## 🧪 **SECTION 9: Test Your Prompt Against Failure Modes**

Use the following checklist:

- **Accuracy Risks** - Does the prompt prevent hallucination? - Does it restrict assumptions?
- **Clarity Risks** - Is the task defined clearly? - Are boundaries explicit?
- **Robustness Risks** - Does the prompt survive messy input? - Does it detect missing information?
- **Safety Risks** - Does it avoid biased or harmful outputs?

This is where Chapter 12 aligns with Chapter 13.

---

## 🎯 **Exercises**

1. Take a vague prompt → add anti-hallucination rules.
2. Take a failing prompt → add a “What NOT to do” block.
3. Take a complex question → add a clarify-before-answer clause.
4. Test your improved prompt with noisy input.

---

## 📌 **Summary Chapter 13 — Avoiding Bad Answers**

You learned techniques to avoid bad answers by controlling:

- context
- assumptions
- boundaries
- uncertainty
- hallucinations
- output constraints

Good prompts don’t just make the model produce great results—
they **protect you from mistakes**.

---
