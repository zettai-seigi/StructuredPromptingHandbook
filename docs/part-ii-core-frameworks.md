---
layout: default
title: "Part II: Core Frameworks"
nav_order: 3
has_children: true
permalink: /part-ii-core-frameworks/
---

# Part II: Core Frameworks
{: .fs-9 }

Architectural Patterns and Design Principles for Effective Prompts
{: .fs-6 .fw-300 }

---

## Overview

Part II dives deep into the structural elements of prompt design. Once you understand the foundations, you need practical frameworks for constructing prompts that work. This section provides architectural patterns, context engineering strategies, instruction design principles, and output specification techniques.

These chapters cover:
- How to structure prompts for maximum effectiveness
- Techniques for providing the right context
- Methods for writing clear, actionable instructions
- Ways to specify exactly what output you need

---

## Chapters in This Part

### [Chapter 4: Prompt Architecture Patterns]({{ site.baseurl }}/chapters/04-prompt-architecture/)

Structural frameworks for prompt design, including:
- The anatomy of an effective prompt
- Common architectural patterns (CRAFT, RISEN, etc.)
- When to use which pattern
- Building blocks and composability

### [Chapter 5: Context Engineering]({{ site.baseurl }}/chapters/05-context-engineering/)

Mastering the art of context, including:
- What context is and why it matters
- Types of context (domain, task, user, system)
- Context loading strategies
- Managing context window constraints

### [Chapter 6: Instruction Design Principles]({{ site.baseurl }}/chapters/06-instruction-design/)

Writing effective instructions, including:
- The instruction hierarchy
- Clarity and specificity techniques
- Handling ambiguity
- Instruction sequencing and priority

### [Chapter 7: Output Specification Techniques]({{ site.baseurl }}/chapters/07-output-specification/)

Controlling AI outputs, including:
- Format specification methods
- Structured output (JSON, XML, Markdown)
- Length and detail control
- Quality constraints and validation

---

## Key Frameworks Introduced

| Framework | Purpose |
|:----------|:--------|
| CRAFT | Context, Role, Action, Format, Tone |
| RISEN | Role, Instructions, Steps, End goal, Narrowing |
| CO-STAR | Context, Objective, Style, Tone, Audience, Response |
| RTF | Role, Task, Format |

---

## The Prompt Architecture Diagram

```
┌─────────────────────────────────────────────────┐
│                   PROMPT                        │
├─────────────────────────────────────────────────┤
│  ┌─────────────────────────────────────────┐   │
│  │           CONTEXT LAYER                 │   │
│  │  Background │ Domain │ Constraints      │   │
│  └─────────────────────────────────────────┘   │
│  ┌─────────────────────────────────────────┐   │
│  │         INSTRUCTION LAYER               │   │
│  │  Role │ Task │ Requirements │ Steps     │   │
│  └─────────────────────────────────────────┘   │
│  ┌─────────────────────────────────────────┐   │
│  │           OUTPUT LAYER                  │   │
│  │  Format │ Structure │ Constraints       │   │
│  └─────────────────────────────────────────┘   │
│  ┌─────────────────────────────────────────┐   │
│  │          EXAMPLES LAYER                 │   │
│  │  Few-shot examples │ Counter-examples   │   │
│  └─────────────────────────────────────────┘   │
└─────────────────────────────────────────────────┘
```

---

## Learning Objectives

After completing Part II, you will be able to:

1. **Select** appropriate prompt architecture patterns for different tasks
2. **Engineer** context effectively within token constraints
3. **Write** clear, unambiguous instructions
4. **Specify** output formats that meet your needs
5. **Combine** these elements into well-structured prompts

---

## Practical Exercises

Each chapter in Part II includes hands-on exercises:
- Pattern application exercises
- Context optimization challenges
- Instruction refinement practice
- Output specification drills

---

## Prerequisites

Completion of Part I: Foundations, or equivalent understanding of:
- Basic prompting concepts
- The 7 Prompting Pillars
- Token and context window basics

---

## Estimated Reading Time

- Chapter 4: 25-30 minutes
- Chapter 5: 30-35 minutes
- Chapter 6: 25-30 minutes
- Chapter 7: 25-30 minutes

**Total: Approximately 2-2.5 hours**

---

## Next Steps

Begin with [Chapter 4: Prompt Architecture Patterns]({{ site.baseurl }}/chapters/04-prompt-architecture/) to learn the structural foundations of effective prompt design.

---

[Begin Part II →]({{ site.baseurl }}/chapters/04-prompt-architecture/){: .btn .btn-primary .fs-5 .mb-4 .mb-md-0 .mr-2 }
