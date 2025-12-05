---
layout: default
title: "Part V: Governance and Ethics - Visual Reference"
nav_exclude: true
---

# Part V: Governance and Ethics - Visual Reference
{: .fs-9 }

Detailed Visual Specifications for Chapters 15-16
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
| Success Green | #28A745 | Positive indicators, safe |
| Warning Red | #DC3545 | Negative indicators, risk |
| Warning Yellow | #FFC107 | Caution indicators |

---

## Chapter 15: Responsible AI Prompting

### Figure 15.1: Responsible AI Pyramid

**Visual ID:** SPH-15.1

**Type:** Pyramid/Triangle Diagram

**Title:** Responsible AI Pyramid

**Chapter Reference:** Chapter 15 - Responsible AI Prompting

**Purpose:** To show the hierarchical layers of responsible AI considerations, from foundational accuracy to peak social impact.

**Content Description:**
A pyramid diagram with five layers from bottom to top: ACCURACY & TRUTH (Foundation: Build on truth) → SAFETY & HARM PREVENTION (Layer 1: Prevent direct harm) → FAIRNESS & BIAS (Layer 2: Ensure fairness) → TRANSPARENCY & EXPLAINABILITY (Layer 3: Be transparent) → SOCIAL IMPACT (Peak: Consider broader impact).

