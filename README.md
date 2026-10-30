<p align="center">
  <a href="README.md">English</a> | <a href="README_CN.md">中文</a>
</p>

<h1 align="center">High-Taste Technical Writing Engine</h1>

<p align="center">
  <strong>A writing skill specification for technical content that values taste, authorship, engineering judgment, and restraint.</strong>
  <br/>
  Built for project write-ups, technical blogs, release posts, architecture notes, and product-level technical storytelling.
</p>

<p align="center">
  <img src="https://img.shields.io/badge/style-high--taste-black?style=flat-square" alt="style"/>
  <img src="https://img.shields.io/badge/focus-authorial%20voice-blue?style=flat-square" alt="voice"/>
  <img src="https://img.shields.io/badge/priority-taste%20first-purple?style=flat-square" alt="priority"/>
  <img src="https://img.shields.io/badge/license-MIT-green?style=flat-square" alt="license"/>
</p>

---

## About

**High-Taste Technical Writing Engine** is a platform-agnostic writing skill specification for generating technical content with a clear authorial voice, strong engineering judgment, and disciplined restraint.

It is not designed to produce generic promotional copy. It is designed to help AI systems write like a thoughtful technical author: precise, credible, structured, readable, and distinct.

This repository packages the skill as a reusable open project so it can be applied across major AI platforms, prompt frameworks, and writing workflows.

---

## Why this exists

A large amount of AI-generated technical writing fails in the same predictable ways:

- it sounds correct, but not written
- it is fluent, but empty
- it lists features, but explains no value
- it tries to be persuasive, but loses credibility
- it sounds like a template instead of a real author

This project exists to solve that problem.

The goal is not to make writing louder. The goal is to make it better:

- more precise
- more readable
- more trustworthy
- more distinctive
- more useful in real technical contexts

---

## Core philosophy

The highest priority of this skill is **taste**.

In this project, taste means:

- clear judgment
- disciplined language
- avoidance of cheap emphasis
- sensitivity to tone
- respect for engineering reality
- writing that feels authored rather than assembled

This comes before growth tricks, before SEO tricks, and before empty enthusiasm.

That does **not** mean discoverability, conversion, structure, or clarity are unimportant. They matter. But they must serve the writing instead of degrading it.

---

## What this skill is for

Use this skill when you want an AI system to generate:

- technical blog posts
- open-source project introductions
- GitHub project descriptions
- release announcements
- architecture write-ups
- engineering retrospectives
- product or platform technical explainers
- implementation notes
- technical landing-page style longform content

It is especially useful when the writing must balance:

- professionalism and readability
- technical depth and accessibility
- discoverability and credibility
- conversion and restraint

---

## What makes this skill different

### 1. Taste comes first
This skill treats taste and authorial quality as first-class constraints, not decorative extras.

### 2. It rejects generic AI voice
It explicitly suppresses template phrasing, inflated praise, empty summary language, and synthetic enthusiasm.

### 3. It favors engineering judgment over feature dumping
Instead of just listing capabilities, it explains why design choices matter, what problem they solve, and where the trade-offs are.

### 4. It is platform-agnostic
It can be used in ChatGPT, Claude, Gemini, DeepSeek, prompt orchestration tools, internal copilots, or custom LLM pipelines.

### 5. It supports discoverability without sacrificing dignity
It allows SEO, search relevance, and conversion optimization, but only when done naturally and without turning the writing into ad copy.

---

## Design goals

This skill is designed to produce writing that is:

- authored, not assembled
- persuasive, but not oily
- clear, but not bland
- structured, but not mechanical
- opinionated, but not theatrical
- discoverable, but not keyword-stuffed
- useful, not decorative

---

## Repository structure

```text
high-taste-technical-writing-engine/
├── README.md
├── README_CN.md
├── SKILL.md              ← single-file skill, import directly
├── LICENSE
├── skill/
│   ├── skill.md
│   ├── skill.cn.md
│   ├── quickstart.md
│   └── quickstart.cn.md
├── docs/
│   ├── writing-principles.md
│   ├── platform-adaptation.md
│   ├── anti-patterns.md
│   └── examples.md
└── examples/
    ├── input-template.md
    ├── output-outline.md
    └── prompt-template.md
```

---

## Quick start

### Option 0: Import the single-file SKILL.md (Claude Code / direct skill import)

The repo root `SKILL.md` is a self-contained, import-ready version of the full skill. To use it with Claude Code or any agent that loads skills from a directory:

```bash
mkdir -p ~/.claude/skills/high-taste-technical-writing
cp SKILL.md ~/.claude/skills/high-taste-technical-writing/SKILL.md
```

Restart the session and the skill will be auto-discovered and applied whenever you write technical content. It carries its own frontmatter (a `name` and a trigger-based `description`) so agents know when to load it.

### Option 1: Use the full skill as a system or developer prompt

Take the content in `skill/skill.md` and use it as a high-priority instruction block in your AI platform.

Then provide:

1. the source material
2. the target platform
3. the target audience
4. the intended action or outcome
5. the desired output format

### Option 2: Use the short prompt template

Use `examples/prompt-template.md` when you need a lighter-weight version for repeated workflows.

### Option 3: Adapt per platform

Use `docs/platform-adaptation.md` to map the skill into:

- system prompts
- developer prompts
- reusable prompt libraries
- custom assistant instructions
- workflow nodes in orchestration tools

---

## Recommended workflow

1. Define the writing task clearly
2. Identify the audience and purpose
3. Provide source material, not vague summaries
4. Load the skill instructions
5. Ask for a full draft
6. Review against the quality checklist
7. Refine tone, emphasis, and conversion points if needed

This skill works best when the source material is real and specific. It is not intended to fabricate depth where none exists.

---

## Quality standard

A good output generated under this skill should:

- sound like a real technical author
- avoid obvious AI phrasing
- explain problems before selling solutions
- describe design choices, not just outcomes
- use precise language rather than inflated adjectives
- maintain restraint even in promotional contexts
- guide the reader naturally toward the next action

If the result sounds like a brochure, the skill has not been followed correctly.

---

## Writing principles

The most important writing principles in this project are:

### Start from a real problem
Do not begin with praise. Begin with reality.

### Explain value, not just features
A feature list is not an argument.

### Prefer mechanisms over adjectives
Say what it does, why it matters, and where it fits.

### Write with judgment
The writing may have opinions, but they must come from analysis and experience.

### Stay restrained
Even promotional content should sound credible.

### Preserve authorial presence
The reader should feel that someone wrote this on purpose.

---

## Anti-patterns this skill tries to prevent

- generic “in today’s world” openings
- exaggerated praise without evidence
- repetitive “powerful / robust / comprehensive” language
- sterile list-only descriptions
- forced excitement
- SEO stuffing
- hard-sell calls to action
- fake neutrality that erases point of view

---

## Documentation

### Skill files
- `SKILL.md`: single-file, import-ready skill (Claude Code / direct skill import)
- `skill/skill.md`: full English skill specification
- `skill/skill.cn.md`: full Chinese skill specification
- `skill/quickstart.md`: fast usage guide in English
- `skill/quickstart.cn.md`: fast usage guide in Chinese

### Supporting docs
- `docs/writing-principles.md`: writing principles and standards
- `docs/platform-adaptation.md`: how to adapt the skill to different AI platforms
- `docs/anti-patterns.md`: failure modes and what to avoid
- `docs/examples.md`: example usage patterns

### Templates
- `examples/input-template.md`: what to provide as input
- `examples/output-outline.md`: default output structure
- `examples/prompt-template.md`: reusable short-form prompt template

---

## Example use cases

- Turn a raw GitHub README into a CSDN article without sounding like AI
- Turn a technical project into a release post with better search relevance and stronger credibility
- Turn architecture notes into a readable engineering article
- Turn an internal technical summary into a public-facing blog post without losing rigor
- Turn a product description into a technical explainer with actual judgment and structure

---

## Who this is for

This project is useful for:

- engineers who publish technical content
- open-source maintainers
- developer advocates who dislike marketing language
- technical founders
- architects and staff engineers
- AI workflow builders who want better writing outputs
- teams building internal writing copilots

---

## Usage notes

This skill is intentionally strict.

It will often produce writing that feels more grounded and less “excited” than typical AI marketing output. That is a feature, not a bug.

If a platform tends to over-praise, over-summarize, or over-smooth text, this skill should be placed as high as possible in the instruction hierarchy.

---

## Contributing

Contributions are welcome, especially in these areas:

- additional platform adaptation guides
- more examples across writing scenarios
- anti-pattern libraries
- benchmark comparisons across AI platforms
- refinements to the skill language while preserving its standards

Please keep the bar high. This repository is not trying to become a generic prompt dump.

---

## License

This project is licensed under the MIT License.

---

## Language switch

- English: `README.md`
- 中文：`README_CN.md`

---

