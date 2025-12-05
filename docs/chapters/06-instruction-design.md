---
layout: default
title: "Chapter 6: Instruction Design Principles"
parent: "Part II: Core Frameworks"
nav_order: 6
permalink: /chapters/06-instruction-design/
---

# Chapter 6: Instruction Design Principles
{: .fs-9 }

Writing Clear, Actionable Instructions That AI Can Follow
{: .fs-6 .fw-300 }

---

## Learning Objectives

After completing this chapter, you will be able to:

1. Construct clear, unambiguous instructions
2. Apply the instruction hierarchy effectively
3. Handle ambiguity in task specifications
4. Sequence instructions for complex tasks
5. Test instructions for clarity and completeness

---

## The Role of Instructions

### What Are Instructions?

**Instructions** are the action-oriented components of a prompt that tell the AI what to do. They transform context into directed action.

### Instructions vs. Context

| Aspect | Context | Instructions |
|:-------|:--------|:-------------|
| **Purpose** | Provides background | Directs action |
| **Nature** | Descriptive | Imperative |
| **Focus** | Situation | Task |
| **Grammar** | Statements | Commands |

### Example Distinction

```markdown
CONTEXT: "We are a B2B SaaS company in the project management space.
Our target audience is mid-size professional services firms."

INSTRUCTION: "Write three value propositions highlighting time savings,
collaboration features, and integration capabilities."
```

---

## The Instruction Hierarchy

### Understanding Priority

Instructions can operate at different levels, with higher levels taking precedence:

```
┌─────────────────────────────────────────────────────────────────┐
│                   INSTRUCTION HIERARCHY                         │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  LEVEL 1: SYSTEM INSTRUCTIONS (Highest Priority)               │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │ Global behavior rules, personas, absolute constraints   │   │
│  │ "Never provide medical diagnoses"                       │   │
│  └─────────────────────────────────────────────────────────┘   │
│                              │                                  │
│                              ▼                                  │
│  LEVEL 2: TASK INSTRUCTIONS                                    │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │ Primary request, main objective                         │   │
│  │ "Analyze this dataset and identify trends"              │   │
│  └─────────────────────────────────────────────────────────┘   │
│                              │                                  │
│                              ▼                                  │
│  LEVEL 3: FORMAT INSTRUCTIONS                                  │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │ Output structure, presentation requirements             │   │
│  │ "Present findings as a numbered list"                   │   │
│  └─────────────────────────────────────────────────────────┘   │
│                              │                                  │
│                              ▼                                  │
│  LEVEL 4: STYLE INSTRUCTIONS (Lowest Priority)                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │ Tone, voice, aesthetic preferences                      │   │
│  │ "Use a professional but approachable tone"              │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

![Vertical stack diagram showing four levels of instruction hierarchy from highest to lowest priority. Level 1 (System Instructions): Deep blue box with 'HIGHEST PRIORITY' badge containing global behavior rules and absolute constraints with example 'Never provide medical diagnoses'. Level 2 (Task Instructions): Teal box for primary requests like 'Analyze this dataset and identify trends'. Level 3 (Format Instructions): Orange box for output structure requirements like 'Present findings as a numbered list'. Level 4 (Style Instructions): Gray box with 'LOWEST PRIORITY' badge for tone and voice preferences. Downward arrows connect each level showing override direction.]({{ site.baseurl }}/images/Figure_06.1.jpeg){: .img-fluid }
*Figure 6.1: The four-level instruction hierarchy showing priority order—system instructions override all others.*

### Hierarchy in Practice

When instructions conflict, higher levels override lower levels:

```markdown
System Instruction: "Always cite sources for factual claims"
Task Instruction: "Write a quick summary without citations"

Result: The AI should still cite sources (system overrides task)
```

---

## Principles of Clear Instructions

### Principle 1: Be Specific

Vague instructions invite interpretation; specific instructions direct action.

| Vague | Specific |
|:------|:---------|
| "Improve this code" | "Refactor this function to reduce cyclomatic complexity below 10" |
| "Make it better" | "Increase the click-through rate by making the CTA more prominent" |
| "Write about AI" | "Write a 500-word introduction to neural networks for college freshmen" |

### Principle 2: Use Action Verbs

Start instructions with clear action verbs:

| Weak | Strong |
|:-----|:-------|
| "You could analyze..." | "Analyze..." |
| "It would be good to..." | "Identify..." |
| "Maybe consider..." | "Evaluate..." |

### Common Action Verbs

| Category | Verbs |
|:---------|:------|
| **Creation** | Write, Create, Generate, Draft, Compose |
| **Analysis** | Analyze, Evaluate, Compare, Assess, Review |
| **Transformation** | Convert, Translate, Refactor, Simplify, Expand |
| **Organization** | List, Categorize, Rank, Prioritize, Structure |
| **Explanation** | Explain, Describe, Summarize, Clarify, Define |

### Principle 3: One Instruction, One Action

Break complex instructions into discrete steps:

```markdown
❌ COMBINED:
"Analyze the data, identify trends, create visualizations,
and write a summary report with recommendations."