**ASCII Source:**
```
┌─────────────────────────────────────────────────────────────────┐
│                 RESPONSIBLE AI PYRAMID                          │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│                          /\                                     │
│                         /  \                                    │
│                        /    \                                   │
│                       /SOCIAL\                                  │
│                      / IMPACT \                                 │
│                     /──────────\                                │
│                    /            \                               │
│                   / TRANSPARENCY \                              │
│                  /   & EXPLAIN.   \                             │
│                 /──────────────────\                            │
│                /                    \                           │
│               /    FAIRNESS &        \                          │
│              /       BIAS             \                         │
│             /────────────────────────────\                      │
│            /                              \                     │
│           /      SAFETY & HARM             \                    │
│          /        PREVENTION                \                   │
│         /────────────────────────────────────\                  │
│        /                                      \                 │
│       /         ACCURACY & TRUTH               \                │
│      /                                          \               │
│     /────────────────────────────────────────────\              │
│                                                                 │
│  Foundation: Build on truth                                     │
│  Layer 1: Prevent direct harm                                   │
│  Layer 2: Ensure fairness                                       │
│  Layer 3: Be transparent                                        │
│  Peak: Consider broader impact                                  │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 650 x 500 px |
| Format | SVG (scalable) |
| Background | White (#FFFFFF) |
| Pyramid Layers | Graduated colors bottom to top |
| Title Font | Open Sans Bold, 18pt |
| Layer Labels | Open Sans Bold, 12pt |
| Description Font | Open Sans Regular, 11pt |

**Styling Details:**
- ACCURACY & TRUTH (base): Primary Blue (#2E5090) - widest
- SAFETY & HARM: Secondary Teal (#1E8A7E)
- FAIRNESS & BIAS: Accent Orange (#E07B39)
- TRANSPARENCY: Success Green (#28A745)
- SOCIAL IMPACT (peak): Warning Yellow (#FFC107) - smallest
- Layer descriptions aligned to right of pyramid
- Gradient fills from darker at base to lighter at top
- 3D effect with shadow on right side

**Caption:** "Figure 15.1: The Responsible AI Pyramid—foundational accuracy supports safety, fairness, transparency, and ultimately positive social impact."

**Position in Chapter:** At the start of "The Responsibility Framework" section

**Notes:** Pyramid shape reinforces that higher layers depend on foundational ones.

---

### Figure 15.2: Types of Bias Diagram

**Visual ID:** SPH-15.2

**Type:** Three-Column Flow Diagram

**Title:** Types of Bias

**Chapter Reference:** Chapter 15 - Responsible AI Prompting

**Purpose:** To illustrate how prompt bias combines with model bias to produce output bias, and what can be controlled.

**Content Description:**
Three columns showing: PROMPT BIAS (Biased framing, Skewed examples) + MODEL BIAS (Training data bias, Algorithmic patterns) = OUTPUT BIAS (Biased outcomes, Unfair impacts). Bottom annotation: "What you can control | What you can't | What you must check".

**ASCII Source:**
```
┌─────────────────────────────────────────────────────────────────┐
│                    TYPES OF BIAS                                │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  PROMPT BIAS            MODEL BIAS          OUTPUT BIAS         │
│  ┌─────────────┐       ┌─────────────┐     ┌─────────────┐     │
│  │ Biased      │       │ Training    │     │ Biased      │     │
│  │ framing     │       │ data bias   │     │ outcomes    │     │
│  │             │   +   │             │  =  │             │     │
│  │ Skewed      │       │ Algorithmic │     │ Unfair      │     │
│  │ examples    │       │ patterns    │     │ impacts     │     │
│  └─────────────┘       └─────────────┘     └─────────────┘     │
│                                                                 │
│  What you can control  What you can't     What you must check  │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 700 x 280 px |
| Format | SVG (scalable) |
| Background | Light Gray (#F5F5F5) |
| Column Boxes | 180 x 120 px each |
| Operator Font | Open Sans Bold, 24pt |
| Label Font | Open Sans Bold, 14pt |
| Content Font | Open Sans Regular, 12pt |

**Styling Details:**
- PROMPT BIAS: Primary Blue header, user-controllable indicator
- MODEL BIAS: Dark Gray header, non-controllable indicator
- OUTPUT BIAS: Warning Red header, must-check indicator
- "+" and "=" operators in large bold font
- Bottom annotations in italic, matching column colors
- Visual connection lines between columns
- Flow direction left to right

**Caption:** "Figure 15.2: Bias flows from prompts and models to outputs—control what you can, check what you must."

**Position in Chapter:** Within "Bias Awareness and Mitigation" section

**Notes:** Emphasize that prompt bias is controllable while model bias is not directly controllable.

---

### Figure 15.3: Harm Categories Grid

**Visual ID:** SPH-15.3

**Type:** Four-Quadrant Grid Diagram

**Title:** Harm Categories

**Chapter Reference:** Chapter 15 - Responsible AI Prompting

**Purpose:** To categorize four types of potential harm from AI systems: Direct, Indirect, Individual, and Societal.

**Content Description:**
A 2x2 grid showing: DIRECT HARM (Dangerous info, Harmful instructions, Hateful content, Illegal activities), INDIRECT HARM (Misinformation, Manipulation, Deception, Unfair advantage), INDIVIDUAL HARM (Privacy violation, Emotional distress, Financial loss, Reputation damage), SOCIETAL HARM (Discrimination, Trust erosion, Job displacement, Power concentration).

**ASCII Source:**
```
┌─────────────────────────────────────────────────────────────────┐
│                    HARM CATEGORIES                              │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  DIRECT HARM                      INDIRECT HARM                 │
│  ┌───────────────────────┐       ┌───────────────────────┐     │
│  │ • Dangerous info      │       │ • Misinformation      │     │
│  │ • Harmful instructions│       │ • Manipulation        │     │
│  │ • Hateful content     │       │ • Deception           │     │
│  │ • Illegal activities  │       │ • Unfair advantage    │     │
│  └───────────────────────┘       └───────────────────────┘     │
│                                                                 │
│  INDIVIDUAL HARM                  SOCIETAL HARM                 │
│  ┌───────────────────────┐       ┌───────────────────────┐     │
│  │ • Privacy violation   │       │ • Discrimination      │     │
│  │ • Emotional distress  │       │ • Trust erosion       │     │
│  │ • Financial loss      │       │ • Job displacement    │     │
│  │ • Reputation damage   │       │ • Power concentration │     │
│  └───────────────────────┘       └───────────────────────┘     │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 700 x 350 px |
| Format | SVG (scalable) |
| Background | White (#FFFFFF) |
| Quadrant Size | 300 x 130 px each |
| Header Font | Open Sans Bold, 14pt |
| Content Font | Open Sans Regular, 12pt |

**Styling Details:**
- DIRECT HARM: Warning Red header and accent
- INDIRECT HARM: Accent Orange header and accent
- INDIVIDUAL HARM: Secondary Teal header and accent
- SOCIETAL HARM: Primary Blue header and accent
- Each quadrant has matching colored left border
- Bullet points in matching colors
- Subtle dividing lines between quadrants

**Caption:** "Figure 15.3: Four categories of AI harm—from direct and indirect effects to individual and societal impacts."

**Position in Chapter:** Within "Harm Prevention" section

**Notes:** Color-coding helps identify harm severity (red = most direct/severe).

---

### Table 15.1: The 6 Principles of Responsible AI

**Visual ID:** SPH-T15.1

**Type:** Reference Table

**Title:** 6 Principles of Responsible AI Prompting

**Chapter Reference:** Chapter 15 - Responsible AI Prompting

**Purpose:** To provide a quick reference for the six core ethical principles.

**Content Description:**
| # | Principle | Description |
|:-:|:----------|:------------|
| 1 | Accuracy | Prompts should seek truthful, correct information |
| 2 | Safety | Prompts should not enable harm |
| 3 | Fairness | Prompts should not discriminate or bias |
| 4 | Transparency | AI nature and limitations should be clear |
| 5 | Privacy | Personal data should be protected |
| 6 | Accountability | Humans remain responsible for AI use |

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Table Width | 100% content width |
| Header | Primary Blue background, white text |
| Rows | Alternating Light Gray/White |
| Number Column | Centered, bold |
| Principle Column | Bold, colored badges |

**Caption:** "Table 15.1: The six principles of responsible AI prompting that guide ethical AI interactions."

**Position in Chapter:** Within "Core Ethical Principles" section

---

## Chapter 16: Security, Privacy, and Compliance

### Figure 16.1: Security Risk Landscape

**Visual ID:** SPH-16.1

**Type:** Four-Quadrant Risk Grid

**Title:** Security Risk Landscape

**Chapter Reference:** Chapter 16 - Security, Privacy, and Compliance

**Purpose:** To categorize security risks into four areas: Prompt-Level, System-Level, User-Level, and Output-Level.

**Content Description:**
A 2x2 grid showing: PROMPT-LEVEL RISKS (Prompt injection, Jailbreaking, Data leakage, Social engineering), SYSTEM-LEVEL RISKS (API key exposure, Data exfiltration, Unauthorized use, Model extraction), USER-LEVEL RISKS (Oversharing PII, Unintended disclosure, Trust exploitation, Privacy violation), OUTPUT-LEVEL RISKS (Sensitive info, Harmful content, Malicious code, Misinformation).

**ASCII Source:**
```
┌─────────────────────────────────────────────────────────────────┐
│                    SECURITY RISK LANDSCAPE                      │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  PROMPT-LEVEL RISKS          SYSTEM-LEVEL RISKS                 │
│  ┌───────────────────┐      ┌───────────────────┐              │
│  │ • Prompt injection │      │ • API key exposure │              │
│  │ • Jailbreaking     │      │ • Data exfiltration│              │
│  │ • Data leakage     │      │ • Unauthorized use │              │
│  │ • Social engineer. │      │ • Model extraction │              │
│  └───────────────────┘      └───────────────────┘              │
│                                                                 │
│  USER-LEVEL RISKS            OUTPUT-LEVEL RISKS                 │
│  ┌───────────────────┐      ┌───────────────────┐              │
│  │ • Oversharing PII  │      │ • Sensitive info   │              │
│  │ • Unintended disc. │      │ • Harmful content  │              │
│  │ • Trust exploitation│     │ • Malicious code   │              │
│  │ • Privacy violation│      │ • Misinformation   │              │
│  └───────────────────┘      └───────────────────┘              │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 700 x 350 px |
| Format | SVG (scalable) |
| Background | Light Gray (#F5F5F5) |
| Quadrant Size | 280 x 130 px each |
| Header Font | Open Sans Bold, 13pt |
| Content Font | Open Sans Regular, 11pt |

**Styling Details:**
- PROMPT-LEVEL: Warning Red header (highest risk focus)
- SYSTEM-LEVEL: Primary Blue header
- USER-LEVEL: Accent Orange header
- OUTPUT-LEVEL: Secondary Teal header
- Each quadrant has matching shield/lock icon
- Bullet points in Dark Gray
- Border around each quadrant in matching color

**Caption:** "Figure 16.1: The four categories of security risks in AI prompting—from prompt-level to output-level threats."

**Position in Chapter:** At the start of "Security Risks in AI Prompting" section

**Notes:** Use security-themed icons (shield, lock) to reinforce the topic.

---

### Figure 16.2: AI Policy Framework

**Visual ID:** SPH-16.2

**Type:** Hierarchical Tier Diagram

**Title:** AI Policy Framework

**Chapter Reference:** Chapter 16 - Security, Privacy, and Compliance

**Purpose:** To show the four tiers of organizational AI policy from high-level principles to technical standards.

**Content Description:**
Four stacked tiers: TIER 1: AI USE POLICY (High-level principles and governance) → TIER 2: DOMAIN POLICIES (Customer Service | HR | Marketing | Development) → TIER 3: OPERATIONAL PROCEDURES (Prompt reviews | Testing | Monitoring | Incident response) → TIER 4: TECHNICAL STANDARDS (Prompt templates | Security controls | Data handling).

**ASCII Source:**
```
┌─────────────────────────────────────────────────────────────────┐
│                    AI POLICY FRAMEWORK                          │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │ TIER 1: AI USE POLICY                                    │   │
│  │ High-level principles and governance                     │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │ TIER 2: DOMAIN POLICIES                                  │   │
│  │ Customer Service │ HR │ Marketing │ Development          │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │ TIER 3: OPERATIONAL PROCEDURES                           │   │
│  │ Prompt reviews │ Testing │ Monitoring │ Incident response│   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
│  ┌─────────────────────────────────────────────────────────┐   │
│  │ TIER 4: TECHNICAL STANDARDS                              │   │
│  │ Prompt templates │ Security controls │ Data handling     │   │
│  └─────────────────────────────────────────────────────────┘   │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 700 x 400 px |
| Format | SVG (scalable) |
| Background | White (#FFFFFF) |
| Tier Boxes | 600 x 70 px each |
| Title Font | Open Sans Bold, 18pt |
| Tier Font | Open Sans Bold, 14pt |
| Content Font | Open Sans Regular, 12pt |

**Styling Details:**
- TIER 1: Primary Blue, widest visual weight (governance)
- TIER 2: Secondary Teal, multiple domain columns
- TIER 3: Accent Orange, operational icons
- TIER 4: Success Green, technical symbols
- Vertical connector line on left showing hierarchy
- Each tier slightly narrower than one above for pyramid effect
- Sub-items separated by | dividers

**Caption:** "Figure 16.2: Four-tier AI policy framework from high-level governance to technical implementation standards."

**Position in Chapter:** Within "Organizational AI Policies" section

**Notes:** Pyramid-like narrowing reinforces hierarchy concept.

---

### Figure 16.3: Incident Response Process

**Visual ID:** SPH-16.3

**Type:** Six-Stage Process Flow Diagram

**Title:** Incident Response Process

**Chapter Reference:** Chapter 16 - Security, Privacy, and Compliance

**Purpose:** To illustrate the six steps of AI security incident response: Detect, Assess, Contain, Eradicate, Recover, Improve.

**Content Description:**
A circular/linear flow showing: 1. DETECT (Identify incident) → 2. ASSESS (Determine severity) → 3. CONTAIN (Stop impact) → 4. ERADICATE (Remove cause) → 5. RECOVER (Resume normal) → 6. IMPROVE (Update controls).

**ASCII Source:**
```
┌─────────────────────────────────────────────────────────────────┐
│                 INCIDENT RESPONSE PROCESS                       │
├─────────────────────────────────────────────────────────────────┤
│                                                                 │
│   1. DETECT         2. ASSESS           3. CONTAIN             │
│   ┌─────────┐      ┌─────────┐        ┌─────────┐             │
│   │Identify │─────▶│Determine│───────▶│ Stop    │             │
│   │incident │      │severity │        │ impact  │             │
│   └─────────┘      └─────────┘        └─────────┘             │
│                                             │                   │
│                                             ▼                   │
│   6. IMPROVE       5. RECOVER          4. ERADICATE            │
│   ┌─────────┐      ┌─────────┐        ┌─────────┐             │
│   │ Update  │◀─────│ Resume  │◀───────│ Remove  │             │
│   │ controls│      │ normal  │        │ cause   │             │
│   └─────────┘      └─────────┘        └─────────┘             │
│                                                                 │
└─────────────────────────────────────────────────────────────────┘
```

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Dimensions | 700 x 300 px |
| Format | SVG (scalable) |
| Background | Light Gray (#F5F5F5) |
| Step Boxes | 100 x 60 px each |
| Number Badges | 24px circular |
| Font | Open Sans Regular, 12pt |

**Styling Details:**
- Steps 1-3 (top row): Warning Red → Accent Orange → Warning Yellow
- Steps 4-6 (bottom row): Secondary Teal → Success Green → Primary Blue
- Number badges: White text on colored circles
- Flow arrows: Dark Gray, 2px stroke
- U-shaped flow pattern (right then down then left)
- Action verbs in bold below each step

**Caption:** "Figure 16.3: The six-step incident response process—from detection through recovery and improvement."

**Position in Chapter:** Within "Incident Response" section

**Notes:** Color progression suggests urgency cooling from red (detect) to green (recover) to blue (improve).

---

### Table 16.1: PII Handling Guidelines

**Visual ID:** SPH-T16.1

**Type:** Reference Table

**Title:** PII Handling Guidelines

**Chapter Reference:** Chapter 16 - Security, Privacy, and Compliance

**Purpose:** To provide clear guidance on what personal data can be included in prompts.

**Content Description:**
| Data Type | Include in Prompts? | If Necessary |
|:----------|:--------------------|:-------------|
| Full name | Avoid | Use initials or pseudonyms |
| Email | Avoid | Partial masking |
| Phone | No | Never include |
| SSN | Never | Never include |
| Address | Avoid | Generalize (city only) |
| Credit card | Never | Never include |
| Medical info | No | Generalize heavily |
| Financial details | Avoid | Aggregate only |

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Table Width | 100% content width |
| Header | Primary Blue background, white text |
| "Never" rows | Warning Red background tint |
| "No" rows | Accent Orange background tint |
| "Avoid" rows | Warning Yellow background tint |

**Caption:** "Table 16.1: PII handling guidelines—know what data can and cannot be included in AI prompts."

**Position in Chapter:** Within "Data Privacy Protection" section

---

### Table 16.2: Regulatory Landscape

**Visual ID:** SPH-T16.2

**Type:** Reference Table

**Title:** Regulatory Landscape

**Chapter Reference:** Chapter 16 - Security, Privacy, and Compliance

**Purpose:** To summarize key regulations affecting AI prompting.

**Content Description:**
| Regulation | Region | Focus | AI Impact |
|:-----------|:-------|:------|:----------|
| GDPR | EU | Data protection | Processing, consent |
| CCPA | California | Consumer privacy | Data rights |
| HIPAA | US | Health information | PHI protection |
| SOX | US | Financial reporting | Data integrity |
| PCI-DSS | Global | Payment data | Card data protection |

**Specifications:**

| Attribute | Value |
|:----------|:------|
| Table Width | 100% content width |
| Header | Secondary Teal background, white text |
| Regulation Column | Bold |
| Region Column | Centered |

**Caption:** "Table 16.2: Key regulations affecting AI prompting by region and focus area."

**Position in Chapter:** Within "Compliance Requirements" section

---

## Summary Statistics

| Part | Chapters | Figures | Tables | Total Visuals |
|:-----|:---------|:--------|:-------|:--------------|
| Part V | 15-16 | 6 | 3 | 9 |

### Figures by Chapter

| Chapter | Figure Count | Visual IDs |
|:--------|:-------------|:-----------|
| Chapter 15 | 3 | SPH-15.1, SPH-15.2, SPH-15.3 |
| Chapter 16 | 3 | SPH-16.1, SPH-16.2, SPH-16.3 |

### Implementation Priority

| Priority | Visual IDs | Rationale |
|:---------|:-----------|:----------|
| High | SPH-15.1 | Core responsible AI framework |
| High | SPH-16.1, SPH-16.2 | Security and policy fundamentals |
| Medium | SPH-15.2, SPH-15.3 | Bias and harm understanding |
| Medium | SPH-16.3 | Incident response process |
| Standard | Tables | Reference materials |

---

*Source: Structured Prompting Handbook - https://zettai-seigi.github.io/StructuredPromptingHandbook/*
