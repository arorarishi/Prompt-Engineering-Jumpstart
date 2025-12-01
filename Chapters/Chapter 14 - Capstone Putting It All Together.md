# **Chapter 14 — Capstone: Putting It All Together**

- [**Chapter 14 — Capstone: Putting It All Together**](#chapter-14--capstone-putting-it-all-together)
  - [_“One final prompt that uses EVERYTHING you’ve learned — and a real scenario to prove it works.”_](#one-final-prompt-that-uses-everything-youve-learned--and-a-real-scenario-to-prove-it-works)
- [🎯 **Why This Chapter Exists**](#-why-this-chapter-exists)
- [🏗️ **SECTION 1 — The Master Prompt Blueprint**](#️-section-1--the-master-prompt-blueprint)
- [🧪 **SECTION 2 — The Real Scenario Walkthrough**](#-section-2--the-real-scenario-walkthrough)
  - [_Scenario: Create a Market Research Summary for a New Fitness App_](#scenario-create-a-market-research-summary-for-a-new-fitness-app)
  - [**Step 1 — Define the Role**](#step-1--define-the-role)
  - [**Step 2 — Define the Goal + Success Criteria**](#step-2--define-the-goal--success-criteria)
  - [**Step 3 — Provide Context**](#step-3--provide-context)
  - [**Step 4 — Add Few-Shot Examples**](#step-4--add-few-shot-examples)
  - [**Step 5 — Add Thinking Instructions**](#step-5--add-thinking-instructions)
  - [**Step 6 — Add Structure**](#step-6--add-structure)
  - [**Step 7 — Add Constraints and Negative Rules**](#step-7--add-constraints-and-negative-rules)
  - [**Step 8 — Add Uncertainty Handling**](#step-8--add-uncertainty-handling)
  - [**Step 9 — Add Iteration Loop**](#step-9--add-iteration-loop)
- [🎉 **SECTION 3 — Final Combined Prompt (Capstone Prompt)**](#-section-3--final-combined-prompt-capstone-prompt)
- [🔍 **SECTION 4 — Before/After Comparison**](#-section-4--beforeafter-comparison)
  - [❌ **Before (Normal User Prompt)**](#-before-normal-user-prompt)
  - [✅ **After (Capstone Prompt)**](#-after-capstone-prompt)
- [🏁 **SECTION 5 — Chapter Summary**](#-section-5--chapter-summary)

## _“One final prompt that uses EVERYTHING you’ve learned — and a real scenario to prove it works.”_

---

# 🎯 **Why This Chapter Exists**

You’ve learned:

- how to give roles
- how to be specific
- how to use few-shot examples
- how to trigger reasoning
- how to control output
- how to iterate
- how to use negative prompting
- how to chain tasks
- how to test your prompts
- how to avoid hallucinations

Now you will combine **all of them** into:

1. A **Master Prompt Template**
2. A **Real-World Scenario Walkthrough**
3. A **Before/After Comparison**
4. A **Ready-to-use Capstone Prompt**

This chapter gives readers **the final skill**:
👉 Prompt engineering as a repeatable system.

---

# 🏗️ **SECTION 1 — The Master Prompt Blueprint**

Below is the “lego-block” master structure. This is the _ultimate_ prompt template your readers will use everywhere.

```
You are a [ROLE].

Your goal: [OBJECTIVE].
Success criteria:
- [criterion 1]
- [criterion 2]
- [criterion 3]

Context:
[CONTEXT BLOCK]

Follow these examples:
[FEW-SHOT EXAMPLES]

Thinking instructions:
Think step-by-step.
Check for missing information.
If unclear, ask for clarification before answering.

Output format:
[STRUCTURED FORMAT]

Constraints:
- Do NOT add information outside context.
- Do NOT assume.
- Do NOT hallucinate.
- Follow the format EXACTLY.

Negative rules:
What NOT to do:
- Do not invent details.
- Do not change meaning.
- Do not expand beyond scope.

Uncertainty handling:
If unsure, say:
“I don’t know based on the given information.”

Iteration loop:
At the end, ask:
“Would you like a refinement or variation?”
```

This template is your **Capstone Formula**.

---

# 🧪 **SECTION 2 — The Real Scenario Walkthrough**

## _Scenario: Create a Market Research Summary for a New Fitness App_

Users learn best when they see how theory becomes _results_.
So let’s apply the master template step by step.

---

## **Step 1 — Define the Role**

```
You are a senior market research analyst.
```

---

## **Step 2 — Define the Goal + Success Criteria**

```
Your goal is to create a market research summary for a new fitness app.

Success criteria:
- Summarize the market clearly
- Identify trends and competitors
- Provide actionable insights
```

---

## **Step 3 — Provide Context**

```
Context:
The app target audience: 18–40
Region: US & India
Category: home workout + diet tracking
```

---

## **Step 4 — Add Few-Shot Examples**

```
Example:
“Competitor analysis: Peloton — premium hardware-based workout ecosystem…”
```

(Only one example is enough.)

---

## **Step 5 — Add Thinking Instructions**

```
Think step-by-step.
Validate assumptions.
Ask for clarification if information is missing.
```

---

## **Step 6 — Add Structure**

```
Output format:
1. Market Overview
2. Trends
3. Competitor Breakdown
4. Opportunities
5. Risks
6. Final Recommendation
```

---

## **Step 7 — Add Constraints and Negative Rules**

```
Constraints:
- Use only info from context
- Do not hallucinate
- Do not guess data

What NOT to do:
- Don’t include statistics not provided
- Don’t change the target audience
- Don’t expand into irrelevant markets
```

---

## **Step 8 — Add Uncertainty Handling**

```
If any data is missing, explicitly state it.
```

---

## **Step 9 — Add Iteration Loop**

```
At the end, ask:
“Would you like deeper analysis or another version?”
```

---

# 🎉 **SECTION 3 — Final Combined Prompt (Capstone Prompt)**

Here is the final prompt that merges all steps into one:

```
You are a senior market research analyst.

Your goal is to create a market research summary for a new fitness app.

Success criteria:
- Summarize the market clearly
- Identify emerging trends
- Analyze competitors
- Provide actionable insights

Context:
The app target audience: 18–40
Regions: US & India
Category: home workout + diet tracking

Example:
Competitor analysis format —
“Competitor: Peloton — premium hardware-based workout ecosystem…”

Thinking instructions:
Think step-by-step.
Check for missing information.
If unclear, ask for clarification before answering.

Output format:
1. Market Overview
2. Trends
3. Competitor Breakdown
4. Opportunities
5. Risks
6. Final Recommendation

Constraints:
- Use ONLY the context above
- Do NOT add external data
- Do NOT guess statistics
- Follow the structure EXACTLY

What NOT to do:
- Do not invent details
- Do not change meaning
- Do not expand beyond scope

Uncertainty handling:
If unsure, say:
“I don’t know based on the given information.”

Iteration:
At the end ask:
“Would you like deeper analysis or another version?”
```

This is the **final master prompt** that uses all 13 chapters.

---

# 🔍 **SECTION 4 — Before/After Comparison**

## ❌ **Before (Normal User Prompt)**

“Do market research for my new fitness app.”

Problems:

- vague
- no structure
- no context
- high hallucination risk

## ✅ **After (Capstone Prompt)**

- role
- objective
- context
- examples
- reasoning
- negative rules
- testing elements
- structure
- uncertainty handling

Everything becomes **professional, predictable, powerful**.

---

# 🏁 **SECTION 5 — Chapter Summary**

This capstone chapter taught you how to:

- assemble all earlier skills into one layered prompt
- use structure, examples, context, roles, constraints
- build a master template you can reuse forever
- apply it to a real scenario
- understand before/after transformations
- create prompts that work in any domain

This is the moment where your prompting becomes **engineering**.

---
