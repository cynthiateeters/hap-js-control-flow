# Station 3 blueprint: Making decisions

**Purpose:** Complete this blueprint BEFORE writing any station content.

---

## 1. Station identity

```
Station ID: station-3-conditionals
Title (student-facing): Making Decisions
Lab context: Third station - applies truthy/falsy and operators to branching logic
Prerequisites: Station 1 (truthy/falsy), Station 2 (logical operators)
```

---

## 2. Learning intent

```
Primary concept: if/else if/else chains let you handle multiple exclusive conditions with clear, readable code.

Supporting concepts:
- Single-branch decisions with if
- Two-branch decisions with if/else
- Multi-branch decisions with if/else if/else
- Choosing the right structure for the problem

Explicit non-goals (what this station does NOT teach):
- switch statements
- Ternary operator
- Nested conditionals (keep it flat)
```

---

## 3. Narrative design

### Characters present

```
- [x] HAP (always - narrator)
- [x] Prof. Teeters (for guidance moments)
- [ ] Grace Hopper (not needed this station)
- [ ] Other entity
```

### HAP's arc

```
Starting state: Using multiple separate if statements that all run independently
Key question: "How do I make JavaScript pick ONE path from many options?"
Ending state: Understands else if chains and when to use each conditional structure
```

---

## 4. Prof. Teeters moments

**Frequency:** Once - explaining the importance of order in else if chains

```
- [ ] Opening perspective shift
- [x] Mid-station guidance
- [ ] Validation of learning

Her key line: "HAP, think of else if like a series of doors. JavaScript opens each door in order, but the moment it finds one that's unlocked, it walks through and ignores all the rest."
```

---

## 5. Grace Hopper moments (if applicable)

**Frequency:** Not in this station

```
- [ ] Not applicable
```

---

## 6. HAP's confessions

List 2-4 specific mistakes HAP made learning this topic:

```
1. I wrote separate if statements instead of else if - my robot got classified as BOTH "Warm" AND "Optimal" at the same time!
2. I put my conditions in the wrong order - checked > 60 before > 90 and everything was "Optimal"
3. I forgot the final else - when coreTemperature was exactly 60, nothing happened and temperatureStatus was undefined
4. I used = instead of === in my condition - assigned instead of compared and broke everything
```

---

## 7. Code example contract

```
Primary role: [x] Illustrative - Shows how if/else if/else chains work

Constraints:
- Code must use Robot ID Card variable (coreTemperature)
- Code must demonstrate proper ordering of conditions
- Code must show the difference between separate ifs and else if chains

Student interaction:
- What they should notice: Only ONE branch executes in an else if chain
- What they should NOT change: The temperature thresholds (90, 75, 60)
```

---

## 8. HAP pose selection

| Location      | Pose intent       | Cognitive state          | Image filename          |
| ------------- | ----------------- | ------------------------ | ----------------------- |
| Intro/Avatar  | Focused, deciding | Working through problem  | hap-laptop_xiewar       |
| Confession    | Showing mistakes  | Embarrassed but learning | hap-broke-things_qtbum4 |
| Order matters | Understanding     | Getting it               | hap-thumbs-up_s4si0j    |

---

## 9. Station flow skeleton

```
1. What You'll Learn - Overview with 3 insight cards + HAP's Confession
2. The Three Conditional Structures - if, if/else, if/else if/else
3. Why Order Matters - The doors analogy and proper ordering
4. Temperature Classification - Complete example with coreTemperature
5. Quick Reference - 4 key takeaways summarized
```

---

## 10. Scene framing

```
Previous station ended with: Understanding logical operators and short-circuit evaluation
This station opens with: HAP's frustration when his robot gets multiple classifications
Connection point: "Now that I could combine conditions, I needed to make my code choose between them..."
```

---

## Pre-writing checklist

Before starting prose:

- [x] Primary concept is ONE sentence
- [x] Non-goals are explicit
- [x] HAP's arc has clear start/end states
- [x] Prof. Teeters appears <= 1 time
- [x] Grace appears only if precision required (not needed)
- [x] At least 2 specific confessions listed
- [x] Code role is declared (one only)
- [x] All images have stated reasons
- [x] Flow skeleton complete

---

_Full documentation: docs/designing-labs/hap-narrative-and-scene-design.md_
