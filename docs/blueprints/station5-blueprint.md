# Station 5 blueprint: Repeating actions

**Purpose:** Complete this blueprint BEFORE writing any station content.

---

## 1. Station identity

```
Station ID: station-5-loops
Title (student-facing): Repeating Actions
Lab context: Fifth station - introduces loops to process collections of data
Prerequisites: Station 1-4 (truthy/falsy, operators, conditionals, functions)
```

---

## 2. Learning intent

```
Primary concept: for loops let you repeat code a specific number of times, making it easy to process every item in an array.

Supporting concepts:
- Arrays hold ordered collections of values
- Loop anatomy: initialization, condition, update
- Accessing array elements with index [i]
- The loop counter tracks progress

Explicit non-goals (what this station does NOT teach):
- while loops
- do...while loops
- for...of loops
- for...in loops
- Array methods (forEach, map, filter)
- Nested loops
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
Starting state: Manually checking each skill one at a time with copy-pasted code
Key question: "How do I run the same code for every item in a list without copying it?"
Ending state: Understands how for loops iterate through arrays automatically
```

---

## 4. Prof. Teeters moments

**Frequency:** Once - explaining the loop anatomy

```
- [ ] Opening perspective shift
- [x] Mid-station guidance
- [ ] Validation of learning

Her key line: "HAP, think of a for loop like a robot arm on an assembly line. It starts at position 0, does its job, moves to the next position, and keeps going until it reaches the end. The three parts tell it: where to start, when to stop, and how to move."
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
1. I started my loop at 1 instead of 0 — I skipped the first item in my array!
2. I used <= instead of < with array.length — I got "undefined" for the last iteration because I went one too far.
3. I forgot to increment i — my loop ran forever and crashed the browser!
4. I tried to access skills[5] in a 5-item array — arrays are zero-indexed, so the last item is skills[4].
```

---

## 7. Code example contract

```
Primary role: [x] Illustrative - Shows how for loops process arrays

Constraints:
- Code must use an array of robot skills
- Code must demonstrate the three parts of a for loop
- Code must show accessing array elements with [i]

Student interaction:
- What they should notice: The loop runs once for each item in the array
- What they should NOT change: The loop structure (initialization; condition; update)
```

---

## 8. HAP pose selection

| Location      | Pose intent       | Cognitive state          | Image filename          |
| ------------- | ----------------- | ------------------------ | ----------------------- |
| Intro/Avatar  | Focused, learning | Working through problem  | hap-laptop_xiewar       |
| Confession    | Showing mistakes  | Embarrassed but learning | hap-broke-things_qtbum4 |
| Assembly line | Understanding     | Getting it               | hap-juggles_v2zxeq      |

---

## 9. Station flow skeleton

```
1. What You'll Learn - Overview with 3 insight cards + HAP's Confession
2. The Problem: Repetitive Code - Why loops matter
3. Arrays: Ordered Collections - Storing multiple values
4. Anatomy of a For Loop - The three parts explained
5. Looping Through Arrays - Combining loops and arrays
6. Quick Reference - 4 key takeaways summarized
```

---

## 10. Scene framing

```
Previous station ended with: Understanding functions as reusable code factories
This station opens with: HAP's frustration checking each robot skill manually
Connection point: "I had a function to check skills, but I was calling it separately for each skill..."
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
