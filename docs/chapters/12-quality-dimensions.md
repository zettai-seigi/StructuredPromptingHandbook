---
layout: default
title: "Chapter 12: Prompt Quality Dimensions"
parent: "Part IV: Quality and Evaluation"
nav_order: 12
permalink: /chapters/12-quality-dimensions/
---

# Chapter 12: Prompt Quality Dimensions
{: .fs-9 }

Understanding What Makes Prompts and Responses Effective
{: .fs-6 .fw-300 }

---

## Learning Objectives

After completing this chapter, you will be able to:

1. Define the 5 Quality Dimensions for prompt evaluation
2. Assess prompts and responses against each dimension
3. Identify common quality issues
4. Apply quality checklists systematically
5. Prioritize quality improvements

---

## The 5 Quality Dimensions Framework

### Overview

The **5 Quality Dimensions** provide a comprehensive framework for evaluating the effectiveness of AI prompts and their resulting outputs:

![5 Quality Dimensions]({{ site.baseurl }}/assets/images/5-quality-dimensions.svg)

### Summary Table

| Dimension | Definition | Key Question |
|:----------|:-----------|:-------------|
| **Relevance** | Alignment with request | "Did it answer what I asked?" |
| **Accuracy** | Factual correctness | "Is the information correct?" |
| **Completeness** | Full coverage | "Did it address everything?" |
| **Coherence** | Logical structure | "Does it make sense?" |
| **Actionability** | Practical utility | "Can I use this directly?" |

---

## Dimension 1: Relevance

### Definition

**Relevance** measures how well the response addresses the actual request. A relevant response directly answers the question asked, not a related or tangential question.

### Relevance Indicators

| Score | Description | Example |
|:-----:|:------------|:--------|
| 5 | Perfectly on-topic, addresses exact request | Asked about X, got comprehensive answer about X |
| 4 | Mostly relevant, minor tangents | Addressed X with some useful but unrequested Y |
| 3 | Partially relevant, significant drift | Answered X but spent equal time on Y |
| 2 | Marginally relevant, mostly off-topic | Touched on X but mainly discussed Y |
| 1 | Not relevant, wrong question answered | Asked about X, got answer about Z |

### Common Relevance Issues

| Issue | Cause | Solution |
|:------|:------|:---------|
| **Wrong interpretation** | Ambiguous prompt | Clarify the specific question |
| **Scope creep** | No boundaries specified | Define what's in/out of scope |
| **Over-generalization** | Context missing | Add specific context |
| **Topic drift** | Weak instruction | Anchor to specific task |

### Improving Relevance

```markdown
❌ LOW RELEVANCE PROMPT:
"Tell me about Python"
[Could go anywhere—history, features, comparisons, tutorials...]

✅ HIGH RELEVANCE PROMPT:
"Explain Python's list comprehension syntax with 3 examples
showing filtering, transformation, and nested loops."
[Specific topic, specific format, specific number]
```

---

## Dimension 2: Accuracy

### Definition

**Accuracy** measures the factual correctness of the information provided. An accurate response contains no errors, false claims, or misleading information.

### Accuracy Indicators

| Score | Description | Example |
|:-----:|:------------|:--------|
| 5 | All facts verified, fully accurate | Technical details all correct |
| 4 | Minor inaccuracies, non-critical | Small error that doesn't affect usefulness |
| 3 | Some inaccuracies, partially reliable | Mix of correct and incorrect information |
| 2 | Significant inaccuracies, unreliable | Major errors that could cause problems |
| 1 | Fundamentally wrong, misleading | Core information is false |

### Accuracy Risk Factors

```
HIGH RISK (More likely to be inaccurate):
• Specific numbers, dates, statistics
• Recent events (after training cutoff)
• Technical specifications
• Legal/medical/financial advice
• Niche domain knowledge

LOWER RISK (More likely to be accurate):
• General concepts
• Well-established facts
• Logical reasoning
• Common patterns
• Widely-known information
```

