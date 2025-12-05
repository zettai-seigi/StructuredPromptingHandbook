---
layout: default
title: "Part II: Core Frameworks - Visual Reference"
nav_exclude: true
---

# Part II: Core Frameworks - Visual Reference
{: .fs-9 }

Detailed Visual Specifications for Chapters 4-7
{: .fs-6 .fw-300 }

---

## Color Palette Reference

| Color Name | Hex Code | Usage |
|:-----------|:---------|:------|
| Primary Blue | #2E5090 | Headers, main elements |
| Secondary Teal | #1E8A7E | Framework boxes, highlights |
| Accent Orange | #E07B39 | Call-outs, emphasis |
| Light Gray | #F5F5F5 | Backgrounds |
| Dark Gray | #333333 | Body text |
| Success Green | #28A745 | Positive examples |
| Warning Red | #DC3545 | Negative examples, anti-patterns |

---

## Chapter 4: Prompt Architecture Patterns

### Figure 4.1: Prompt Architecture Components

**Visual ID:** SPH-4.1

**Type:** Vertical Flow Diagram

**Title:** Prompt Architecture

**Chapter Reference:** Chapter 4 - Prompt Architecture Patterns

**Purpose:** To illustrate the five structural components of effective prompts and their sequential relationship.

**Content Description:**
A vertical flow diagram showing five stacked boxes representing the layers of prompt architecture: Preamble (optional), Context, Instruction, Input Data (if applicable), and Output Specification. Arrows connect each layer showing the flow from top to bottom.

**ASCII Source:**
```
┌─────────────────────────────────────────────────────────────────┐
│                    PROMPT ARCHITECTURE                          │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ┌───────────────────────────────────────────────────────────┐ │
│  │ 1. PREAMBLE (Optional)                                    │ │
│  │    System-level instructions, persona, global rules       │ │
│  └───────────────────────────────────────────────────────────┘ │
│                              │                                  │
│                              ▼                                  │
│  ┌───────────────────────────────────────────────────────────┐ │
│  │ 2. CONTEXT                                                │ │
│  │    Background, domain, situation                          │ │
│  └───────────────────────────────────────────────────────────┘ │
│                              │                                  │
│                              ▼                                  │
│  ┌───────────────────────────────────────────────────────────┐ │
│  │ 3. INSTRUCTION                                            │ │
│  │    Task definition, action required                       │ │
│  └───────────────────────────────────────────────────────────┘ │
│                              │                                  │
│                              ▼                                  │
│  ┌───────────────────────────────────────────────────────────┐ │
│  │ 4. INPUT DATA (If applicable)                             │ │
│  │    Content to process, examples, reference material       │ │
│  └───────────────────────────────────────────────────────────┘ │
│                              │                                  │
│                              ▼                                  │
│  ┌───────────────────────────────────────────────────────────┐ │
│  │ 5. OUTPUT SPECIFICATION                                   │ │
│  │    Format, structure, constraints                         │ │
│  └───────────────────────────────────────────────────────────┘ │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 700 x 500 px |
| Format | SVG (scalable) |
| Background | Light gray (#F5F5F5) |
| Border | 2px solid Primary Blue |
| Title Font | Open Sans Bold, 18pt |
| Component Font | Open Sans Regular, 14pt |
| Description Font | Open Sans Light, 12pt |

**Styling Details:**
- Each component box has rounded corners (8px radius)
- Component 1 (Preamble): Dashed border to indicate optional
- Component 4 (Input Data): Dashed border with "(If applicable)" notation
- Connecting arrows: Primary Blue, 2px stroke, filled arrowheads
- Number badges in Primary Blue circles

**Caption:** "Figure 4.1: The five structural components of effective prompt architecture, showing the recommended sequence from preamble to output specification."

**Position in Chapter:** After "Structural Overview" section introduction

**Notes:** Use subtle gradient fills (lighter version of Primary Blue) for each component box to create depth.

---

### Figure 4.2: Framework Selection Flowchart

**Visual ID:** SPH-4.2

**Type:** Decision Tree Flowchart

**Title:** Pattern Selection Guide

**Chapter Reference:** Chapter 4 - Prompt Architecture Patterns

**Purpose:** To help users select the appropriate prompting framework (RTF, RISEN, CO-STAR, CRAFT) based on their task requirements.

**Content Description:**
A decision tree starting with "Is the task simple & quick?" and branching through questions about steps, audience focus, to arrive at one of four framework recommendations: RTF, RISEN, CO-STAR, or CRAFT.

**ASCII Source:**
```
                         ┌─────────────────┐
                         │ Is the task     │
                         │ simple & quick? │
                         └────────┬────────┘
                                  │
                    ┌─────────────┴─────────────┐
                    │                           │
                   YES                          NO
                    │                           │
                    ▼                           ▼
               ┌────────┐            ┌─────────────────┐
               │  RTF   │            │ Does it require │
               └────────┘            │ specific steps? │
                                     └────────┬────────┘
                                              │
                                ┌─────────────┴─────────────┐
                                │                           │
                               YES                          NO
                                │                           │
                                ▼                           ▼
                           ┌────────┐          ┌─────────────────┐
                           │ RISEN  │          │ Is audience     │
                           └────────┘          │ the key factor? │
                                               └────────┬────────┘
                                                        │
                                          ┌─────────────┴─────────────┐
                                          │                           │
                                         YES                          NO
                                          │                           │
                                          ▼                           ▼
                                     ┌────────┐                  ┌────────┐
                                     │CO-STAR │                  │ CRAFT  │
                                     └────────┘                  └────────┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 650 x 450 px |
