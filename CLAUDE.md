# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Progress tracking (required)

**Maintain a running progress report** at `reports/progress-log.md` throughout development. Update it after completing each significant task (installing dependencies, creating pages, finishing stations, etc.). This provides continuity across sessions and documents decisions made.

---

## Project overview

**HAP's Learning Lab: JavaScript Control Flow** - A 6-station educational experience teaching control flow concepts through HAP's apprentice narrative. This lab extends the Robot ID Card project from JS Foundations, adding truthy/falsy values, logical operators, conditionals, functions, and loops.

### Station structure

| Station | Title                        | Demo              | Key Concepts                  |
| ------- | ---------------------------- | ----------------- | ----------------------------- |
| 1       | The Truth About Values       | Falsy Detector    | Truthy/falsy, 6 falsy values  |
| 2       | Combining Conditions         | Condition Builder | AND, OR, NOT, short-circuit   |
| 3       | Making Decisions             | Status Classifier | if/else, else if, ranges      |
| 4       | Reusable Code with Functions | Function Factory  | Parameters, return, scope     |
| 5       | Repeating Actions            | Skill Scanner     | for loops, arrays, iteration  |
| 6       | AI-Assisted Debugging        | —                 | Prompt engineering, debugging |

### Robot ID Card variables

```javascript
// From JS Foundations (prior knowledge)
const robotName = "HyBit A. ProtoBot";
const modelNumber = "HAP-7000";
const creationYear = 2024;
let energyLevel = 100;
let tasksDone = 0;
let statusMessage = "Ready to learn!";

// NEW for JS Control Flow
let nickname = ""; // Falsy (empty string)
let backupBattery = 0; // Falsy (zero)
let secondaryMission = null; // Falsy (null)
let isOnline = true; // Boolean logic
let isCharging = false; // Compound conditions
let coreTemperature = 72; // Range classification
```

### Reference implementation

See `../hap-js-foundations/` for a complete 6-station example.

## Commands

```bash
npm run dev        # Start dev server at localhost:4321
npm run build      # Production build to dist/
npm run preview    # Preview production build
```

## Architecture

### Layout system

```text
src/layouts/
├── MainLayout.astro     # Base layout with header, footer, navigation
└── StationLayout.astro  # Wraps MainLayout with station-specific props
                         # Auto-calculates prev/next navigation from stationNumber
```

Station pages pass a `stationNumber` prop (1-6) to `StationLayout`, which handles navigation links automatically.

### Component hierarchy

```text
StationLayout (stationNumber, title, subtitle, introContent, ...)
    └── MainLayout (pageTitle, navigation, footer)
        ├── Header.astro (avatar, titles)
        ├── Navigation.astro (station dots, prev/next)
        ├── <slot /> (station content)
        └── Footer.astro (copyright, reminder)
```

### Syntax highlighting

Uses Astro's built-in Shiki with `css-variables` theme, customized in `src/styles/shiki-hap-theme.css`. The `CodeBlock.astro` component wraps Astro's `<Code>` component.

Supported languages: html, css, javascript, json, markdown, bash, text, nunjucks

## Content creation workflow

1. Complete `docs/reference-cards/station-blueprint-template.md` for each station
2. Copy `src/templates/station-template.astro` to `src/pages/stations/station[N].astro`
3. Replace all `[PLACEHOLDER_*]` markers with content
4. Use `station6-template.astro` for the final station (different structure)
5. Validate with skills in `skills/` before committing
6. Run `npm run build` to verify

### Template files

| Template                                | Purpose                                |
| --------------------------------------- | -------------------------------------- |
| `src/templates/hub-template.astro`      | Landing page → `src/pages/index.astro` |
| `src/templates/station-template.astro`  | Stations 1-5                           |
| `src/templates/station6-template.astro` | Final station (different layout)       |

## HAP's voice (critical)

HAP always speaks in **first-person apprentice voice**. This is non-negotiable.

### Required patterns

