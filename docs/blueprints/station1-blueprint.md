# Station 1 blueprint: The truth about values

**Purpose:** Complete this blueprint BEFORE writing any station content.

---

## 1. Station identity

```
Station ID: station-1-truthy-falsy
Title (student-facing): The Truth About Values
Lab context: First station in JS Control Flow - builds on JS Foundations Robot ID Card
Prerequisites: JS Foundations (variables, data types, console.log)
```

---

## 2. Learning intent

```
Primary concept: JavaScript has exactly 7 falsy values - everything else is truthy.

Supporting concepts:
- Values behave differently in boolean contexts (if statements)
- Empty strings, 0, and null are common "gotcha" falsy values
- Truthy doesn't mean true - it means "treated as true in boolean context"

Explicit non-goals (what this station does NOT teach):
- Logical operators (Station 2)
- Comparison operators (beyond basic if)
- Type coercion details beyond boolean context
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
Starting state: Confused why his if statement ran when nickname was ""
Key question: "Why does JavaScript treat some values as false?"
Ending state: Knows the 7 falsy values and can predict boolean behavior
```

---

## 4. Prof. Teeters moments

**Frequency:** Once - mid-station guidance

```
- [ ] Opening perspective shift
- [x] Mid-station guidance
- [ ] Validation of learning

Her key line: "HAP, JavaScript doesn't care if a variable has a value - it cares if that value is meaningful. An empty string exists, but it says nothing."
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
1. I wrote `if (nickname === true)` instead of `if (nickname)` - Prof. Teeters showed me JavaScript checks truthiness automatically
2. I thought `0` meant "no backup battery" but didn't realize JavaScript sees `0` as falsy too - my warning message never showed!
3. I tested `"false"` (the string) and was shocked it's truthy - the word false isn't the same as the value false
4. I mixed up `null` and `undefined` - they're both falsy but mean different things
```

---

## 7. Code example contract

```
Primary role: [x] Illustrative - Shows how truthy/falsy values behave in if statements

Constraints:
- Code must use Robot ID Card variables (nickname, backupBattery, secondaryMission)
- Code must NOT use logical operators (save for Station 2)
- Code must NOT use comparison operators except in explanatory context

Student interaction:
- What they should notice: The same if structure behaves differently based on the value's truthiness
- What they should NOT change: The Robot ID Card variable names
```

---

## 8. HAP pose selection

| Location        | Pose intent       | Cognitive state          | Image filename          |
| --------------- | ----------------- | ------------------------ | ----------------------- |
| Intro/Avatar    | Studying, focused | Curious learner          | hap-laptop_xiewar       |
| Confession      | Showing mistakes  | Embarrassed but learning | hap-broke-things_qtbum4 |
| Quick Reference | Confident         | Understanding            | hap-thumbs-up_s4si0j    |

---

## 9. Station flow skeleton

```
1. What You'll Learn - Overview with 3 insight cards + HAP's Confession
2. The Seven Falsy Values - Core concept with the definitive list
3. Robot ID Card Variables - Applying falsy/truthy to our familiar variables
4. Testing Values in Practice - Code examples with if statements
5. Quick Reference - 4 key takeaways summarized
```

---

## 10. Scene framing

```
Previous station ended with: Hub page introduction to control flow journey
This station opens with: HAP's confusion about why his if statement didn't work as expected
Connection point: "I thought I understood variables from JS Foundations, but then..."
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