| Format | SVG (scalable) |
| Background | White (#FFFFFF) |
| Decision Nodes | Rounded rectangles, Secondary Teal border |
| Answer Labels | YES/NO in Accent Orange |
| Framework Boxes | Primary Blue fill, white text |

**Styling Details:**
- Decision nodes: White fill with 2px Secondary Teal border
- YES/NO labels: Bold, Accent Orange
- Framework result boxes: Primary Blue (#2E5090) fill with white bold text
- Connecting lines: Dark Gray, 2px stroke
- Branch arrows: Filled triangular heads

**Caption:** "Figure 4.2: Decision flowchart for selecting the appropriate prompting framework based on task characteristics."

**Position in Chapter:** Within "Pattern Selection Guide" section

**Notes:** Consider adding hover states for interactive web version showing brief framework descriptions.

---

### Figure 4.3: Block Composition Diagram

**Visual ID:** SPH-4.3

**Type:** Building Block Diagram

**Title:** Block Composition

**Chapter Reference:** Chapter 4 - Prompt Architecture Patterns

**Purpose:** To show how modular prompt components combine to form prompts of different complexity levels.

**Content Description:**
Three levels of prompt composition shown as stacked blocks: Simple Prompt (one block), Basic Prompt (three blocks), and Full Prompt (seven blocks), demonstrating the additive nature of prompt building blocks.

**ASCII Source:**
```
┌─────────────────────────────────────────────────────────────┐
│                    BLOCK COMPOSITION                        │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  Simple Prompt = Task Block                                 │
│                                                             │
│  Basic Prompt = Context Block + Task Block + Format Block   │
│                                                             │
│  Full Prompt = Role Block                                   │
│              + Context Block                                │
│              + Task Block                                   │
│              + Input Block                                  │
│              + Format Block                                 │
│              + Constraint Block                             │
│              + Example Block                                │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 600 x 350 px |
| Format | SVG (scalable) |
| Background | Light Gray (#F5F5F5) |
| Block Elements | Colored rectangles representing each component |
| Labels | Open Sans Regular, 12pt |

**Styling Details:**
- Each block type gets a unique color from the palette
- Role Block: Primary Blue
- Context Block: Secondary Teal
- Task Block: Accent Orange
- Input Block: #6C757D (Medium Gray)
- Format Block: #28A745 (Success Green)
- Constraint Block: #FFC107 (Yellow)
- Example Block: #17A2B8 (Info Blue)
- Use connecting "+" symbols between blocks
- Show progressive stacking from left (Simple) to right (Full)

**Caption:** "Figure 4.3: Modular building blocks combine to create prompts of varying complexity, from simple single-block prompts to comprehensive seven-block structures."

**Position in Chapter:** Within "Building Blocks Approach" section

**Notes:** Consider animated version for web showing blocks assembling progressively.

---

## Chapter 5: Context Engineering

### Figure 5.1: Context Type Taxonomy

**Visual ID:** SPH-5.1

**Type:** Taxonomy Grid Diagram

**Title:** Types of Context

**Chapter Reference:** Chapter 5 - Context Engineering

**Purpose:** To present the seven types of context (Domain, Task, User, System, Historical, Data, Constraint) in a structured visual format.

**Content Description:**
A grid layout showing seven context type boxes arranged in two rows (4+3), each with a title and brief description beneath pointing to its core function.

**ASCII Source:**
```
┌─────────────────────────────────────────────────────────────────────┐
│                      TYPES OF CONTEXT                               │
├─────────────────────────────────────────────────────────────────────┤
│                                                                     │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐  ┌───────────┐ │
│  │   DOMAIN    │  │    TASK     │  │    USER     │  │  SYSTEM   │ │
│  │   Context   │  │   Context   │  │   Context   │  │  Context  │ │
│  └──────┬──────┘  └──────┬──────┘  └──────┬──────┘  └─────┬─────┘ │
│         │                │                │               │        │
│         ▼                ▼                ▼               ▼        │
│   Industry         Goal of the      Who is           Technical     │
│   knowledge        current task     asking           environment   │
│                                                                     │
│  ┌─────────────┐  ┌─────────────┐  ┌─────────────┐                │
│  │ HISTORICAL  │  │   DATA      │  │ CONSTRAINT  │                │
│  │   Context   │  │   Context   │  │   Context   │                │
│  └──────┬──────┘  └──────┬──────┘  └──────┬──────┘                │
│         │                │                │                        │
│         ▼                ▼                ▼                        │
│   Previous         Content to       Boundaries                     │
│   interactions     process          and limits                     │
│                                                                     │
└─────────────────────────────────────────────────────────────────────┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 750 x 400 px |
| Format | SVG (scalable) |
| Background | White (#FFFFFF) |
| Context Boxes | 120 x 60 px each |
| Border | 2px solid Primary Blue |
| Title Font | Open Sans Bold, 14pt |
| Description Font | Open Sans Light, 11pt |

**Styling Details:**
- Top row: Domain (blue), Task (teal), User (orange), System (gray)
- Bottom row: Historical (green), Data (purple), Constraint (red)
- Each box has matching color header bar with white text
- Body is white with centered label
- Arrows pointing to descriptions use same color as header

**Caption:** "Figure 5.1: The seven types of context that inform effective prompting, from domain expertise to constraint boundaries."

**Position in Chapter:** At the start of "Types of Context" section

**Notes:** Consider icon additions in each box header for visual recognition.

---

### Figure 5.2: Context Budget Allocation

**Visual ID:** SPH-5.2

**Type:** Stacked Bar/Budget Diagram

**Title:** Context Budget

**Chapter Reference:** Chapter 5 - Context Engineering

**Purpose:** To visualize how the token limit is allocated across different prompt components and available response space.

**Content Description:**
A vertical budget diagram showing total token allocation (8,000 tokens) divided into Reserved for Response (3,000), System Prompt (500), User Prompt (1,500), and Context/Data (3,000).

**ASCII Source:**
```
┌─────────────────────────────────────────────────────────────┐
│                    CONTEXT BUDGET                           │
│                  (Within Token Limit)                       │
├─────────────────────────────────────────────────────────────┤
│                                                             │
│  Total Available: 8,000 tokens                              │
│                                                             │
│  ┌─────────────────────────────────────┐                   │
│  │ Reserved for Response    (3,000)    │                   │
│  └─────────────────────────────────────┘                   │
│                                                             │
│  Available for Input: 5,000 tokens                          │
│                                                             │
│  ┌──────────────────┐  ┌──────────────────┐                │
│  │ System Prompt    │  │ User Prompt      │                │
│  │ (500)            │  │ (1,500)          │                │
│  └──────────────────┘  └──────────────────┘                │
│                                                             │
│  ┌──────────────────────────────────────────────────────┐  │
│  │ Context/Data                                  (3,000) │  │
│  └──────────────────────────────────────────────────────┘  │
│                                                             │
└─────────────────────────────────────────────────────────────┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 600 x 400 px |
| Format | SVG (scalable) |
| Background | Light Gray (#F5F5F5) |
| Budget Bars | Proportional width based on token values |
| Labels | Token counts in parentheses |

**Styling Details:**
- Reserved for Response: Light Blue (#A8D4E6)
- System Prompt: Secondary Teal
- User Prompt: Accent Orange
- Context/Data: Primary Blue
- Token numbers right-aligned within bars
- Clear division line between input and output allocation
- Total bar at top showing full 8,000 capacity

**Caption:** "Figure 5.2: Token budget allocation showing how context competes with other prompt components for available input space."

**Position in Chapter:** Within "Context Optimization" section

**Notes:** Could be made interactive to allow users to adjust allocations and see impact.

---

### Figure 5.3: Context With vs Without Comparison

**Visual ID:** SPH-5.3

**Type:** Before/After Comparison Diagram

**Title:** The Context Imperative

**Chapter Reference:** Chapter 5 - Context Engineering

**Purpose:** To illustrate the dramatic difference in output quality between prompts with and without proper context.

**Content Description:**
A side-by-side comparison showing two paths: "Without Context" leading to "Generic Response (May fit or miss)" and "With Context" leading to "Specific Response (Tailored to need)."

**ASCII Source:**
```
Without Context                    With Context
      │                                 │
      ▼                                 ▼
┌─────────────┐                  ┌─────────────┐
│   Generic   │                  │   Specific  │
│  Response   │                  │  Response   │
│  (May fit   │                  │ (Tailored   │
│  or miss)   │                  │  to need)   │
└─────────────┘                  └─────────────┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 500 x 250 px |
| Format | SVG (scalable) |
| Background | White (#FFFFFF) |
| Left Path | Warning Red accents |
| Right Path | Success Green accents |

**Styling Details:**
- "Without Context" header in Warning Red
- "With Context" header in Success Green
- Left result box: Light red background, dashed border
- Right result box: Light green background, solid border
- Arrows in matching colors
- Result descriptions in italics

**Caption:** "Figure 5.3: The difference context makes—from generic, hit-or-miss responses to tailored, precise outputs."

**Position in Chapter:** At the start of "What Is Context?" section

**Notes:** Simple but impactful visual for emphasizing context importance.

---

## Chapter 6: Instruction Design Principles

### Figure 6.1: Instruction Hierarchy

**Visual ID:** SPH-6.1

**Type:** Hierarchical Stack Diagram

**Title:** Instruction Hierarchy

**Chapter Reference:** Chapter 6 - Instruction Design Principles

**Purpose:** To show the four levels of instruction priority (System, Task, Format, Style) and how higher levels override lower ones.

**Content Description:**
A vertical stack showing four instruction levels from highest priority (System Instructions) to lowest (Style Instructions), with clear delineation of each level's purpose.

**ASCII Source:**
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

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 700 x 500 px |
| Format | SVG (scalable) |
| Background | Light Gray (#F5F5F5) |
| Level Boxes | Graduated sizes (larger at top) |
| Border | Primary Blue outer frame |

**Styling Details:**
- Level 1 (System): Deep Primary Blue, bold "HIGHEST PRIORITY" badge
- Level 2 (Task): Secondary Teal
- Level 3 (Format): Accent Orange
- Level 4 (Style): Medium Gray, "LOWEST PRIORITY" badge
- Downward arrows showing override direction
- Example text in italic within each level
- Visual size reduction from top to bottom indicating priority

**Caption:** "Figure 6.1: The four-level instruction hierarchy showing priority order—system instructions override all others."

**Position in Chapter:** Within "The Instruction Hierarchy" section

**Notes:** Use opacity or saturation to emphasize priority difference (darker = higher priority).

---

### Figure 6.2: Instruction Refinement Loop

**Visual ID:** SPH-6.2

**Type:** Circular Process Diagram

**Title:** Instruction Refinement

**Chapter Reference:** Chapter 6 - Instruction Design Principles

**Purpose:** To illustrate the iterative process of drafting, testing, evaluating, and refining instructions.

**Content Description:**
A circular workflow showing five stages: Draft Instruction → Test (Run it) → Evaluate Results → Refine/Improve (loops back to Draft) or if good results → Document & Reuse (exit point).

**ASCII Source:**
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

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 550 x 450 px |
| Format | SVG (scalable) |
| Background | White (#FFFFFF) |
| Process Boxes | Rounded rectangles, 100 x 60 px |
| Decision Branch | Diamond shape for evaluation |

**Styling Details:**
- Draft: Light Blue
- Test: Secondary Teal
- Evaluate: Accent Orange (diamond shape for decision)
- Refine: Warning Red (indicates iteration needed)
- Document: Success Green (final success state)
- "No" path in red, "Yes" path in green
- Circular arrow from Refine back to Draft

**Caption:** "Figure 6.2: The instruction refinement loop—an iterative process for improving instruction clarity through testing and evaluation."

**Position in Chapter:** Within "Instruction Refinement Workflow" section

**Notes:** Consider adding iteration counter visual element showing "common: 2-3 iterations."

---

## Chapter 7: Output Specification Techniques

### Figure 7.1: Output Impact Comparison

**Visual ID:** SPH-7.1

**Type:** Before/After Comparison Diagram

**Title:** Impact of Output Specification

**Chapter Reference:** Chapter 7 - Output Specification Techniques

**Purpose:** To contrast the characteristics of AI outputs with and without proper specification.

**Content Description:**
A side-by-side comparison showing four characteristics each for unspecified outputs (Variable format, Unpredictable, Manual processing, Hard to validate) versus specified outputs (Consistent format, Predictable, Automatable, Easy to validate).

**ASCII Source:**
```
Without Specification              With Specification
        │                                  │
        ▼                                  ▼
┌───────────────────┐           ┌───────────────────┐
│ Variable format   │           │ Consistent format │
│ Unpredictable     │           │ Predictable       │
│ Manual processing │           │ Automatable       │
│ Hard to validate  │           │ Easy to validate  │
└───────────────────┘           └───────────────────┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 600 x 300 px |
| Format | SVG (scalable) |
| Background | White (#FFFFFF) |
| Left Column | Warning Red theme |
| Right Column | Success Green theme |

**Styling Details:**
- Left box: Light red (#FFEBEE) background, red border
- Right box: Light green (#E8F5E9) background, green border
- Headers in bold with matching colors
- Bullet points or checkmarks in right column
- X marks in left column
- Visual alignment showing direct contrasts

**Caption:** "Figure 7.1: The transformation from unpredictable outputs to consistent, automatable results through proper specification."

**Position in Chapter:** At the start of "Why Output Specification Matters" section

**Notes:** Simple comparison that reinforces the chapter's core message.

---

### Table 7.1: Format Specification Methods

**Visual ID:** SPH-T7.1

**Type:** Reference Table

**Title:** Format Specification Methods

**Chapter Reference:** Chapter 7 - Output Specification Techniques

**Purpose:** To provide a quick reference for the four methods of specifying output format.

**Content Description:**
| Method | Description | Use Case |
|:-------|:------------|:---------|
| Format Naming | Specify by known format name | "Return as JSON" |
| Template Specification | Provide structure template | Reports, forms |
| Schema Definition | Define exact structure | API responses |
| Example-Based | Show desired output sample | Complex formats |

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Table Width | 100% content width |
| Header | Primary Blue background, white text |
| Rows | Alternating Light Gray/White |
| Border | 1px Light Gray |

**Caption:** "Table 7.1: Four methods for specifying output format, from simple naming to comprehensive schema definition."

**Position in Chapter:** Within "Format Specification Methods" section

---

### Table 7.2: Length Specification Options

**Visual ID:** SPH-T7.2

**Type:** Reference Table

**Title:** Length Specification Options

**Chapter Reference:** Chapter 7 - Output Specification Techniques

**Purpose:** To show different ways to specify output length constraints.

**Content Description:**
| Specification Type | Example |
|:-------------------|:--------|
| Word count | "Write 200-300 words" |
| Sentence count | "Respond in 3-5 sentences" |
| Paragraph count | "Provide a 2-paragraph summary" |
| Page length | "One page maximum (~500 words)" |
| Character limit | "Maximum 280 characters (tweet length)" |

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Table Width | 80% content width |
| Header | Secondary Teal background |
| Example Column | Monospace font (code style) |

**Caption:** "Table 7.2: Options for specifying output length across different measurement units."

**Position in Chapter:** Within "Length and Detail Control" section

---

## Summary Statistics

| Part | Chapters | Figures | Tables | Total Visuals |
|:-----|:---------|:--------|:-------|:--------------|
| Part II | 4-7 | 7 | 2 | 9 |

### Figures by Chapter

| Chapter | Figure Count | Visual IDs |
|:--------|:-------------|:-----------|
| Chapter 4 | 3 | SPH-4.1, SPH-4.2, SPH-4.3 |
| Chapter 5 | 3 | SPH-5.1, SPH-5.2, SPH-5.3 |
| Chapter 6 | 2 | SPH-6.1, SPH-6.2 |
| Chapter 7 | 1 | SPH-7.1 |

### Implementation Priority

| Priority | Visual IDs | Rationale |
|:---------|:-----------|:----------|
| High | SPH-4.1, SPH-4.2 | Core framework visuals referenced throughout |
| High | SPH-5.1, SPH-6.1 | Key taxonomies users will reference often |
| Medium | SPH-5.2, SPH-5.3 | Supporting context concepts |
| Medium | SPH-6.2, SPH-7.1 | Process and comparison diagrams |
| Standard | SPH-4.3 | Advanced composition concept |

---

*Source: Structured Prompting Handbook - https://zettai-seigi.github.io/StructuredPromptingHandbook/*