✅ SEPARATED:
"1. Analyze the dataset for patterns and anomalies
2. Identify the top 3 significant trends
3. Describe appropriate visualization for each trend
4. Summarize findings in 200 words
5. Provide 3 actionable recommendations"
```

### Principle 4: Define Success Criteria

Make the goal measurable or verifiable:

```markdown
❌ UNCLEAR: "Write a good product description"

✅ CLEAR: "Write a product description that:
- Is 100-150 words
- Includes 3 key features
- Contains one compelling benefit statement
- Ends with a call-to-action"
```

---

## Handling Ambiguity

### Types of Ambiguity

| Type | Example | Solution |
|:-----|:--------|:---------|
| **Lexical** | "Fix the bug" (which bug?) | Specify the exact issue |
| **Structural** | "Fast car rental service" | Clarify: fast cars or fast service? |
| **Referential** | "Analyze it" (what's 'it'?) | Use explicit references |
| **Scope** | "Improve the design" (all of it?) | Define boundaries |

### Ambiguity Resolution Strategies

**Strategy 1: Explicit Enumeration**
```markdown
Instead of: "Handle the errors"
Use: "Handle these specific errors:
1. Network timeout (retry with exponential backoff)
2. Invalid input (return validation message)
3. Authentication failure (redirect to login)"
```

**Strategy 2: Example Clarification**
```markdown
Instead of: "Format like a professional report"
Use: "Format as a professional report:
- Title page with date and author
- Executive summary (1 page max)
- Body with numbered sections
- Appendix for detailed data

Example structure:
1. Introduction
2. Methodology
3. Findings
4. Recommendations"
```

**Strategy 3: Boundary Definition**
```markdown
Instead of: "Improve the user experience"
Use: "Improve the checkout flow user experience specifically:
- In scope: Shopping cart to payment confirmation
- Out of scope: Product browsing, account management
- Focus on: Reducing steps, clearer progress indication"
```

---

## Instruction Sequencing

### Why Sequence Matters

The order of instructions affects how AI processes and prioritizes them.

### Sequencing Principles

**Principle 1: Critical First**
Place the most important instructions early.

**Principle 2: Logical Flow**
Order instructions in the sequence they should be considered or executed.

**Principle 3: Constraints Before Actions**
State limitations before the task they constrain.

### Sequencing Example

```markdown
✅ WELL-SEQUENCED:

**Constraints (First):**
- Maximum 500 words
- No technical jargon
- Must include a real-world analogy

**Task (Second):**
Explain how blockchain works to a high school student.

**Format (Third):**
1. Opening hook (1 sentence)
2. Core explanation (3-4 paragraphs)
3. Practical example
4. Summary of key points
```

### Sequencing for Multi-Step Tasks

```markdown
STEP 1: Read and understand the provided code
↓
STEP 2: Identify potential security vulnerabilities
↓
STEP 3: Rank vulnerabilities by severity
↓
STEP 4: For the top 3 vulnerabilities:
   a. Explain the risk
   b. Show the vulnerable code
   c. Provide corrected code
↓
STEP 5: Summarize overall security posture
```

---

## Instruction Patterns

### Pattern: The Explicit Request

```markdown
[Action Verb] + [Object] + [Specifications]

"Write a function that calculates compound interest
with parameters for principal, rate, time, and compounding frequency."
```

### Pattern: The Conditional Instruction

```markdown
IF [condition] THEN [action] ELSE [alternative]

"If the input contains PII, redact it and note what was removed.
Otherwise, process the input normally."
```

### Pattern: The Prioritized List

```markdown
Complete the following in order of priority:
1. [Critical task]
2. [Important task]
3. [Nice-to-have task]

If time/space is limited, complete as many as possible starting from #1.
```

### Pattern: The Iterative Refinement

```markdown
First: Generate an initial draft
Then: Review for [criteria]
Finally: Revise to address any issues found

Show both the initial draft and final version.
```

### Pattern: The Comparative Analysis

```markdown
Compare [A] and [B] across these dimensions:
- [Dimension 1]
- [Dimension 2]
- [Dimension 3]

Present as a table, then provide a recommendation.
```

---

## Testing Your Instructions

### The Interpretation Test

Ask: "Could someone interpret this differently than I intend?"

```markdown
❌ AMBIGUOUS: "Make the button better"
Interpretations: Bigger? Different color? Different text? Different position?

