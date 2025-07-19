---
description: Understand context and perform initial task analysis
---
# Context Review & Initial Assessment

## Memory Bank Context
- @memory-bank/projectbrief.md
- @memory-bank/productContext.md
- @memory-bank/systemPatterns.md
- @memory-bank/techContext.md
- @memory-bank/activeContext.md
- @memory-bank/progress.md

## Task
Think through the task requirements and current project context to establish comprehensive understanding.

$ARGUMENTS

## Process

### 1. Task Decomposition
- Break down the task into core requirements
- Identify explicit and implicit constraints
- Clarify the scope and expected outcomes
- Note any assumptions that need validation

### 2. Context Discovery
Leverage parallel tool execution for efficient information gathering:
- Use Task agent for broad pattern searches when exploring unknown areas
- Apply Grep/Glob for specific file and content location
- Read relevant files, configurations, and documentation
- Check recent git history if understanding evolution helps

### 3. Initial Analysis
Based on gathered information:
- Map current system state and relevant components
- Identify dependencies and integration points
- Recognize existing patterns that should be followed
- Spot potential challenges or contradictions

### 4. Knowledge Synthesis
- Connect findings to existing project documentation
- Relate to established project patterns and conventions
- Consider technical constraints and architecture decisions
- Review current project context and focus areas

### 5. Feedback Loop Analysis (When returning from other phases)
When revisiting due to implementation feedback:
- **From `/workflow:execute`**: Focus on specific blockers or discoveries
  - Review the documented issues from implementation
  - Investigate root causes of integration problems
  - Clarify ambiguous requirements based on real constraints
- **From `/workflow:plan`**: Re-examine assumptions that proved incorrect
  - Validate new constraints discovered during planning
  - Research alternative approaches for blocked strategies
- **Efficiency tip**: Target investigation to specific feedback rather than full re-analysis

## Output

Present findings in a structured format (consider TodoWrite for complex tasks):

**Task Understanding:**
- Core requirements identified
- Constraints and assumptions
- Scope boundaries

**Current State:**
- Relevant files and components
- Existing patterns discovered
- Dependencies mapped

**Initial Assessment:**
- Complexity evaluation
- Potential challenges
- Areas needing deeper investigation

**Next Steps:**
- Recommended approach (e.g., proceed to /plan for complex tasks)
- Specific areas for detailed analysis
- Any immediate clarifications needed

## Guidelines

- Focus on understanding, not solutioning
- Use TodoWrite for complex tasks requiring multi-step exploration or when investigating multiple unknown areas
- Acknowledge when more investigation is needed
- Keep Memory Bank context in mind
- Scale effort with task complexity

## Workflow Integration

**Input Sources**:
- Fresh task: Task description from user
- Feedback loop: Specific issues from `/workflow:execute` or `/workflow:plan`
- Re-assessment: New constraints or discoveries from implementation

**Output**: Structured findings (updated with new insights if from feedback loop)

**Next Steps**:
- Complex tasks → `/workflow:plan`
- Simple/clear tasks → `/workflow:execute`
- Need clarification → Ask user
- Resolved blockers → Return to originating phase with solutions

**State Preservation**: 
- For complex tasks: Document key findings in TodoWrite
- For feedback loops: Update findings with new discoveries
- Include both original understanding and evolved insights