### Improving Accuracy

**Request Verification:**
```markdown
"Provide the answer, then list your sources or indicate
which parts you're most/least confident about."
```

**Constrain to Known Information:**
```markdown
"Only include information you're confident is accurate.
If uncertain, say 'I'm not certain about X' rather than guessing."
```

**Request Caveats:**
```markdown
"For any technical specifications, note if they may have
changed since your training data."
```

---

## Dimension 3: Completeness

### Definition

**Completeness** measures whether all aspects of the request have been addressed. A complete response covers every part of the question without significant omissions.

### Completeness Indicators

| Score | Description | Example |
|:-----:|:------------|:--------|
| 5 | All points addressed thoroughly | Every question answered in full |
| 4 | Most points covered, minor gaps | 90% coverage, small omission |
| 3 | Partial coverage, notable gaps | Answered 2 of 4 parts |
| 2 | Significant omissions | Major aspects missing |
| 1 | Barely addressed | Only superficially touched |

### Completeness Checklist

```markdown
For any multi-part request, verify:

□ Part 1 of question → Addressed? Y/N
□ Part 2 of question → Addressed? Y/N
□ Part 3 of question → Addressed? Y/N
□ Implied requirements → Addressed? Y/N
□ Edge cases mentioned → Addressed? Y/N
```

### Improving Completeness

**Explicit Enumeration:**
```markdown
"Address each of the following points:
1. [Point 1]
2. [Point 2]
3. [Point 3]

For each point, provide [specific requirement]."
```

**Completeness Check Instruction:**
```markdown
"After your response, review the original request and
confirm you've addressed every part. Note any parts
you couldn't fully address."
```

---

## Dimension 4: Coherence

### Definition

**Coherence** measures the logical structure and flow of the response. A coherent response is organized, follows a logical progression, and is easy to understand.

### Coherence Indicators

| Score | Description | Example |
|:-----:|:------------|:--------|
| 5 | Perfectly structured, logical flow | Clear organization, smooth transitions |
| 4 | Well-organized, minor flow issues | Good structure, occasional jumps |
| 3 | Adequate structure, some confusion | Organization present but inconsistent |
| 2 | Poorly organized, hard to follow | Jumbled information, unclear connections |
| 1 | Incoherent, confusing | No discernible structure |

### Coherence Elements

![Coherence Elements]({{ site.baseurl }}/assets/images/coherence-elements.svg)

### Improving Coherence

**Structure Specification:**
```markdown
"Organize your response as:
1. Summary (1-2 sentences)
2. Main explanation (3-4 paragraphs)
3. Key takeaways (bullet points)

Use headers for each section."
```

**Flow Instruction:**
```markdown
"Present information in logical order, from basic to advanced.
Use transition phrases between major points."
```

---

## Dimension 5: Actionability

### Definition

**Actionability** measures whether the output can be directly used for its intended purpose. An actionable response requires no additional transformation before use.

### Actionability Indicators

| Score | Description | Example |
|:-----:|:------------|:--------|
| 5 | Immediately usable as-is | Code runs, content is ready to publish |
| 4 | Usable with minor adjustments | Small tweaks needed |
| 3 | Requires moderate work | Useful but needs significant editing |
| 2 | Foundation only, major work needed | Starting point but far from done |
| 1 | Not usable without complete rework | Must start over |

### Actionability Factors

```markdown
HIGHLY ACTIONABLE:
✓ Correct format for intended use
✓ Complete—no placeholders or TODOs
✓ Tested/verified (for code)
✓ Appropriate level of detail
✓ Ready for target audience

POORLY ACTIONABLE:
✗ Wrong format
✗ Contains [placeholder text]
✗ Missing critical pieces
✗ Too abstract or theoretical
✗ Requires significant adaptation
```

### Improving Actionability

**Format Matching:**
```markdown
"Provide the output in a format I can directly use:
- If code: Complete, runnable, with no placeholders
- If copy: Publication-ready, no [INSERT X HERE]
- If plan: Specific actions, not general advice"
```