✅ UNAMBIGUOUS: "Make the button more prominent by:
- Increasing size to 48px height
- Using primary brand color (#0066CC)
- Adding 'Get Started Now' as the text"
```

### The Completeness Test

Ask: "Do my instructions cover all necessary aspects?"

**Checklist:**
- [ ] What to do (task)
- [ ] How to do it (method/approach)
- [ ] What to produce (output)
- [ ] What to avoid (constraints)
- [ ] How to handle edge cases

### The Clarity Test

Ask: "Would a new team member understand this?"

```markdown
❌ INSIDER LANGUAGE:
"Use the standard TPS report format for the Q4 metrics"

✅ EXPLICIT:
"Format as a quarterly metrics report with:
- Executive summary (1 paragraph)
- KPI table (metric, target, actual, variance)
- Trend analysis (2-3 paragraphs)
- Action items (bulleted list)"
```

---

## Instruction Refinement Workflow

### The Refinement Loop

```
┌─────────────────────────────────────────────────────────────┐
│                 INSTRUCTION REFINEMENT                      │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│     ┌──────────┐                                           │
│     │  DRAFT   │ ◀───────────────────────────┐             │
│     │Instruction│                             │             │
│     └────┬─────┘                             │             │
│          │                                    │             │
│          ▼                                    │             │
│     ┌──────────┐                             │             │
│     │   TEST   │                             │             │
│     │ (Run it) │                             │             │
│     └────┬─────┘                             │             │
│          │                                    │             │
│          ▼                                    │             │
│     ┌──────────┐      ┌──────────┐          │             │
│     │ EVALUATE │─────▶│  REFINE  │──────────┘             │
│     │ Results  │ No   │ Improve  │                         │
│     └────┬─────┘      └──────────┘                         │
│          │                                                  │
│          │ Yes (Good Results)                              │
│          ▼                                                  │
│     ┌──────────┐                                           │
│     │ DOCUMENT │                                           │
│     │ & Reuse  │                                           │
│     └──────────┘                                           │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

![Circular workflow diagram showing the instruction refinement process. Five stages: Draft (light blue box for creating initial instruction) flows to Test (teal box for running the instruction) flows to Evaluate (orange diamond decision point). From Evaluate, 'No' path in red goes to Refine (red box for improvement) which loops back to Draft. 'Yes' path in green from Evaluate leads to Document & Reuse (green success box). The loop from Refine back to Draft shows the iterative nature of instruction improvement.]({{ site.baseurl }}/images/Figure_06.2.jpeg){: .img-fluid }
*Figure 6.2: The instruction refinement loop—an iterative process for improving instruction clarity through testing and evaluation.*

### Refinement Questions

After testing, ask:
1. Did the output match expectations?
2. What was missing or wrong?
3. What instruction would have prevented that?
4. Is the refined instruction still clear?

---

## Common Instruction Mistakes

### Mistake 1: Instruction Overload

**Problem:** Too many instructions overwhelm and confuse.

```markdown
❌ OVERLOADED:
"Write, edit, proofread, format, optimize for SEO, add images,
include citations, translate to Spanish, and publish the article."

✅ FOCUSED:
"Write a 1000-word article on [topic]. I'll handle editing and SEO separately."
```

### Mistake 2: Contradictory Instructions

**Problem:** Instructions conflict with each other.

```markdown
❌ CONTRADICTORY:
"Be concise. Include comprehensive details on all aspects."

✅ RESOLVED:
"Provide comprehensive details, but express each point concisely—
no filler words or redundant explanations."
```

### Mistake 3: Assuming Prior Knowledge

**Problem:** Instructions assume understanding that doesn't exist.

```markdown
❌ ASSUMES:
"Use the standard format for the client deck"

✅ EXPLICIT:
"Format as a client presentation:
- 10-15 slides
- One key point per slide
- Executive summary on slide 2
- Recommendation on final slide"
```

---

## Key Takeaways

- **Instructions direct action**; they are the imperative core of prompts
- The **instruction hierarchy** determines priority when conflicts arise
- **Specific, action-oriented** language produces better results
- **Break complex tasks** into discrete, sequential steps
- **Ambiguity is the enemy**—resolve it through explicit specification
- **Test and refine** instructions through iterative improvement

---

## Summary

Instruction design is where prompting becomes actionable. Clear, specific, well-sequenced instructions transform context and intent into directed AI behavior. By applying the principles in this chapter—specificity, action verbs, single-action steps, success criteria, and systematic ambiguity resolution—you ensure your prompts produce the outputs you actually need.

---

## Review Questions

1. What are the four levels of the instruction hierarchy?
2. Why should complex instructions be broken into discrete steps?
3. What are three strategies for resolving ambiguity?
4. How does instruction sequencing affect AI output?
5. What three tests can you apply to evaluate instruction clarity?

---

## Practical Exercise

**Exercise 6.1: Instruction Improvement**

Take this vague instruction and improve it:
"Help me with my presentation"

Improved version should include:
- Specific action verbs
- Clear deliverables
- Format specifications
- Success criteria

**Exercise 6.2: Instruction Sequencing**

Given this task: "Create a marketing email campaign for a product launch"

Write sequenced instructions that:
1. Define the task hierarchy
2. Break into logical steps
3. Include constraints
4. Specify output format

---

## Chapter Navigation

| Previous | Up | Next |
|:---------|:---|:-----|
| [← Chapter 5: Context Engineering]({{ site.baseurl }}/chapters/05-context-engineering/) | [Part II: Core Frameworks]({{ site.baseurl }}/part-ii-core-frameworks/) | [Chapter 7: Output Specification →]({{ site.baseurl }}/chapters/07-output-specification/) |
