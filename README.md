# fossee-python-debugging-assistant
AI Debugging Assistant Prompt for FOSSEE Python Internship Task 2

# Python Debugging Assistant Prompt - FOSSEE Internship Task 2

**Candidate:** Diya Raghuvanshi  
**Task:** Python Screening Task 2 - Write a Prompt for an AI Debugging Assistant  
**Date:** 14 September 2025

## Repository Structure

- `debugging_prompt.md` - The main AI debugging assistant prompt
- `test_example.md` - Sample test case and output 
- `README.md` - This file with setup instructions and reasoning

## Setup Instructions

1. **Using the Prompt:**
   - Copy the content from `debugging_prompt.md`
   - Paste it into any AI assistant (ChatGPT, Claude, Gemini, etc.)
   - Fill in the `[CURRENT_CONTEXT]` section with:
     - Student's buggy code
     - Error description
     - Test cases
     - Conversation history (if any)
   - The AI will respond with Socratic questions to guide debugging

2. **Example Usage:**
   See `test_example.md` for a complete example of the prompt in action.

## Design Reasoning

### Why This Approach?

I designed this prompt using the **Socratic Method** as the core pedagogical approach because:

- **Active Learning:** Students learn better when they discover solutions themselves rather than being given direct answers
- **Deep Understanding:** Questions force students to think through underlying concepts, not just fix syntax
- **Transferable Skills:** Students learn debugging strategies they can apply to future problems
- **Confidence Building:** Self-discovery builds more confidence than receiving solutions

### Tone and Style Choice

**Professional but Supportive Mentor Tone:**
- Uses "instructor" rather than "assistant" to establish educational authority
- Includes specific guidance for acknowledging student frustration
- Balances challenge with support to maintain productive struggle
- Emphasizes encouragement and reframing difficulties as learning opportunities

**Question-Based Communication:**
- Every response must be primarily questions to avoid solution-giving
- Questions are categorized by cognitive level (comprehension, analysis, application)
- Progressive questioning from general to specific allows adaptation to student needs

### How It Avoids Giving Solutions

**Multiple Prevention Mechanisms:**

1. **Explicit Prohibitions:** Clear "NEVER" statements about providing code solutions, line numbers, or direct fixes
2. **Question-Only Constraint:** Forces AI to communicate through questions only
3. **Internal Processing:** The `[THOUGHT]` section keeps bug analysis hidden from students
4. **Self-Correction:** Built-in quality check ensures questions don't reveal answers

**Key Innovation:** The structured `[THOUGHT]` section allows the AI to fully understand the problem while maintaining educational constraints.

### Encouraging Student-Friendly Feedback

**Systematic Encouragement:**
- Acknowledgment of effort and partial progress
- Reframing challenges as learning opportunities
- Focus on building confidence through guided discovery
- Limitation to 2-3 questions to prevent cognitive overload

**Educational Focus:**
- Emphasis on understanding concepts, not just fixing bugs
- Teaching debugging strategies for independent problem-solving
- Metacognitive questions that help students understand their own thinking

### Balancing Bug Identification and Student Guidance

**The `[THOUGHT]` Process:**
- AI analyzes bugs systematically but privately
- Understanding informs question strategy without revealing analysis
- Prevents random or unfocused questioning

**Layered Approach:**
- Start with broad questions about expected behavior
- Progressively narrow focus based on student responses
- Never point directly to bugs but guide attention to relevant areas
- Focus on teaching debugging process, not just finding specific errors

### Beginner vs. Advanced Adaptation

**Adaptive Questioning Strategy:**

**For Beginners:**
- Focus on fundamental Python concepts and terminology
- Provide more context about basic programming constructs
- Ask about simple cases and basic understanding
- Example: "What do you think happens when we use `range(5)`?"

**For Advanced Students:**
- Ask about edge cases, efficiency, and best practices
- Discuss code design and architectural considerations
- Explore deeper programming principles
- Example: "How might this approach perform with very large inputs?"

**Assessment Integration:**
- Gauge student level from code complexity and problem-solving approach
- Adapt language complexity and concept depth accordingly
- Start broadly and adjust based on student responses

### Research Foundation

### Research Foundation

This prompt incorporates evidence-based educational strategies:

- **Socratic Method:** Questions lead students to self-discovery rather than providing direct instruction, promoting deeper understanding and critical thinking
- **Constructivist Learning Theory:** Students build understanding through guided discovery rather than passive information consumption
- **Scaffolding:** Progressive questioning provides temporary support that's gradually removed as student understanding develops
- **Zone of Proximal Development (Vygotsky):** Questions calibrated to challenge students just beyond their current ability level with appropriate guidance
- **Cognitive Load Management:** Limits questions per response (2-3 maximum) to prevent cognitive overwhelm and maintain focus
- **Metacognitive Awareness:** Explicit focus on students' thinking processes, helping them understand how they learn and debug
- **Productive Struggle:** Maintains appropriate challenge level that promotes learning without causing frustration or helplessness
- **Inquiry-Based Learning:** Student-driven exploration through strategic questioning rather than teacher-centered instruction
- **Formative Assessment:** Continuous evaluation of student understanding through their responses to guide next questions
- **Growth Mindset Cultivation:** Reframes errors and debugging challenges as valuable learning opportunities rather than failures
- **Active Learning Principles:** Engages students in the debugging process rather than passive problem-solving observation
- **Differentiated Instruction:** Adapts questioning complexity and focus based on apparent student skill level and needs

The design was informed by research papers on AI in education, prompting best practices guides, and Socratic teaching methodology.

## Expected Effectiveness

This prompt should effectively:
- Teach debugging as a transferable skill, not just fix individual bugs
- Build student confidence through self-discovery
- Adapt to different skill levels and learning needs
- Prevent over-reliance on AI assistance
- Create engaging educational interactions that feel like working with a skilled mentor

---

**Contact:** diya.raghuvanshi2005@gmail.com  
**GitHub:** (https://github.com/DiyaR1211)
