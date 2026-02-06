# Station 6 blueprint: AI assistance for debugging

**Purpose:** Complete this blueprint BEFORE writing any station content. Station 6 uses a unique 12-section structure focused on responsible AI use.

---

## 1. Station identity

```
Station ID: station-6-ai-debugging
Title (student-facing): AI Assistance for Debugging
Lab context: Final station - teaches responsible AI collaboration for debugging JavaScript control flow
Prerequisites: Stations 1-5 (truthy/falsy, operators, conditionals, functions, loops)
```

---

## 2. Learning intent

```
Primary concept: AI can accelerate debugging, but you own every line of code — verification is mandatory, not optional.

Supporting concepts:
- Detailed prompts produce better AI responses than vague requests
- AI consistently forgets accessibility unless explicitly asked
- Understanding the fix matters more than fixing it fast
- AI excels at pattern recognition but struggles with project-specific context

Explicit non-goals (what this station does NOT teach):
- Specific AI tools or platforms (keeps it general)
- Advanced debugging techniques (DevTools, profilers)
- Writing tests (beyond verification concepts)
- AI for code generation from scratch (focus is on debugging existing code)
```

---

## 3. Narrative design

### Characters present

```
- [x] HAP (always - narrator)
- [x] Prof. Teeters (for guidance on responsible AI use)
- [x] Grace Hopper (for precision about verification terminology)
- [ ] Other entity
```

### HAP's arc

```
Starting state: Excited that AI can fix bugs instantly — ships AI-generated fixes without testing
Key question: "How do I use AI to debug faster without breaking things or skipping learning?"
Ending state: Understands that AI is a collaborator, not a replacement — verification and understanding are non-negotiable
```

---

## 4. Prof. Teeters moments

**Frequency:** Twice - opening lesson and closing reflection

```
- [x] Opening perspective shift
- [ ] Mid-station guidance
- [x] Validation of learning (closing section)

Her key lines:
- Opening: "HAP, AI can generate code faster than you can type, but it doesn't care about your users the way you should. You own every line of code, whether you wrote it or AI did."
- Closing: "You've learned that AI is a powerful collaborator, but the responsibility never leaves your hands. Every fix you ship, you must understand."
```

---

## 5. Grace Hopper moments (if applicable)

**Frequency:** Once - on verification terminology

```
- [ ] Terminology correction
- [x] Technical precision
- [ ] Reframing question

Her key line: "Verification is not optional. The word comes from the Latin 'verus' meaning true. You must confirm the truth of every fix before it reaches users."
```

---

## 6. HAP's confessions

List 2-4 specific mistakes HAP made learning this topic:

```
1. I asked AI to "fix my code" without explaining what was wrong — it changed working code and broke three other things!
2. I copied an AI-generated fix without testing it — the bug disappeared but the fix had an infinite loop that crashed the browser. 😳
3. I let AI "improve" my function without specifying requirements — it removed the accessibility features I had carefully added.
4. I trusted AI's explanation of why my condition wasn't working — it was wrong about operator precedence and I shipped a bug to production.
```

---

## 7. Code example contract

```
Primary role: [x] Illustrative - Shows effective prompting and verification workflows

Constraints:
- Code examples must use concepts from Stations 1-5 (truthy/falsy, operators, conditionals, functions, loops)
- Examples must show realistic bugs students might encounter
- Must include accessibility considerations in debugging prompts
- Must demonstrate before/after prompt quality

Student interaction:
- What they should notice: The dramatic difference between vague and detailed prompts
- What they should NOT change: The verification workflow steps
```

---

## 8. HAP pose selection

| Location             | Pose intent            | Cognitive state     | Image filename          |
| -------------------- | ---------------------- | ------------------- | ----------------------- |
| Intro/Avatar         | Studying, learning     | Focused on laptop   | hap-laptop_xiewar       |
| Section 1 confession | Confused by AI failure | Lost, overwhelmed   | hap-confused-map_q8q0ej |
| Section 2            | Working with AI        | Productive          | hap-laptop_xiewar       |
| Closing celebration  | Celebrating mastery    | Proud, accomplished | hap-celebrating_bljvgl  |

---

## 9. Station 6 section plan (12 required sections)

```
1. What You'll Learn
   - 3 insight cards: Speed with responsibility, Detailed prompts work better, You own the code
   - HAP's confession about shipping broken AI code

2. What AI Can and Can't Do
   - Strengths: Pattern recognition, syntax errors, explaining code, suggesting fixes
   - Weaknesses: Project context, user intent, accessibility, performance optimization

3. Debugging Truthy/Falsy Issues with AI
   - Vague prompt → Bad output (breaks other conditions)
   - Detailed prompt → Good output (understands full context)

4. Debugging Conditional Logic with AI
   - More complex: nested if/else with operator precedence issues
   - Comprehensive prompt including all requirements

5. AI for Control Flow Accessibility
   - AI forgets: focus states, keyboard navigation, screen reader text
   - Accessibility-first prompt template for debugging

6. Optimizing Control Flow Performance with AI
   - AI needs explicit guidance on loop efficiency, early returns
   - Before/after performance comparison

7. Try It Yourself: AI Debugging Challenge
   - Challenge: Debug a broken skill scanner function
   - Requirements: Fix the loop, maintain accessibility, explain the issue

8. HAP's Rules for Working with AI (6 rules)
   1. Always explain the full context
   2. Include what's working, not just what's broken
   3. Request accessibility explicitly
   4. Verify every fix manually
   5. Understand before you ship
   6. Keep a debugging log

9. Advanced Prompt Strategies
   - Refinement prompts
   - Debugging prompts
   - Safe refactoring prompts

10. When NOT to Use AI
    - Learning new concepts (need struggle for understanding)
    - Security-sensitive code (AI may miss vulnerabilities)
    - Understanding your own logic (must trace it yourself)

11. Quick Reference: AI Debugging Tasks
    - Excellent: Syntax errors, explaining code, suggesting alternatives
    - Unreliable: Performance optimization, accessibility verification
    - Not recommended: Security review, architecture decisions

12. Learning Objectives Checklist
    - Understanding AI capabilities
    - Prompt engineering skills
    - Verification workflow
    - Professional responsibility
    - Prof. Teeters' closing reflection
```

---

## 10. Scene framing

```
Previous station ended with: Understanding for loops to iterate through arrays
This station opens with: HAP's excitement about AI quickly turning to disaster
Connection point: "I had just learned loops in Station 5, and I thought AI could help me debug even faster..."
```

---

## Pre-writing checklist

Before starting prose:

- [x] Primary concept is ONE sentence
- [x] Non-goals are explicit
- [x] HAP's arc has clear start/end states
- [x] Prof. Teeters appears ≤2 times (opening + closing for Station 6)
- [x] Grace appears only if precision required
- [x] At least 2 specific confessions listed
- [x] Code role is declared (one only)
- [x] All images have stated reasons
- [x] All 12 sections planned

---

## Cloudinary image versions (verified)

| Image            | Public ID               | Version     |
| ---------------- | ----------------------- | ----------- |
| HAP laptop       | hap-laptop_xiewar       | v1759495998 |
| HAP confused map | hap-confused-map_q8q0ej | v1759495999 |
| HAP celebrating  | hap-celebrating_bljvgl  | v1762699548 |

---

_Full documentation: docs/designing-labs/hap-narrative-and-scene-design.md_
