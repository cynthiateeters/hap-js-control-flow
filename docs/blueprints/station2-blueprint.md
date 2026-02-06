# Station 2 blueprint: Combining conditions

**Purpose:** Complete this blueprint BEFORE writing any station content.

---

## 1. Station identity

```
Station ID: station-2-logical-operators
Title (student-facing): Combining Conditions
Lab context: Second station - builds on truthy/falsy from Station 1
Prerequisites: Station 1 (truthy/falsy values), JS Foundations (variables)
```

---

## 2. Learning intent

```
Primary concept: Logical operators (&&, ||, !) combine conditions and short-circuit for efficiency.

Supporting concepts:
- AND (&&) requires both conditions to be true
- OR (||) requires at least one condition to be true
- NOT (!) inverts a boolean value
- Short-circuit evaluation stops early when result is determined

Explicit non-goals (what this station does NOT teach):
- if/else chains (Station 3)
- Ternary operator
- Bitwise operators
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
Starting state: Trying to check multiple conditions with nested if statements
Key question: "Is there a better way to combine conditions?"
Ending state: Understands &&, ||, ! and can use short-circuit patterns
```

---

## 4. Prof. Teeters moments

**Frequency:** Once - explaining short-circuit evaluation

```
- [ ] Opening perspective shift
- [x] Mid-station guidance
- [ ] Validation of learning

Her key line: "HAP, JavaScript is lazy in a good way. With AND, it stops at the first false because it already knows the answer can't be true. With OR, it stops at the first true."
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
1. I wrote nested if statements instead of using && - my code was 10 lines when it could have been 2!
2. I forgot that || returns the first truthy value, not just true/false - nickname || robotName blew my mind
3. I put the expensive function call BEFORE the simple check in my && chain - Prof. Teeters showed me why order matters
4. I used ! on the wrong thing and inverted my entire condition - spent an hour debugging backwards logic
```

---

## 7. Code example contract

```
Primary role: [x] Illustrative - Shows how logical operators combine conditions

Constraints:
- Code must use Robot ID Card variables (isOnline, isCharging, energyLevel)
- Code must demonstrate short-circuit evaluation
- Code must NOT use if/else chains (save for Station 3)

Student interaction:
- What they should notice: How && and || work together, short-circuit behavior
- What they should NOT change: The Robot ID Card variable names
```

---

## 8. HAP pose selection

| Location      | Pose intent        | Cognitive state          | Image filename            |
| ------------- | ------------------ | ------------------------ | ------------------------- |
| Intro/Avatar  | Focused, combining | Working through problem  | hap-laptop_xiewar         |
| Confession    | Showing mistakes   | Embarrassed but learning | hap-broke-things_qtbum4   |
| Short-circuit | Breakthrough       | Mind blown               | hap-brain-explodes_wu0or8 |

---

## 9. Station flow skeleton

```
1. What You'll Learn - Overview with 3 insight cards + HAP's Confession
2. The Three Logical Operators - AND, OR, NOT explained
3. Short-Circuit Evaluation - The efficiency trick
4. Real-World Patterns - Default values, guard clauses
5. Quick Reference - 4 key takeaways summarized
```

---

## 10. Scene framing

```
Previous station ended with: Understanding truthy/falsy values
This station opens with: HAP's frustration with nested if statements
Connection point: "Now that I knew which values were truthy, I wanted to check multiple things at once..."
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
