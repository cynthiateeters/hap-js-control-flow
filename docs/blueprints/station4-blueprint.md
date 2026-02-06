# Station 4 blueprint: Reusable code with functions

**Purpose:** Complete this blueprint BEFORE writing any station content.

---

## 1. Station identity

```
Station ID: station-4-functions
Title (student-facing): Reusable Code with Functions
Lab context: Fourth station - introduces functions to organize and reuse code
Prerequisites: Station 1-3 (truthy/falsy, logical operators, conditionals)
```

---

## 2. Learning intent

```
Primary concept: Functions let you name a block of code and run it whenever you need it, with different inputs producing different outputs.

Supporting concepts:
- Defining functions with parameters (inputs)
- Returning values (outputs)
- Calling functions with arguments
- Function scope (variables inside stay inside)

Explicit non-goals (what this station does NOT teach):
- Arrow functions (=> syntax)
- Callback functions
- Methods on objects
- Higher-order functions
- Closures
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
Starting state: Writing the same code over and over for different Robot ID Card values
Key question: "How do I stop copying and pasting the same code everywhere?"
Ending state: Understands how to create functions that accept inputs and return outputs
```

---

## 4. Prof. Teeters moments

**Frequency:** Once - explaining the function factory analogy

```
- [ ] Opening perspective shift
- [x] Mid-station guidance
- [ ] Validation of learning

Her key line: "HAP, think of a function like a factory machine. You put raw materials in (parameters), the machine does its work, and a finished product comes out (return value). The same machine can make different products depending on what you put in!"
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
1. I forgot to use the return keyword - my function ran but gave me undefined instead of the result!
2. I tried to use a variable I created inside a function from outside - JavaScript said it wasn't defined because of scope.
3. I called my function without parentheses - I got the function code itself instead of running it!
4. I mixed up parameters and arguments - Prof. Teeters helped me remember: Parameters are Placeholders, Arguments are Actual values.
```

---

## 7. Code example contract

```
Primary role: [x] Illustrative - Shows how functions work with inputs and outputs

Constraints:
- Code must use Robot ID Card variables
- Code must demonstrate parameters, return values, and function calls
- Code must show the difference between defining and calling functions

Student interaction:
- What they should notice: Same function produces different results with different inputs
- What they should NOT change: The function structure (parameters, return)
```

---

## 8. HAP pose selection

| Location        | Pose intent       | Cognitive state          | Image filename          |
| --------------- | ----------------- | ------------------------ | ----------------------- |
| Intro/Avatar    | Focused, creating | Working through problem  | hap-laptop_xiewar       |
| Confession      | Showing mistakes  | Embarrassed but learning | hap-broke-things_qtbum4 |
| Factory analogy | Understanding     | Getting it               | hap-chef.jpg            |

---

## 9. Station flow skeleton

```
1. What You'll Learn - Overview with 3 insight cards + HAP's Confession
2. The Problem: Repeated Code - Why functions matter
3. Anatomy of a Function - define, call, parameters, return
4. The Factory Analogy - Prof. Teeters' explanation with examples
5. Scope: What Happens Inside Stays Inside - Variable visibility
6. Quick Reference - 4 key takeaways summarized
```

---

## 10. Scene framing

```
Previous station ended with: Understanding if/else if/else chains for decision making
This station opens with: HAP's frustration with copying the same status-checking code for different values
Connection point: "Now that I could make decisions, I found myself writing the same decision logic over and over..."
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