**Completeness Requirement:**
```markdown
"Do not use placeholders. If you're unsure about a specific
detail, ask me rather than using [TODO] or similar."
```

---

## Quality Assessment Template

### Full Assessment Form

```markdown
## Prompt Quality Assessment

**Prompt ID:** [Identifier]
**Date:** [Date]
**Use Case:** [Description]

### Prompt Text
[The prompt being evaluated]

### Response Summary
[Brief summary of the response received]

### Quality Scoring (1-5 scale)

| Dimension | Score | Notes |
|:----------|:-----:|:------|
| Relevance | _/5 | |
| Accuracy | _/5 | |
| Completeness | _/5 | |
| Coherence | _/5 | |
| Actionability | _/5 | |
| **TOTAL** | _/25 | |

### Issues Identified
1. [Issue 1]
2. [Issue 2]

### Root Cause Analysis
[Why did these issues occur?]

### Prompt Improvements
[Specific changes to make]

### Revised Prompt
[The improved version]
```

### Quick Assessment

For rapid evaluation, use this abbreviated form:

```markdown
Quick Quality Check:

Relevance:     □ On-target  □ Partial  □ Off-topic
Accuracy:      □ Correct    □ Mostly   □ Errors
Completeness:  □ Full       □ Partial  □ Gaps
Coherence:     □ Clear      □ Okay     □ Confusing
Actionability: □ Ready      □ Needs work □ Not usable

Action: □ Use as-is  □ Minor edit  □ Re-prompt
```

---

## Quality Improvement Workflow

### The Improvement Cycle

![Quality Improvement Cycle]({{ site.baseurl }}/assets/images/quality-improvement-cycle.svg)

### Prioritizing Improvements

| Priority | Focus First On |
|:---------|:---------------|
| 1 | **Relevance** - If it's not addressing the right question, nothing else matters |
| 2 | **Accuracy** - Wrong information is worse than incomplete |
| 3 | **Completeness** - Missing pieces limit usefulness |
| 4 | **Coherence** - Structure can be fixed with formatting |
| 5 | **Actionability** - Final polish for direct use |

---

## Key Takeaways

- The **5 Quality Dimensions** provide a comprehensive evaluation framework
- **Relevance** ensures you get answers to what you actually asked
- **Accuracy** ensures information is correct
- **Completeness** ensures nothing important is missing
- **Coherence** ensures the response is understandable
- **Actionability** ensures the output is usable
- **Systematic assessment** identifies specific areas for improvement

---

## Summary

Quality assessment transforms prompt engineering from guesswork into a measurable discipline. The 5 Quality Dimensions—Relevance, Accuracy, Completeness, Coherence, and Actionability—provide a framework for evaluating any prompt-response pair. By systematically assessing against these dimensions, you can identify specific weaknesses and make targeted improvements. Over time, this practice builds intuition for what makes prompts effective.

---

## Review Questions

1. What are the 5 Quality Dimensions and their key questions?
2. Why is Relevance typically the first dimension to address?
3. What factors increase accuracy risk?
4. How do you measure Completeness for multi-part requests?
5. What makes a response "actionable"?

---

## Practical Exercise

**Exercise 12.1: Quality Assessment**

Take a recent AI interaction and assess it using the full assessment template. Score each dimension and identify areas for improvement.

**Exercise 12.2: Prompt Revision**

Using your assessment from 12.1, revise the prompt to address the identified weaknesses. Re-run and compare quality scores.

---

## Chapter Navigation

| Previous | Up | Next |
|:---------|:---|:-----|
| [← Chapter 11: Multi-Turn Design]({{ site.baseurl }}/chapters/11-multi-turn/) | [Part IV: Quality and Evaluation]({{ site.baseurl }}/part-iv-quality-evaluation/) | [Chapter 13: Testing and Iteration →]({{ site.baseurl }}/chapters/13-testing-iteration/) |