- "I learned from Prof. Teeters that..."
- "When I was practicing..."
- "This was tricky for me too..."
- Share specific mistakes and what they taught

### Forbidden patterns

- "You should..." (too instructional)
- "Obviously..." or "It's simple..." (dismissive)
- "Just" or "simply" (minimizing)
- Generic statements without attribution to Prof. Teeters

See `docs/reference-cards/hap-voice-card.md` for complete guidelines.

## Characters

| Character     | Role      | Voice                                                             |
| ------------- | --------- | ----------------------------------------------------------------- |
| HAP           | Narrator  | First-person, curious, humble, uses 🟠 emoji                      |
| Prof. Teeters | Mentor    | Calm, encouraging, uses analogies (max 1 appearance per station)  |
| Grace Hopper  | Assistant | Precise, no contractions, no emojis (only when precision matters) |

## CSS requirements

**All colors must use HSL format** - never hex or rgb:

```css
/* Correct */
--warm-orange: hsl(32, 76%, 63%);

/* Wrong */
--warm-orange: #e8a557;
```

Use "CSS custom property" terminology, never "CSS variable".

## HAP images

**Never guess image filenames.** Always verify against:
`skills/hap-image-validation/hap-cloudinary-complete-inventory.md`

Common poses:

| Filename                    | Use case                       |
| --------------------------- | ------------------------------ |
| `HAP-learner_dvehmt`        | Default, footer                |
| `hap-laptop_xiewar`         | Hero, studying                 |
| `hap-waving_dgzacg`         | Greeting                       |
| `hap-broke-things_qtbum4`   | Confession callouts            |
| `hap-brain-explodes_wu0or8` | Breakthroughs (use sparingly!) |
| `hap-celebrating_bljvgl`    | Major victories                |

Cloudinary URL format:

```text
https://res.cloudinary.com/cynthia-teeters/image/upload/f_auto,q_auto,w_[WIDTH],c_limit/v[VERSION]/[FILENAME].jpg
```

## Skills for validation

Located in `skills/` directory (run with `/format skillname`):

| Skill                  | Purpose                                |
| ---------------------- | -------------------------------------- |
| `hap-voice`            | Validate first-person apprentice voice |
| `accessibility-check`  | WCAG 2.2 Level AA compliance           |
| `css-standards`        | HSL color format enforcement           |
| `station-content`      | Station structure patterns             |
| `hap-image-validation` | Verify image filenames exist           |

## Heading case conventions

- **HTML files**: Title Case ("What You'll Learn")
- **Markdown files**: Sentence case ("What you'll learn")

## Emoji usage

- 🟠 HAP's signature (tips, insights)
- 🔬 Science, research discoveries
- 😳 After Grace corrects HAP

Rules: Never in code blocks, never as decoration, max 2-3 per station.

## Copyright notice

All HTML files must include:

```html
<!--
HAP Educational Content © 2026 Cynthia Teeters. All rights reserved.
HyBit A. ProtoBot (HAP) character and the apprentice learning methodology are proprietary educational innovations.
-->
```

## Common pitfalls

1. **Don't copy from completed stations** - Always use templates from `src/templates/`
2. **Don't hallucinate HAP images** - Check the inventory file
3. **Don't use hex/rgb colors** - Use hsl() only
4. **Don't break HAP's voice** - First-person, humble, references mentor
5. **Don't overuse breakthrough images** - `hap-brain-explodes` max once per station
6. **Don't skip validation** - Run skills before committing

## Key documentation

| Document                                                | Purpose                      |
| ------------------------------------------------------- | ---------------------------- |
| `docs/designing-labs/hap-narrative-and-scene-design.md` | Complete narrative framework |
| `docs/reference-cards/hap-voice-card.md`                | HAP voice quick reference    |
| `docs/reference-cards/station-blueprint-template.md`    | Pre-writing checklist        |
| `docs/reference-cards/character-quick-ref.md`           | All three characters         |
