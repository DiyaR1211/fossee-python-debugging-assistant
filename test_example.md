# Test Examples

This document demonstrates the debugging prompt in action across different skill levels and bug types, with actual AI outputs.

## Test Case 1: Beginner - Missing Return Statement

### Input Code
```python
def add_numbers(a, b):
    result = a + b
    print(result)

answer = add_numbers(3, 5)
print("The answer is:", answer)
```

### Problem Context
- **Expected Output:** "The answer is: 8"
- **Actual Output:** "8\nThe answer is: None"
- **Bug Type:** Logic Error - Misinterpretation (print vs return confusion)
- **Student Level:** Beginner

### Student Input
"My function prints the right number but when I try to use the result, it says None. I don't understand why."

### AI Response Using This Prompt
"That's a great piece of code to look at! I see that the final output is `The answer is: None`, which is different from the `8` that gets printed earlier.

Could you walk me through these questions?

1. Your code produces two separate lines of output. Can you point to which line of code is responsible for printing the `8`, and which line is responsible for printing `The answer is: None`?
2. When the line `answer = add_numbers(3, 5)` runs, what specific value do you expect the `add_numbers` function to "give back" to be stored in the `answer` variable?"

### Analysis
✅ **Follows Prompt Rules:**
- No direct solution given
- Uses only Socratic questions (2 questions, within limit)
- Appropriate for beginner level
- Focuses on core concept discovery
- Encouraging tone with acknowledgment

---

## Test Case 2: Intermediate - Factorial Function Bug

### Input Code
```python
def factorial(n):
    result = 0
    for i in range(1, n + 1):
        result *= i
    return result

print(factorial(5))  # Expected: 120, Actual: 0
```

### Problem Context
- **Expected Output:** 120
- **Actual Output:** 0
- **Bug Type:** Logic Error - Wrong initialization
- **Student Level:** Intermediate

### Student Input
"My factorial function isn't working, it always returns 0 for n >= 1. Can you help?"

### Actual AI Response Using This Prompt
"Thanks for sharing your code! It's a great attempt, and figuring out this kind of logic bug is a fantastic way to deepen your understanding of how loops work.

You've correctly noticed that the function always returns `0` for any number greater than or equal to 1. Let's trace the code's execution with a simple example to see if we can spot why.

Let's imagine we call `factorial(3)`:

1. What is the initial value of the `result` variable before the `for` loop begins?
2. During the very first run of the loop, what is the value of `i`, and what will the new value of `result` be after the line `result *= i` is executed?"

### Analysis
✅ **Follows Prompt Rules:**
- Guides discovery through tracing questions
- 2 focused questions that build understanding
- No direct mention of initialization error or solution
- Encourages step-by-step analysis
- Appropriate complexity for intermediate student

---

## Test Case 3: Advanced - Mutable Default Argument

### Input Code
```python
def append_to_list(item, lst=[]):
    lst.append(item)
    return lst

def build_shopping_lists():
    fruits = append_to_list("apple")
    vegetables = append_to_list("carrot")
    dairy = append_to_list("milk")
    
    return fruits, vegetables, dairy

result = build_shopping_lists()
print("Fruits:", result[0])
print("Vegetables:", result[1])
print("Dairy:", result[2])
```

### Problem Context
- **Expected Output:** Separate lists for each category
- **Actual Output:** All lists contain ["apple", "carrot", "milk"]
- **Bug Type:** Logic Error - Fundamental Misconception (mutable default arguments)
- **Student Level:** Advanced

### Student Input
"This is really strange. I expected each function call to start with a fresh empty list, but somehow all my lists are getting mixed together. I've been debugging this for an hour and can't figure out why the lists are sharing state. Is this some kind of Python bug or memory issue?"

### Actual AI Response Using This Prompt
"That is a fantastic piece of code to investigate! This demonstrates one of the most famous "gotchas" in Python, and understanding it is a huge step in mastering how the language works under the hood.

You've noticed the surprising output: all three lists—`fruits`, `vegetables`, and `dairy`—end up containing every single item. This is a very interesting clue.

Let's start with a broad question to form a hypothesis:

1. Given that all three variables (`fruits`, `vegetables`, and `dairy`) seem to hold the exact same list at the end, what might that suggest about the list object that the `append_to_list` function is using on each call?
2. Let's focus on the line `def append_to_list(item, lst=[]):`. In your mental model, how many times does Python create the empty list `[]` that is used as the default value? Does it happen once, or every time the function is called?"

### Analysis
✅ **Follows Prompt Rules:**
- Acknowledges advanced student's debugging effort
- Questions target deeper Python concepts (object mutability, evaluation timing)
- Encourages hypothesis formation and testing
- No direct solution about using `None` as default
- Appropriate depth for advanced programmer

---

## Summary

These test cases demonstrate the prompt's effectiveness across different scenarios:

### **Skill Level Adaptation:**
- **Beginner:** Simple conceptual questions about fundamental programming concepts
- **Intermediate:** Step-by-step tracing questions for algorithmic debugging  
- **Advanced:** Deep conceptual questions about language-specific behavior

### **Consistent Quality:**
All responses maintain the Socratic approach while adapting complexity and terminology to the apparent student skill level. The AI consistently:

- Uses encouraging, supportive language
- Asks 2-3 focused questions maximum
- Guides discovery without revealing solutions
- Addresses root concepts rather than surface symptoms
- Builds debugging skills alongside problem-solving

### **Real-World Validation:**
These examples include actual AI outputs generated using the prompt, demonstrating its practical effectiveness across different AI systems and debugging scenarios.
