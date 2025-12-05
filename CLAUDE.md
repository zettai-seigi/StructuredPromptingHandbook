# CLAUDE.md - Project Instructions

## Project Overview

This is the **Structured Prompting Handbook** - a comprehensive guide to effective AI prompting techniques, frameworks, and best practices.

## Structure

```
StructuredPromptingHandbook/
├── docs/                          # GitHub Pages content
│   ├── _config.yml               # Jekyll configuration
│   ├── index.md                  # Home page
│   ├── chapters.md               # Table of contents
│   ├── part-*.md                 # Part landing pages (6)
│   ├── chapters/                 # All 19 chapter markdown files
│   └── assets/images/            # Diagrams and visuals (to be added)
├── README.md                     # Repository documentation
├── LICENSE                       # MIT License
├── .gitignore                    # Git ignore rules
├── CLAUDE.md                     # This file
└── CLAUDE_REPLICATION_GUIDE.md   # Replication instructions
```

## Key Frameworks

### The 7 Prompting Pillars
1. Clarity - Unambiguous communication
2. Context - Relevant background information
3. Constraint - Boundaries and limitations
4. Composition - Structure and formatting
5. Calibration - Tone, style, and persona
6. Chain - Logical sequencing and reasoning
7. Critique - Self-evaluation and refinement

### The 5 Quality Dimensions
1. Relevance - Response addresses the actual request
2. Accuracy - Information is factually correct
3. Completeness - All aspects covered
4. Coherence - Logically structured
5. Actionability - Output can be directly used

### The 4 Maturity Levels
1. Novice - Basic prompts, learning
2. Practitioner - Structured, consistent
3. Expert - Advanced, optimizing
4. Master - Designing, teaching

### The 6 Control Objectives
1. Accuracy Control - Ensure factual correctness
2. Consistency Control - Maintain reproducible outputs
3. Safety Control - Prevent harmful content
4. Privacy Control - Protect sensitive information
5. Compliance Control - Meet regulatory requirements
6. Quality Control - Maintain output standards

## Chapter Organization

- **Part I: Foundations** (Ch 1-3) - Core concepts and pillars
- **Part II: Core Frameworks** (Ch 4-7) - Architecture and design
- **Part III: Advanced Techniques** (Ch 8-11) - CoT, few-shot, personas
- **Part IV: Quality & Evaluation** (Ch 12-14) - Testing and metrics
- **Part V: Governance & Ethics** (Ch 15-16) - Responsible AI
- **Part VI: Implementation** (Ch 17-19) - Roadmap and practices

## Commands

### Local Development
```bash
cd docs
bundle install
bundle exec jekyll serve
# Open http://localhost:4000/StructuredPromptingHandbook/
```

### Git Operations
```bash
git add .
git commit -m "Description"
git push origin main
```

## Maintenance Notes

- Maintain consistent YAML frontmatter across chapters
- Cross-references use format: `/chapters/XX-slug/`
- All chapters follow: Learning Objectives → Content → Key Takeaways → Summary → Review Questions → Exercise → Navigation
- ASCII diagrams should render in monospace fonts
- Tables use markdown format compatible with Jekyll/Just the Docs
