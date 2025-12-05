---
layout: default
title: "Part IV: Quality and Evaluation - Visual Reference"
nav_exclude: true
---

# Part IV: Quality and Evaluation - Visual Reference
{: .fs-9 }

Detailed Visual Specifications for Chapters 12-14
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
| Success Green | #28A745 | Positive indicators, pass |
| Warning Red | #DC3545 | Negative indicators, fail |
| Warning Yellow | #FFC107 | Caution indicators |

---

## Chapter 12: Prompt Quality Dimensions

### Figure 12.1: The 5 Quality Dimensions

**Visual ID:** SPH-12.1

**Type:** Vertical Stack Diagram

**Title:** 5 Quality Dimensions

**Chapter Reference:** Chapter 12 - Prompt Quality Dimensions

**Purpose:** To present the five quality dimensions (Relevance, Accuracy, Completeness, Coherence, Actionability) as a comprehensive evaluation framework.

**Content Description:**
Five stacked boxes, each containing a quality dimension name and its key question: RELEVANCE (Does it address what was actually asked?), ACCURACY (Is the information factually correct?), COMPLETENESS (Are all aspects of the request covered?), COHERENCE (Is it logically structured and easy to follow?), ACTIONABILITY (Can the output be directly used for its purpose?).

**ASCII Source:**
```
┌─────────────────────────────────────────────────────────────────┐
│                    5 QUALITY DIMENSIONS                         │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │  1. RELEVANCE                                            │   │
│  │     Does it address what was actually asked?             │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │  2. ACCURACY                                             │   │
│  │     Is the information factually correct?                │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │  3. COMPLETENESS                                         │   │
│  │     Are all aspects of the request covered?              │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │  4. COHERENCE                                            │   │
│  │     Is it logically structured and easy to follow?       │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │  5. ACTIONABILITY                                        │   │
│  │     Can the output be directly used for its purpose?     │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 700 x 450 px |
| Format | SVG (scalable) |
| Background | Light Gray (#F5F5F5) |
| Border | 2px solid Primary Blue |
| Dimension Boxes | 600 x 60 px each |
| Title Font | Open Sans Bold, 18pt |
| Dimension Font | Open Sans Bold, 14pt |
| Question Font | Open Sans Regular, 12pt |

**Styling Details:**
- Dimension 1 (Relevance): Primary Blue accent bar on left
- Dimension 2 (Accuracy): Secondary Teal accent bar on left
- Dimension 3 (Completeness): Accent Orange accent bar on left
- Dimension 4 (Coherence): Success Green accent bar on left
- Dimension 5 (Actionability): Warning Yellow accent bar on left
- Number badges: Circular, matching colors
- Question text in italic, lighter color
- Each box has subtle shadow for depth

**Caption:** "Figure 12.1: The 5 Quality Dimensions framework for comprehensive prompt and response evaluation."

**Position in Chapter:** At the start of "The 5 Quality Dimensions Framework" section

**Notes:** Consider adding small icons for each dimension (target for Relevance, checkmark for Accuracy, etc.)

---

### Figure 12.2: Coherence Elements

**Visual ID:** SPH-12.2

**Type:** Three-Column Component Diagram

**Title:** Coherence Elements

**Chapter Reference:** Chapter 12 - Prompt Quality Dimensions

**Purpose:** To break down the three key elements of coherence: Organization, Flow, and Clarity.

**Content Description:**
Three columns showing: ORGANIZATION (Clear sections, Proper hierarchy, Consistent formatting), FLOW (Logical progression, Smooth transitions, No jumps or gaps), and CLARITY (Unambiguous language, Consistent terminology, No jargon without definition).

**ASCII Source:**
```
┌─────────────────────────────────────────────────────────────────┐
│                    COHERENCE ELEMENTS                           │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ORGANIZATION        FLOW             CLARITY                   │
│  ┌─────────────┐    ┌─────────────┐  ┌─────────────┐           │
│  │ Clear       │    │ Logical     │  │ Unambiguous │           │
│  │ sections    │    │ progression │  │ language    │           │
│  │             │    │             │  │             │           │
│  │ Proper      │    │ Smooth      │  │ Consistent  │           │
│  │ hierarchy   │    │ transitions │  │ terminology │           │
│  │             │    │             │  │             │           │
│  │ Consistent  │    │ No jumps    │  │ No jargon   │           │
│  │ formatting  │    │ or gaps     │  │ without     │           │
│  │             │    │             │  │ definition  │           │
│  └─────────────┘    └─────────────┘  └─────────────┘           │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 650 x 300 px |
| Format | SVG (scalable) |
| Background | White (#FFFFFF) |
| Column Width | 180 px each |
| Header Font | Open Sans Bold, 14pt |
| Item Font | Open Sans Regular, 12pt |

**Styling Details:**
- ORGANIZATION column: Primary Blue header
- FLOW column: Secondary Teal header
- CLARITY column: Accent Orange header
- Bullet points in matching header colors
- Subtle connecting lines between columns showing relationship
- Icon for each column header (grid for Organization, arrow for Flow, eye for Clarity)

**Caption:** "Figure 12.2: The three elements of coherence—Organization, Flow, and Clarity—that make responses understandable."

**Position in Chapter:** Within "Dimension 4: Coherence" section

**Notes:** Elements should visually flow left to right, suggesting the reading/comprehension process.

---

### Figure 12.3: Quality Improvement Cycle

**Visual ID:** SPH-12.3

**Type:** Circular Process Flow Diagram

**Title:** Quality Improvement Cycle

**Chapter Reference:** Chapter 12 - Prompt Quality Dimensions

**Purpose:** To illustrate the iterative process of running prompts, assessing quality, identifying gaps, and revising.

**Content Description:**
A circular workflow: RUN (Execute prompt) → ASSESS (Score on 5 dimensions) → IDENTIFY GAPS (Issues found) → REVISE (Improve prompt) [loops back to RUN], or if no issues → DOCUMENT SUCCESS (exit point).

**ASCII Source:**
```
┌─────────────────────────────────────────────────────────────────┐
│                  QUALITY IMPROVEMENT CYCLE                      │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│     ┌──────────┐                                               │
│     │   RUN    │ Execute prompt                                │
│     └────┬─────┘                                               │
│          │                                                      │
│          ▼                                                      │
│     ┌──────────┐                                               │
│     │  ASSESS  │ Score on 5 dimensions                         │
│     └────┬─────┘                                               │
│          │                                                      │
│          ▼                                                      │
│     ┌──────────┐        ┌──────────┐                          │
│     │ IDENTIFY │───────▶│  REVISE  │ Improve prompt            │
│     │  GAPS    │ Issues │          │                           │
│     └────┬─────┘ found  └────┬─────┘                          │
│          │                   │                                  │
│          │ No issues         │                                  │
│          ▼                   │                                  │
│     ┌──────────┐            │                                  │
│     │ DOCUMENT │◀───────────┘                                  │
│     │ SUCCESS  │                                               │
│     └──────────┘                                               │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 600 x 450 px |
| Format | SVG (scalable) |
| Background | Light Gray (#F5F5F5) |
| Step Boxes | 100 x 50 px |
| Arrow Width | 2px |
| Font | Open Sans Regular, 12pt |

**Styling Details:**
- RUN: Primary Blue fill
- ASSESS: Secondary Teal fill
- IDENTIFY GAPS: Accent Orange fill
- REVISE: Warning Red fill (indicates iteration needed)
- DOCUMENT SUCCESS: Success Green fill
- "Issues found" label on branch in Warning Red
- "No issues" label in Success Green
- Loop arrow from REVISE back to RUN
- Description text next to each box

**Caption:** "Figure 12.3: The quality improvement cycle—assess, identify gaps, revise, and repeat until success."

**Position in Chapter:** Within "Quality Improvement Workflow" section

**Notes:** Emphasize the loop path as the common case, success path as the goal.

---

## Chapter 13: Testing and Iteration Strategies

### Figure 13.1: Prompt Testing Lifecycle

**Visual ID:** SPH-13.1

**Type:** Circular Process Flow Diagram

**Title:** Prompt Testing Lifecycle

**Chapter Reference:** Chapter 13 - Testing and Iteration Strategies

**Purpose:** To illustrate the six-stage testing lifecycle from design through documentation.

**Content Description:**
A circular workflow with six stages: 1. DESIGN (Prompt) → 2. TEST (Execute) → 3. ANALYZE (Results) → 4. EVALUATE (Score) → 5. ITERATE (Refine) [loops back to DESIGN] → 6. DOCUMENT (& Deploy) [exit point].

**ASCII Source:**
```
┌─────────────────────────────────────────────────────────────────┐
│                  PROMPT TESTING LIFECYCLE                       │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│   ┌──────────┐    ┌──────────┐    ┌──────────┐                │
│   │ 1.DESIGN │───▶│ 2. TEST  │───▶│3.ANALYZE │                │
│   │  Prompt  │    │ Execute  │    │ Results  │                │
│   └──────────┘    └──────────┘    └──────────┘                │
│        ▲                               │                        │
│        │                               ▼                        │
│        │         ┌──────────┐    ┌──────────┐                  │
│        └─────────│5. ITERATE│◀───│4.EVALUATE│                  │
│                  │ Refine   │    │ Score    │                  │
│                  └──────────┘    └──────────┘                  │
│                        │                                        │
│                        ▼                                        │
│                  ┌──────────┐                                  │
│                  │6.DOCUMENT│                                  │
│                  │& Deploy  │                                  │
│                  └──────────┘                                  │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 650 x 400 px |
| Format | SVG (scalable) |
| Background | White (#FFFFFF) |
| Step Boxes | 90 x 55 px each |
| Number Badges | 20px circular |
| Font | Open Sans, 12pt |

**Styling Details:**
- Steps 1-3 (top row): Primary Blue, Secondary Teal, Accent Orange
- Steps 4-5 (middle): Success Green, Warning Yellow
- Step 6 (exit): Dark Blue (final state)
- Circular flow arrows in Dark Gray
- Exit arrow to Document in Success Green
- Number badges in white text on colored circles
- Description labels below each box

**Caption:** "Figure 13.1: The six-stage prompt testing lifecycle from initial design through documentation and deployment."

**Position in Chapter:** Within "The Prompt Testing Lifecycle" section

**Notes:** Show the loop clearly as the iteration path, with Document as the exit point.

---

### Figure 13.2: Testing Benefits Framework

**Visual ID:** SPH-13.2

**Type:** Four-Quadrant Grid Diagram

**Title:** Prompt Testing Benefits

**Chapter Reference:** Chapter 13 - Testing and Iteration Strategies

**Purpose:** To highlight the four key benefits of systematic prompt testing: Quality, Efficiency, Confidence, and Knowledge.

**Content Description:**
Four boxes arranged in a 2x2 grid: QUALITY (Catch issues early), EFFICIENCY (Find optimal prompts faster), CONFIDENCE (Know it works before deploy), KNOWLEDGE (Learn what works & why).

**ASCII Source:**
```
┌─────────────────────────────────────────────────────────────────┐
│              PROMPT TESTING BENEFITS                            │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  QUALITY        EFFICIENCY       CONFIDENCE      KNOWLEDGE      │
│  ┌─────────┐   ┌─────────┐     ┌─────────┐    ┌─────────┐     │
│  │ Catch   │   │ Find    │     │ Know it │    │ Learn   │     │
│  │ issues  │   │ optimal │     │ works   │    │ what    │     │
│  │ early   │   │ prompts │     │ before  │    │ works   │     │
│  │         │   │ faster  │     │ deploy  │    │ & why   │     │
│  └─────────┘   └─────────┘     └─────────┘    └─────────┘     │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 700 x 200 px |
| Format | SVG (scalable) |
| Background | Light Gray (#F5F5F5) |
| Benefit Boxes | 140 x 100 px each |
| Header Font | Open Sans Bold, 14pt |
| Content Font | Open Sans Regular, 12pt |

**Styling Details:**
- QUALITY: Primary Blue, shield icon
- EFFICIENCY: Secondary Teal, speedometer icon
- CONFIDENCE: Accent Orange, checkmark icon
- KNOWLEDGE: Success Green, lightbulb icon
- Each box has matching colored header bar
- White body with centered text
- Subtle shadow for depth

**Caption:** "Figure 13.2: The four key benefits of systematic prompt testing—Quality, Efficiency, Confidence, and Knowledge."

**Position in Chapter:** Within "The Testing Imperative" section

**Notes:** Use icons to make each benefit instantly recognizable.

---

### Figure 13.3: A/B Testing Flow

**Visual ID:** SPH-13.3

**Type:** Comparison Flow Diagram

**Title:** A/B Testing for Prompts

**Chapter Reference:** Chapter 13 - Testing and Iteration Strategies

**Purpose:** To illustrate the A/B testing process where the same inputs are run through two prompt variants and results are compared.

**Content Description:**
A flow showing: Same Input(s) splits into two paths—Prompt A → Output A and Prompt B → Output B—then both outputs merge into Compare Results.

**ASCII Source:**
```
        ┌─────────────────┐
        │  Same Input(s)  │
        └────────┬────────┘
                 │
      ┌──────────┴──────────┐
      ▼                     ▼
┌───────────┐         ┌───────────┐
│ Prompt A  │         │ Prompt B  │
└─────┬─────┘         └─────┬─────┘
      │                     │
      ▼                     ▼
┌───────────┐         ┌───────────┐
│ Output A  │         │ Output B  │
└─────┬─────┘         └─────┬─────┘
      │                     │
      └──────────┬──────────┘
                 ▼
        ┌─────────────────┐
        │    Compare      │
        │    Results      │
        └─────────────────┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 500 x 400 px |
| Format | SVG (scalable) |
| Background | White (#FFFFFF) |
| Input Box | Primary Blue |
| Prompt A Path | Secondary Teal |
| Prompt B Path | Accent Orange |
| Compare Box | Success Green |

**Styling Details:**
- Same Input(s): Primary Blue, centered at top
- Split path: Y-junction with equal branches
- Prompt A / Output A: Secondary Teal theme
- Prompt B / Output B: Accent Orange theme
- Compare Results: Success Green, centered at bottom
- Connecting lines: Matching colors for each path
- Clear visual distinction between A and B paths

**Caption:** "Figure 13.3: A/B testing flow—run the same inputs through two prompt variants and compare results."

**Position in Chapter:** Within "A/B Testing for Prompts" section

**Notes:** Keep symmetrical to emphasize fair comparison.

---

### Figure 13.4: PDCA Iteration Cycle

**Visual ID:** SPH-13.4

**Type:** Circular Quadrant Diagram

**Title:** PDCA Cycle

**Chapter Reference:** Chapter 13 - Testing and Iteration Strategies

**Purpose:** To show the Plan-Do-Check-Act cycle for prompt iteration.

**Content Description:**
A circular diagram divided into four quadrants: PLAN (Identify improvement opportunity), DO (Implement change), CHECK (Test and measure), ACT (Standardize if it works), with arrows showing clockwise flow.

**ASCII Source:**
```
┌─────────────────────────────────────────────────────────────────┐
│                      PDCA CYCLE                                 │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│         PLAN                              DO                    │
│    ┌─────────────┐                  ┌─────────────┐            │
│    │ Identify    │                  │ Implement   │            │
│    │ improvement │                  │ change      │            │
│    │ opportunity │                  │             │            │
│    └──────┬──────┘                  └──────┬──────┘            │
│           │                                │                    │
│           └────────────────┬───────────────┘                    │
│                            │                                    │
│           ┌────────────────┴───────────────┐                    │
│           │                                │                    │
│    ┌──────┴──────┐                  ┌──────┴──────┐            │
│    │ Standardize │                  │ Test and    │            │
│    │ if it works │                  │ measure     │            │
│    │             │                  │             │            │
│    └─────────────┘                  └─────────────┘            │
│         ACT                              CHECK                  │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 550 x 400 px |
| Format | SVG (scalable) |
| Background | Light Gray (#F5F5F5) |
| Quadrant Size | 200 x 150 px each |
| Title Font | Open Sans Bold, 16pt |
| Content Font | Open Sans Regular, 12pt |

**Styling Details:**
- PLAN quadrant: Primary Blue
- DO quadrant: Secondary Teal
- CHECK quadrant: Accent Orange
- ACT quadrant: Success Green
- Circular arrows connecting quadrants clockwise
- Center point with connecting lines to all quadrants
- Each quadrant has matching colored header

**Caption:** "Figure 13.4: The Plan-Do-Check-Act (PDCA) cycle for systematic prompt iteration and improvement."

**Position in Chapter:** Within "The PDCA Cycle" section

**Notes:** Classic Deming cycle representation adapted for prompt engineering.

---

## Chapter 14: Performance Metrics and Evaluation

### Figure 14.1: Measurement Categories Grid

**Visual ID:** SPH-14.1

**Type:** Six-Category Grid Diagram

**Title:** Measurement Categories

**Chapter Reference:** Chapter 14 - Performance Metrics and Evaluation

**Purpose:** To present the six categories of metrics to measure: Quality, Efficiency, User Experience, Reliability, Safety, and Maintainability.

**Content Description:**
A 2x3 grid showing: QUALITY (Accuracy, Relevance, Completeness, Consistency), EFFICIENCY (Response Time, Token usage, Cost per query), USER EXPERIENCE (Satisfaction, Ease of use, Trust, Task completion), RELIABILITY (Consistency across runs, Error rate, Edge case handling), SAFETY (Harmful output rate, Policy compliance), MAINTAINABILITY (Ease of modification, Documentation quality).

**ASCII Source:**
```
┌─────────────────────────────────────────────────────────────────┐
│                    MEASUREMENT CATEGORIES                       │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  QUALITY              EFFICIENCY          USER EXPERIENCE       │
│  ┌─────────────┐     ┌─────────────┐     ┌─────────────┐       │
│  │ Accuracy    │     │ Response    │     │ Satisfaction│       │
│  │ Relevance   │     │ Time        │     │ Ease of use │       │
│  │ Completeness│     │ Token usage │     │ Trust       │       │
│  │ Consistency │     │ Cost per    │     │ Task        │       │
│  │             │     │ query       │     │ completion  │       │
│  └─────────────┘     └─────────────┘     └─────────────┘       │
│                                                                 │
│  RELIABILITY          SAFETY              MAINTAINABILITY       │
│  ┌─────────────┐     ┌─────────────┐     ┌─────────────┐       │
│  │ Consistency │     │ Harmful     │     │ Ease of     │       │
│  │ across runs │     │ output rate │     │ modification│       │
│  │ Error rate  │     │ Policy      │     │ Documentation│      │
│  │ Edge case   │     │ compliance  │     │ quality     │       │
│  │ handling    │     │             │     │             │       │
│  └─────────────┘     └─────────────┘     └─────────────┘       │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 750 x 400 px |
| Format | SVG (scalable) |
| Background | White (#FFFFFF) |
| Category Boxes | 200 x 140 px each |
| Header Font | Open Sans Bold, 14pt |
| Item Font | Open Sans Regular, 11pt |

**Styling Details:**
- Top row (Quality, Efficiency, User Experience): Primary Blue, Secondary Teal, Accent Orange
- Bottom row (Reliability, Safety, Maintainability): Success Green, Warning Red, Info Blue
- Each category box has colored header bar
- Bullet points in matching colors
- Icons in each header (gauge for Quality, clock for Efficiency, etc.)

**Caption:** "Figure 14.1: Six categories of prompt performance metrics spanning quality, efficiency, user experience, and operations."

**Position in Chapter:** Within "What to Measure" section

**Notes:** Comprehensive overview that users can reference when designing measurement systems.

---

### Figure 14.2: Benchmark Structure

**Visual ID:** SPH-14.2

**Type:** Vertical Component Stack Diagram

**Title:** Benchmark Structure

**Chapter Reference:** Chapter 14 - Performance Metrics and Evaluation

**Purpose:** To show the four components of a complete evaluation benchmark: Test Set, Gold Standard, Scoring Methodology, and Baseline Scores.

**Content Description:**
Four stacked components: TEST SET (Fixed set of inputs, Representative of real usage, Includes edge cases), GOLD STANDARD (Ideal outputs for each input, Or evaluation criteria), SCORING METHODOLOGY (How to evaluate responses, Metrics to calculate), BASELINE SCORES (Reference performance to compare against).

**ASCII Source:**
```
┌─────────────────────────────────────────────────────────────────┐
│                    BENCHMARK STRUCTURE                          │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │ TEST SET                                                 │   │
│  │ • Fixed set of inputs                                   │   │
│  │ • Representative of real usage                          │   │
│  │ • Includes edge cases                                   │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │ GOLD STANDARD                                            │   │
│  │ • Ideal outputs for each input                          │   │
│  │ • Or evaluation criteria                                │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │ SCORING METHODOLOGY                                      │   │
│  │ • How to evaluate responses                             │   │
│  │ • Metrics to calculate                                  │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │ BASELINE SCORES                                          │   │
│  │ • Reference performance to compare against              │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 650 x 450 px |
| Format | SVG (scalable) |
| Background | Light Gray (#F5F5F5) |
| Component Boxes | 600 x 85 px each |
| Header Font | Open Sans Bold, 14pt |
| Bullet Font | Open Sans Regular, 12pt |

**Styling Details:**
- TEST SET: Primary Blue header
- GOLD STANDARD: Secondary Teal header
- SCORING METHODOLOGY: Accent Orange header
- BASELINE SCORES: Success Green header
- White body with bullet points
- Numbered indicators (1-4) optional
- Vertical connector line on left showing progression

**Caption:** "Figure 14.2: The four components of a complete evaluation benchmark for consistent prompt measurement."

**Position in Chapter:** Within "Benchmark Development" section

**Notes:** Shows the building blocks needed for repeatable evaluation.

---

### Figure 14.3: Continuous Monitoring Pipeline

**Visual ID:** SPH-14.3

**Type:** Horizontal Pipeline Flow Diagram

**Title:** Continuous Monitoring

**Chapter Reference:** Chapter 14 - Performance Metrics and Evaluation

**Purpose:** To illustrate the continuous monitoring flow: Collect → Analyze → Alert, with Dashboard display.

**Content Description:**
A horizontal pipeline: COLLECT (Log all prompts and responses) → ANALYZE (Compute metrics over time) → ALERT (Notify if threshold crossed), with a branch from ANALYZE to DISPLAY (on dashboard).

**ASCII Source:**
```
┌─────────────────────────────────────────────────────────────────┐
│                  CONTINUOUS MONITORING                          │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│   COLLECT                ANALYZE               ALERT            │
│   ┌─────────┐           ┌─────────┐          ┌─────────┐       │
│   │ Log all │           │ Compute │          │ Notify  │       │
│   │ prompts │──────────▶│ metrics │─────────▶│ if      │       │
│   │ and     │           │ over    │          │ threshold│      │
│   │responses│           │ time    │          │ crossed │       │
│   └─────────┘           └─────────┘          └─────────┘       │
│                              │                                  │
│                              ▼                                  │
│                         ┌─────────┐                            │
│                         │ Display │                            │
│                         │ on      │                            │
│                         │dashboard│                            │
│                         └─────────┘                            │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 700 x 300 px |
| Format | SVG (scalable) |
| Background | White (#FFFFFF) |
| Stage Boxes | 110 x 80 px each |
| Arrow Width | 3px |
| Font | Open Sans Regular, 12pt |

**Styling Details:**
- COLLECT: Primary Blue, database icon
- ANALYZE: Secondary Teal, chart icon
- ALERT: Warning Red, bell icon
- DASHBOARD: Accent Orange, monitor icon
- Flow arrows: Dark Gray with animated dash option
- Downward branch from ANALYZE to DASHBOARD
- Description text inside each box

**Caption:** "Figure 14.3: The continuous monitoring pipeline—collect data, analyze metrics, alert on issues, and display on dashboard."

**Position in Chapter:** Within "Continuous Monitoring" section

**Notes:** Consider animated version showing data flowing through pipeline.

---

### Table 14.1: Core Quantitative Metrics

**Visual ID:** SPH-T14.1

**Type:** Reference Table

**Title:** Core Metrics Reference

**Chapter Reference:** Chapter 14 - Performance Metrics and Evaluation

**Purpose:** To provide a quick reference for the five core quantitative metrics with definitions, formulas, and targets.

**Content Description:**
| Metric | Definition | Formula | Target |
|:-------|:-----------|:--------|:-------|
| Accuracy | Correct responses / Total | Correct / Total × 100% | ≥95% |
| Task Completion | Successfully completed / Attempted | Complete / Attempted × 100% | ≥90% |
| Format Compliance | Correct format / Total | Compliant / Total × 100% | ≥98% |
| Consistency | Same output for same input | Match rate × 100% | ≥85% |
| Response Time | Average time to response | Sum(times) / Count | <3s |

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Table Width | 100% content width |
| Header | Primary Blue background, white text |
| Rows | Alternating Light Gray/White |
| Formula Column | Monospace font |
| Target Column | Bold, color-coded |

**Caption:** "Table 14.1: Core quantitative metrics for prompt performance with calculation formulas and recommended targets."

**Position in Chapter:** Within "Quantitative Metrics" section

---

## Summary Statistics

| Part | Chapters | Figures | Tables | Total Visuals |
|:-----|:---------|:--------|:-------|:--------------|
| Part IV | 12-14 | 8 | 1 | 9 |

### Figures by Chapter

| Chapter | Figure Count | Visual IDs |
|:--------|:-------------|:-----------|
| Chapter 12 | 3 | SPH-12.1, SPH-12.2, SPH-12.3 |
| Chapter 13 | 4 | SPH-13.1, SPH-13.2, SPH-13.3, SPH-13.4 |
| Chapter 14 | 3 | SPH-14.1, SPH-14.2, SPH-14.3 |

### Implementation Priority

| Priority | Visual IDs | Rationale |
|:---------|:-----------|:----------|
| High | SPH-12.1 | Core 5 Dimensions framework |
| High | SPH-13.1, SPH-13.3 | Testing lifecycle and A/B testing fundamentals |
| High | SPH-14.1 | Comprehensive measurement overview |
| Medium | SPH-12.3, SPH-13.4 | Improvement cycles |
| Medium | SPH-14.2, SPH-14.3 | Benchmark and monitoring structures |
| Standard | SPH-12.2, SPH-13.2 | Supporting detail visuals |

---

*Source: Structured Prompting Handbook - https://zettai-seigi.github.io/StructuredPromptingHandbook/*
