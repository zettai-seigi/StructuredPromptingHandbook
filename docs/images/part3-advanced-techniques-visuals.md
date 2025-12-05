---
layout: default
title: "Part III: Advanced Techniques - Visual Reference"
nav_exclude: true
---

# Part III: Advanced Techniques - Visual Reference
{: .fs-9 }

Detailed Visual Specifications for Chapters 8-11
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
| Success Green | #28A745 | Positive examples, YES paths |
| Warning Red | #DC3545 | Negative examples, NO paths |
| Info Blue | #17A2B8 | Informational elements |

---

## Chapter 8: Chain-of-Thought and Reasoning

### Figure 8.1: Standard vs Chain-of-Thought Comparison

**Visual ID:** SPH-8.1

**Type:** Process Flow Comparison Diagram

**Title:** The Core Insight

**Chapter Reference:** Chapter 8 - Chain-of-Thought and Reasoning

**Purpose:** To illustrate the fundamental difference between standard prompting (direct question to answer) and chain-of-thought prompting (question through steps to answer).

**Content Description:**
A side-by-side comparison showing two approaches: Standard Prompting as a single arrow from Question to Answer, and Chain-of-Thought Prompting showing Question flowing through Step 1, Step 2, Step 3 to reach Answer.

**ASCII Source:**
```
Standard Prompting:
Question ──────────────────────────────────▶ Answer

Chain-of-Thought Prompting:
Question ──▶ Step 1 ──▶ Step 2 ──▶ Step 3 ──▶ Answer
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 650 x 200 px |
| Format | SVG (scalable) |
| Background | White (#FFFFFF) |
| Arrow Color | Primary Blue |
| Step Boxes | Secondary Teal fill, rounded corners |
| Labels | Open Sans Regular, 14pt |

**Styling Details:**
- Standard Prompting: Single long arrow, direct connection
- Chain-of-Thought: Segmented path with visible step boxes
- Question box: Light blue fill
- Answer box: Success Green fill
- Step boxes: Sequential numbering with Secondary Teal
- Arrow heads: Filled triangles

**Caption:** "Figure 8.1: Standard prompting jumps directly to answers, while chain-of-thought breaks problems into visible reasoning steps."

**Position in Chapter:** At the start of "What Is Chain-of-Thought Prompting?" section

**Notes:** Keep simple to emphasize the core concept quickly.

---

### Figure 8.2: Chain-of-Thought Process Flow

**Visual ID:** SPH-8.2

**Type:** Vertical Process Flow Diagram

**Title:** Chain-of-Thought Process

**Chapter Reference:** Chapter 8 - Chain-of-Thought and Reasoning

**Purpose:** To show the complete chain-of-thought process from problem through decomposition, multiple reasoning steps, to conclusion.

**Content Description:**
A vertical flow showing: PROBLEM → DECOMPOSITION ("Let me break this into parts...") → STEP 1 (Reasoning and intermediate result) → STEP 2 (Reasoning and intermediate result) → STEP N (Reasoning and intermediate result) → CONCLUSION ("Therefore, the answer is...").

**ASCII Source:**
```
┌──────────────────────────────────────────────────────────────────┐
│                    CHAIN-OF-THOUGHT PROCESS                      │
├──────────────────────────────────────────────────────────────────┤
│                                                                  │
│   PROBLEM                                                        │
│      │                                                           │
│      ▼                                                           │
│   ┌──────────────────────────────────────────────────────────┐  │
│   │ DECOMPOSITION                                             │  │
│   │ "Let me break this into parts..."                        │  │
│   └──────────────────────────────────────────────────────────┘  │
│      │                                                           │
│      ▼                                                           │
│   ┌──────────────────────────────────────────────────────────┐  │
│   │ STEP 1: First, I need to...                              │  │
│   │ [Reasoning and intermediate result]                       │  │
│   └──────────────────────────────────────────────────────────┘  │
│      │                                                           │
│      ▼                                                           │
│   ┌──────────────────────────────────────────────────────────┐  │
│   │ STEP 2: Now, using that result...                        │  │
│   │ [Reasoning and intermediate result]                       │  │
│   └──────────────────────────────────────────────────────────┘  │
│      │                                                           │
│      ▼                                                           │
│   ┌──────────────────────────────────────────────────────────┐  │
│   │ STEP N: Finally...                                        │  │
│   │ [Reasoning and intermediate result]                       │  │
│   └──────────────────────────────────────────────────────────┘  │
│      │                                                           │
│      ▼                                                           │
│   ┌──────────────────────────────────────────────────────────┐  │
│   │ CONCLUSION                                                │  │
│   │ "Therefore, the answer is..."                            │  │
│   └──────────────────────────────────────────────────────────┘  │
│                                                                  │
└──────────────────────────────────────────────────────────────────┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 700 x 550 px |
| Format | SVG (scalable) |
| Background | Light Gray (#F5F5F5) |
| Border | 2px solid Primary Blue |
| Step Boxes | 550 x 50 px each |
| Title Font | Open Sans Bold, 18pt |
| Step Font | Open Sans Regular, 13pt |

**Styling Details:**
- PROBLEM box: Accent Orange fill
- DECOMPOSITION box: Light Secondary Teal
- STEP boxes: White fill with Secondary Teal left border (4px)
- CONCLUSION box: Success Green fill
- Connecting arrows: Dark Gray, 2px stroke
- Step numbers: Bold, Primary Blue circles
- "Let me..." and "Therefore..." text in italics

**Caption:** "Figure 8.2: The complete chain-of-thought process showing how problems are decomposed into steps before reaching a conclusion."

**Position in Chapter:** Within "The Reasoning Chain Diagram" section

**Notes:** Ellipsis (...) visual between Step 2 and Step N to indicate variable number of steps.

---

### Figure 8.3: Chain-of-Thought Decision Guide

**Visual ID:** SPH-8.3

**Type:** Decision Tree Flowchart

**Title:** Should I Use Chain-of-Thought?

**Chapter Reference:** Chapter 8 - Chain-of-Thought and Reasoning

**Purpose:** To help users decide when to apply chain-of-thought prompting based on task characteristics.

**Content Description:**
A decision tree with three yes/no questions: "Is the task complex with multiple steps?" → "Is there a logical/mathematical component?" → "Do you need to verify the reasoning?" Each path leads to recommendations about using CoT.

**ASCII Source:**
```
┌─────────────────────────────────────────────────────────────────┐
│              SHOULD I USE CHAIN-OF-THOUGHT?                     │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  Is the task complex with multiple steps?                       │
│      │                                                          │
│      ├── YES ──▶ Could benefit from CoT                        │
│      │                                                          │
│      └── NO ───▶ Probably not needed                           │
│                                                                 │
│  Is there a logical/mathematical component?                     │
│      │                                                          │
│      ├── YES ──▶ Strongly consider CoT                         │
│      │                                                          │
│      └── NO ───▶ Optional                                      │
│                                                                 │
│  Do you need to verify the reasoning?                          │
│      │                                                          │
│      ├── YES ──▶ Use CoT for transparency                      │
│      │                                                          │
│      └── NO ───▶ May skip for efficiency                       │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 600 x 400 px |
| Format | SVG (scalable) |
| Background | White (#FFFFFF) |
| Question Boxes | Rounded rectangles, light fill |
| YES Labels | Success Green |
| NO Labels | Warning Red |

**Styling Details:**
- Questions: White fill with Primary Blue text
- YES paths: Success Green arrows and text
- NO paths: Warning Red arrows and text
- Recommendation boxes: Matching color (green for positive, red for negative)
- Each question in its own section with clear visual separation

**Caption:** "Figure 8.3: Decision guide for determining when chain-of-thought prompting will improve results."

**Position in Chapter:** Within "When to Use Chain-of-Thought" section

**Notes:** Consider animated version where clicking YES/NO highlights the path.

---

## Chapter 9: Few-Shot and Example-Based Prompting

### Figure 9.1: Learning Paradigm Progression

**Visual ID:** SPH-9.1

**Type:** Horizontal Progression Diagram

**Title:** The Learning Paradigm

**Chapter Reference:** Chapter 9 - Few-Shot and Example-Based Prompting

**Purpose:** To show the progression from zero-shot to one-shot to few-shot prompting.

**Content Description:**
Three horizontal paths showing: Zero-Shot (Instruction → Task), One-Shot (Instruction + 1 Example → Task), and Few-Shot (Instruction + N Examples → Task), where N is typically 2-5 examples.

**ASCII Source:**
```
Zero-Shot:     Instruction ──────────────────────▶ Task

One-Shot:      Instruction + 1 Example ──────────▶ Task

Few-Shot:      Instruction + N Examples ─────────▶ Task
               (typically 2-5 examples)
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 600 x 250 px |
| Format | SVG (scalable) |
| Background | White (#FFFFFF) |
| Arrow Color | Primary Blue |
| Label Font | Open Sans Regular, 14pt |

**Styling Details:**
- Zero-Shot: Single short element before arrow
- One-Shot: Instruction box + small "1" badge
- Few-Shot: Instruction box + stacked example indicators
- Example count "(typically 2-5 examples)" in smaller italic text
- Task boxes: Identical across all three to show consistent output target
- Visual progression from simple (top) to complex (bottom)

**Caption:** "Figure 9.1: The progression from zero-shot (no examples) through one-shot to few-shot prompting with multiple examples."

**Position in Chapter:** At the start of "What Is Few-Shot Prompting?" section

**Notes:** Use graduated shading to show complexity increase.

---

### Figure 9.2: Example Selection Process

**Visual ID:** SPH-9.2

**Type:** Vertical Process Flow Diagram

**Title:** Example Selection Process

**Chapter Reference:** Chapter 9 - Few-Shot and Example-Based Prompting

**Purpose:** To illustrate the six-step process for selecting effective few-shot examples.

**Content Description:**
A vertical flow showing: IDENTIFY the target task pattern → BRAINSTORM potential example inputs → FILTER for diversity and representativeness → CREATE ideal outputs for each input → ORDER from simple to complex → TEST with target inputs to verify pattern transfer.

**ASCII Source:**
```
┌─────────────────────────────────────────────────────────────────┐
│               EXAMPLE SELECTION PROCESS                         │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  1. IDENTIFY the target task pattern                            │
│      │                                                          │
│      ▼                                                          │
│  2. BRAINSTORM potential example inputs                         │
│      │                                                          │
│      ▼                                                          │
│  3. FILTER for diversity and representativeness                 │
│      │                                                          │
│      ▼                                                          │
│  4. CREATE ideal outputs for each input                         │
│      │                                                          │
│      ▼                                                          │
│  5. ORDER from simple to complex                                │
│      │                                                          │
│      ▼                                                          │
│  6. TEST with target inputs to verify pattern transfer          │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 600 x 450 px |
| Format | SVG (scalable) |
| Background | Light Gray (#F5F5F5) |
| Step Boxes | Alternating colors from palette |
| Number Badges | Circular, Primary Blue |
| Font | Open Sans Regular, 14pt |

**Styling Details:**
- Step 1 (IDENTIFY): Primary Blue
- Step 2 (BRAINSTORM): Secondary Teal
- Step 3 (FILTER): Accent Orange
- Step 4 (CREATE): Success Green
- Step 5 (ORDER): Info Blue
- Step 6 (TEST): Primary Blue (completing the cycle)
- Connecting arrows: Dark Gray, 2px
- Action verbs in bold caps

**Caption:** "Figure 9.2: The six-step process for selecting effective few-shot examples, from identifying patterns to testing transfer."

**Position in Chapter:** Within "Selecting Effective Examples" section

**Notes:** Could add icons for each step (magnifying glass for IDENTIFY, lightbulb for BRAINSTORM, etc.)

---

### Figure 9.3: Example Diversity Framework

**Visual ID:** SPH-9.3

**Type:** Three-Column Category Diagram

**Title:** Example Diversity

**Chapter Reference:** Chapter 9 - Few-Shot and Example-Based Prompting

**Purpose:** To show the three dimensions of diversity to consider when selecting examples: length, complexity, and content.

**Content Description:**
A three-column layout showing: Length Diversity (Short/Medium/Long input examples), Complexity Diversity (Simple/Moderate/Edge case), and Content Diversity (Different topics/structures within scope).

**ASCII Source:**
```
┌────────────────────────────────────────────────────────────────┐
│                    EXAMPLE DIVERSITY                           │
├────────────────────────────────────────────────────────────────┤
│                                                                │
│  Length Diversity:                                             │
│  • Short input example                                         │
│  • Medium input example                                        │
│  • Long input example                                          │
│                                                                │
│  Complexity Diversity:                                         │
│  • Simple, clear-cut case                                      │
│  • Moderate complexity                                         │
│  • Edge case or unusual situation                              │
│                                                                │
│  Content Diversity:                                            │
│  • Different topics/domains within scope                       │
│  • Different structures within the input type                  │
│                                                                │
└────────────────────────────────────────────────────────────────┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 600 x 350 px |
| Format | SVG (scalable) |
| Background | White (#FFFFFF) |
| Section Headers | Bold, colored per category |
| Bullet Points | Matching category color |

**Styling Details:**
- Length Diversity header: Primary Blue
- Complexity Diversity header: Secondary Teal
- Content Diversity header: Accent Orange
- Sub-items: Progressive indentation with bullet points
- Visual representation of length (short bar, medium bar, long bar) next to Length section
- Complexity shown as simple circle, medium star, complex shape

**Caption:** "Figure 9.3: The three dimensions of example diversity to ensure comprehensive coverage in few-shot prompts."

**Position in Chapter:** Within "Example Diversity Strategy" section

**Notes:** Could include visual icons representing each sub-item.

---

### Figure 9.4: Diminishing Returns Curve

**Visual ID:** SPH-9.4

**Type:** Line Graph

**Title:** Diminishing Returns in Few-Shot

**Chapter Reference:** Chapter 9 - Few-Shot and Example-Based Prompting

**Purpose:** To visualize how quality improvement from additional examples follows a diminishing returns curve, with most benefit from 2-5 examples.

**Content Description:**
A line graph showing Quality (y-axis) vs Number of Examples (x-axis, 1-6+). The curve rises steeply from 1-3 examples, then plateaus after 4-5 examples.

**ASCII Source:**
```
                Quality
                   │
                   │          ╭────────────────
                   │        ╱
                   │      ╱
                   │    ╱
                   │  ╱
                   │╱
                   └──────────────────────────────
                       1    2    3    4    5    6+
                            Number of Examples

Quality improves rapidly at first, then plateaus.
Usually 2-5 examples capture most of the benefit.
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 500 x 300 px |
| Format | SVG (scalable) |
| Background | White (#FFFFFF) |
| Axis Color | Dark Gray |
| Curve Color | Primary Blue |
| Highlight Zone | Light green shading (2-5 range) |

**Styling Details:**
- Y-axis: "Quality" label
- X-axis: Numbers 1 through "6+"
- Curve: Smooth logarithmic-style curve
- Shaded "optimal zone" from 2-5 examples in light green
- Annotation arrow pointing to plateau region
- Subtitle text in smaller font below

**Caption:** "Figure 9.4: The diminishing returns curve showing optimal example count—typically 2-5 examples capture most benefits."

**Position in Chapter:** Within "How Many Examples?" section

**Notes:** Consider adding data points on the curve with tooltips showing typical improvement percentages.

---

## Chapter 10: System Prompts and Persona Design

### Figure 10.1: Prompt Hierarchy

**Visual ID:** SPH-10.1

**Type:** Hierarchical Stack Diagram

**Title:** Prompt Hierarchy

**Chapter Reference:** Chapter 10 - System Prompts and Persona Design

**Purpose:** To show the priority relationship between system prompts, user prompts, and AI responses.

**Content Description:**
A vertical stack showing: SYSTEM PROMPT (highest priority, sets global behavior, defines persona, establishes constraints, persistent across conversation) → USER PROMPT (individual requests, specific tasks, operates within system constraints) → AI RESPONSE (shaped by both system and user prompts).

**ASCII Source:**
```
┌─────────────────────────────────────────────────────────────────┐
│                    PROMPT HIERARCHY                             │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ┌───────────────────────────────────────────────────────────┐ │
│  │                    SYSTEM PROMPT                          │ │
│  │  • Highest priority                                       │ │
│  │  • Sets global behavior                                   │ │
│  │  • Defines persona                                        │ │
│  │  • Establishes constraints                                │ │
│  │  • Persistent across conversation                         │ │
│  └───────────────────────────────────────────────────────────┘ │
│                              │                                  │
│                              ▼                                  │
│  ┌───────────────────────────────────────────────────────────┐ │
│  │                    USER PROMPT                            │ │
│  │  • Individual requests                                    │ │
│  │  • Specific tasks                                         │ │
│  │  • Operates within system constraints                     │ │
│  └───────────────────────────────────────────────────────────┘ │
│                              │                                  │
│                              ▼                                  │
│  ┌───────────────────────────────────────────────────────────┐ │
│  │                    AI RESPONSE                            │ │
│  │  • Shaped by both system and user prompts                │ │
│  └───────────────────────────────────────────────────────────┘ │
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
| Title Font | Open Sans Bold, 18pt |
| Content Font | Open Sans Regular, 13pt |

**Styling Details:**
- SYSTEM PROMPT box: Deep Primary Blue fill, white text, "HIGHEST PRIORITY" badge
- USER PROMPT box: Secondary Teal fill, white text
- AI RESPONSE box: Accent Orange fill, white text
- Size graduation: System largest, User medium, Response smallest
- Connecting arrows: Thick (3px), Dark Gray
- Priority indicators: Descending opacity or size

**Caption:** "Figure 10.1: The prompt hierarchy showing how system prompts take precedence over user prompts in shaping AI responses."

**Position in Chapter:** Within "System vs. User Prompts" section

**Notes:** Use opacity gradient to reinforce priority (system = 100% opacity, response = 70% opacity).

---

### Figure 10.2: System Prompt Anatomy

**Visual ID:** SPH-10.2

**Type:** Component Block Diagram

**Title:** System Prompt Anatomy

**Chapter Reference:** Chapter 10 - System Prompts and Persona Design

**Purpose:** To show the six building blocks of a comprehensive system prompt.

**Content Description:**
Six stacked blocks: IDENTITY BLOCK (Who are you? What is your role?), PURPOSE BLOCK (What are you designed to do?), BEHAVIOR BLOCK (How should you act and respond?), CONSTRAINTS BLOCK (What must you avoid or never do?), KNOWLEDGE BLOCK - Optional (What information do you have access to?), FORMAT BLOCK - Optional (How should you structure responses?).

**ASCII Source:**
```
┌─────────────────────────────────────────────────────────────────┐
│                   SYSTEM PROMPT ANATOMY                         │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ┌───────────────────────────────────────────────────────────┐ │
│  │ 1. IDENTITY BLOCK                                         │ │
│  │    Who are you? What is your role?                        │ │
│  └───────────────────────────────────────────────────────────┘ │
│                                                                 │
│  ┌───────────────────────────────────────────────────────────┐ │
│  │ 2. PURPOSE BLOCK                                          │ │
│  │    What are you designed to do?                           │ │
│  └───────────────────────────────────────────────────────────┘ │
│                                                                 │
│  ┌───────────────────────────────────────────────────────────┐ │
│  │ 3. BEHAVIOR BLOCK                                         │ │
│  │    How should you act and respond?                        │ │
│  └───────────────────────────────────────────────────────────┘ │
│                                                                 │
│  ┌───────────────────────────────────────────────────────────┐ │
│  │ 4. CONSTRAINTS BLOCK                                      │ │
│  │    What must you avoid or never do?                       │ │
│  └───────────────────────────────────────────────────────────┘ │
│                                                                 │
│  ┌───────────────────────────────────────────────────────────┐ │
│  │ 5. KNOWLEDGE BLOCK (Optional)                             │ │
│  │    What information do you have access to?                │ │
│  └───────────────────────────────────────────────────────────┘ │
│                                                                 │
│  ┌───────────────────────────────────────────────────────────┐ │
│  │ 6. FORMAT BLOCK (Optional)                                │ │
│  │    How should you structure responses?                    │ │
│  └───────────────────────────────────────────────────────────┘ │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 700 x 500 px |
| Format | SVG (scalable) |
| Background | White (#FFFFFF) |
| Block Height | 60 px each |
| Number Badges | Circular, 24px diameter |
| Font | Open Sans, 13pt |

**Styling Details:**
- Block 1 (Identity): Primary Blue
- Block 2 (Purpose): Secondary Teal
- Block 3 (Behavior): Accent Orange
- Block 4 (Constraints): Warning Red
- Block 5 (Knowledge): Light Gray with dashed border (optional)
- Block 6 (Format): Light Gray with dashed border (optional)
- Question text in italics
- Optional blocks clearly marked with dashed borders

**Caption:** "Figure 10.2: The six components of a comprehensive system prompt, with knowledge and format blocks being optional."

**Position in Chapter:** Within "System Prompt Architecture" section

**Notes:** Optional blocks should have visual distinction (lighter colors, dashed borders).

---

### Figure 10.3: Persona Spectrum

**Visual ID:** SPH-10.3

**Type:** Horizontal Spectrum Diagram

**Title:** The Persona Spectrum

**Chapter Reference:** Chapter 10 - System Prompts and Persona Design

**Purpose:** To show the range of persona specificity from generic "Helpful Assistant" to highly specific character-based personas.

**Content Description:**
A horizontal spectrum from Generic (left) to Specific (right) with four example personas: Helpful Assistant (very broad), Writing Assistant (domain focus), Marketing Copywriter (role specific), and "Sarah, 15-yr Marketing Director" (full character).

**ASCII Source:**
```
Generic                                              Specific
   │                                                    │
   ▼                                                    ▼
┌──────────┐   ┌──────────┐   ┌──────────┐   ┌──────────┐
│ Helpful  │   │ Writing  │   │ Marketing│   │ Sarah,   │
│ Assistant│   │ Assistant│   │ Copywriter│  │ 15-yr    │
│          │   │          │   │          │   │ Marketing│
│          │   │          │   │          │   │ Director │
└──────────┘   └──────────┘   └──────────┘   └──────────┘
     │              │              │              │
 Very broad    Domain focus   Role specific   Full character
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 750 x 250 px |
| Format | SVG (scalable) |
| Background | White (#FFFFFF) |
| Spectrum Bar | Gradient from light to dark Primary Blue |
| Persona Boxes | 130 x 90 px each |
| Label Font | Open Sans Regular, 12pt |

**Styling Details:**
- Horizontal gradient bar: Light gray → Primary Blue (left to right)
- "Generic" label: Light gray
- "Specific" label: Primary Blue
- Persona boxes: Increasing opacity/saturation left to right
- Sub-labels in italics below each box
- Arrows from spectrum to persona boxes

**Caption:** "Figure 10.3: The persona spectrum from generic assistants to fully characterized AI personalities."

**Position in Chapter:** Within "Persona Design Principles" section

**Notes:** Consider icons in each persona box representing their domain.

---

## Chapter 11: Multi-Turn Conversation Design

### Figure 11.1: Single-Turn vs Multi-Turn Comparison

**Visual ID:** SPH-11.1

**Type:** Process Comparison Diagram

**Title:** Single-Turn vs Multi-Turn Conversations

**Chapter Reference:** Chapter 11 - Multi-Turn Conversation Design

**Purpose:** To illustrate the fundamental difference between single-turn (self-contained) and multi-turn (context-carrying) conversations.

**Content Description:**
Two diagrams: Single-Turn shows Prompt → Response as isolated exchange. Multi-Turn shows Prompt 1 → Response 1, with context carrying forward to Prompt 2 → Response 2, and continuing to Prompt 3 → Response 3.

**ASCII Source:**
```
SINGLE-TURN
┌──────────┐       ┌──────────┐
│  Prompt  │──────▶│ Response │
└──────────┘       └──────────┘

MULTI-TURN
┌──────────┐       ┌──────────┐
│ Prompt 1 │──────▶│Response 1│─────┐
└──────────┘       └──────────┘     │
                                    │ Context carries forward
┌──────────┐       ┌──────────┐     │
│ Prompt 2 │──────▶│Response 2│◀────┘
└──────────┘       └──────────┘     │
                                    │
┌──────────┐       ┌──────────┐     │
│ Prompt 3 │──────▶│Response 3│◀────┘
└──────────┘       └──────────┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 550 x 400 px |
| Format | SVG (scalable) |
| Background | White (#FFFFFF) |
| Prompt Boxes | Primary Blue fill |
| Response Boxes | Secondary Teal fill |
| Context Arrows | Accent Orange, dashed |

**Styling Details:**
- Single-Turn section: Clean, simple layout at top
- Multi-Turn section: Shows vertical progression with context lines
- "Context carries forward" annotation with curved arrow
- Context lines: Dashed Accent Orange, indicating information flow
- Turn numbers in badges

**Caption:** "Figure 11.1: Single-turn conversations are self-contained, while multi-turn conversations build context across exchanges."

**Position in Chapter:** At the start of "Understanding Multi-Turn Conversations" section

**Notes:** Animate context flow for interactive version.

---

### Figure 11.2: Conversation Flow Structures

**Visual ID:** SPH-11.2

**Type:** Four-Quadrant Flow Diagram

**Title:** Conversation Flow Structures

**Chapter Reference:** Chapter 11 - Multi-Turn Conversation Design

**Purpose:** To show four common conversation flow patterns: Linear, Branching, Loop, and Hub-and-Spoke.

**Content Description:**
Four flow diagrams: Linear Flow (Start → Step 1 → Step 2 → Step 3 → End), Branching Flow (Start splitting to Path A/B/C leading to End A/B/C), Loop Flow (Start → Process → Decision with iteration loop back to Process, or to End), Hub-and-Spoke (Start → Hub with spokes to Topics A/B/C, then to End).

**ASCII Source:**
```
Linear Flow:
Start → Step 1 → Step 2 → Step 3 → End

Branching Flow:
        ┌─→ Path A → End A
Start ──┼─→ Path B → End B
        └─→ Path C → End C

Loop Flow:
Start → Process → Decision ─→ End
            ↑          │
            └──────────┘
            (iterate)

Hub-and-Spoke:
            ┌─ Topic A ─┐
            │           │
Start ─→ Hub ─ Topic B ─┤─→ End
            │           │
            └─ Topic C ─┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 700 x 500 px |
| Format | SVG (scalable) |
| Background | Light Gray (#F5F5F5) |
| Section Layout | 2x2 grid |
| Node Size | 60 x 30 px |
| Font | Open Sans Regular, 11pt |

**Styling Details:**
- Linear: Simple horizontal chain, Primary Blue
- Branching: Tree structure, Secondary Teal
- Loop: Circular flow with decision diamond, Accent Orange
- Hub-and-Spoke: Central hub with radiating spokes, Success Green
- Each quadrant clearly labeled
- Consistent node styling within each quadrant
- Arrows with clear directionality

**Caption:** "Figure 11.2: Four common conversation flow structures—choose based on task requirements and user interaction patterns."

**Position in Chapter:** Within "Conversation Flow Design" section

**Notes:** Each quadrant should be visually distinct but use consistent styling language.

---

### Figure 11.3: Conversation State Types

**Visual ID:** SPH-11.3

**Type:** Three-Section Stack Diagram

**Title:** Conversation State

**Chapter Reference:** Chapter 11 - Multi-Turn Conversation Design

**Purpose:** To show the three types of state that must be tracked in multi-turn conversations: User State, Task State, and Context State.

**Content Description:**
Three stacked sections within a container: USER STATE (Identified preferences, Expressed needs, Skill/knowledge level, Emotional state), TASK STATE (Current stage of task, Completed steps, Pending items, Decisions made), CONTEXT STATE (Established facts, Shared references, Previously discussed topics, Agreed definitions).

**ASCII Source:**
```
┌─────────────────────────────────────────────────────────────────┐
│                    CONVERSATION STATE                           │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │ USER STATE                                               │   │
│  │ • Identified preferences                                │   │
│  │ • Expressed needs                                       │   │
│  │ • Skill/knowledge level                                 │   │
│  │ • Emotional state                                       │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │ TASK STATE                                               │   │
│  │ • Current stage of task                                 │   │
│  │ • Completed steps                                       │   │
│  │ • Pending items                                         │   │
│  │ • Decisions made                                        │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │ CONTEXT STATE                                            │   │
│  │ • Established facts                                     │   │
│  │ • Shared references                                     │   │
│  │ • Previously discussed topics                           │   │
│  │ • Agreed definitions                                    │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 650 x 450 px |
| Format | SVG (scalable) |
| Background | White (#FFFFFF) |
| Border | 2px solid Primary Blue |
| Section Height | 110 px each |
| Title Font | Open Sans Bold, 14pt |
| Content Font | Open Sans Regular, 12pt |

**Styling Details:**
- USER STATE: Primary Blue header, person icon
- TASK STATE: Secondary Teal header, checklist icon
- CONTEXT STATE: Accent Orange header, document icon
- Bullet points in matching header colors
- Visual icons in header left side
- Clear visual separation between sections

**Caption:** "Figure 11.3: The three types of conversational state that must be tracked across multi-turn interactions."

**Position in Chapter:** Within "State Management" section

**Notes:** Icons help quickly identify each state type at a glance.

---

## Summary Statistics

| Part | Chapters | Figures | Tables | Total Visuals |
|:-----|:---------|:--------|:-------|:--------------|
| Part III | 8-11 | 10 | 0 | 10 |

### Figures by Chapter

| Chapter | Figure Count | Visual IDs |
|:--------|:-------------|:-----------|
| Chapter 8 | 3 | SPH-8.1, SPH-8.2, SPH-8.3 |
| Chapter 9 | 4 | SPH-9.1, SPH-9.2, SPH-9.3, SPH-9.4 |
| Chapter 10 | 3 | SPH-10.1, SPH-10.2, SPH-10.3 |
| Chapter 11 | 3 | SPH-11.1, SPH-11.2, SPH-11.3 |

### Implementation Priority

| Priority | Visual IDs | Rationale |
|:---------|:-----------|:----------|
| High | SPH-8.1, SPH-8.2 | Core CoT concepts referenced throughout |
| High | SPH-10.1, SPH-10.2 | Essential system prompt architecture |
| High | SPH-11.1 | Fundamental multi-turn distinction |
| Medium | SPH-9.2, SPH-9.4 | Process and optimization guidance |
| Medium | SPH-8.3, SPH-11.2, SPH-11.3 | Decision guides and state management |
| Standard | SPH-9.1, SPH-9.3, SPH-10.3 | Supporting concepts |

---

*Source: Structured Prompting Handbook - https://zettai-seigi.github.io/StructuredPromptingHandbook/*
