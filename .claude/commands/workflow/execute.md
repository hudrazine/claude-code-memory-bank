---
description: Execute planned implementation with quality checks
---
# Implementation & Quality Assurance

## Task
Think carefully about implementation details and execute the planned solution with focus on quality.

$ARGUMENTS

## Implementation Process

### Setup & Preparation
- Review the approved plan or task requirements
- Verify working on correct branch with no conflicting changes
- For complex implementations, consider using TodoWrite to track progress

### Code Implementation
**Follow project patterns:**
- Adhere to existing coding conventions and architectural patterns
- Implement incrementally with validation between significant changes
- Use MultiEdit for cohesive multi-file modifications
- Maintain clean, readable code with appropriate error handling

**Quality during development:**
- Test functionality after each component is implemented
- Check for compile/syntax/type errors regularly
- Ensure edge cases are properly handled

## Quality Assurance

### Automated Checks
Run all relevant project quality tools:
- Code formatting and linting
- Type checking and static analysis  
- Unit and integration tests
- Build verification

### Manual Validation
- Test implemented features thoroughly
- Verify error messages are user-friendly
- Ensure no debug code or temporary TODOs remain
- Confirm implementation matches requirements

## Completion Review

### Final Checklist
- All changes follow project patterns ✓
- Quality checks pass ✓
- Implementation matches plan ✓
- No regressions introduced ✓

### Summary Report
**Changes:** List files modified and key implementations
**Quality Status:** Report results of all checks
**Next Steps:** Any follow-up work or discovered improvements

## Guidelines

- Prioritize correctness and quality over speed
- Ask for clarification if requirements are ambiguous
- Report any issues discovered during implementation
- Keep changes focused on the approved scope
- If blocked, document the issue clearly and suggest solutions

## Feedback Loop Handling

During implementation, if you encounter:

### Requirements Uncertainty
- **Symptom**: Unclear specifications, ambiguous edge cases, missing context
- **Action**: Pause implementation → Document findings → `/workflow:understand` for clarification
- **Example**: "The API specification doesn't define error response format"

### Better Approach Discovered
- **Symptom**: Found more efficient solution, identified architectural improvement
- **Action**: Document discovery → `/workflow:plan` to evaluate alternatives
- **Example**: "Discovered existing utility that could replace custom implementation"

### Integration Issues
- **Symptom**: Unexpected dependencies, conflicting patterns, breaking changes
- **Action**: Assess impact → Return to appropriate phase:
  - Minor adjustments: Continue with documented workaround
  - Major conflicts: `/workflow:understand` for context re-evaluation
  - Architecture changes: `/workflow:plan` for strategy revision

### Quality Check Failures
- **Symptom**: Tests failing, linting errors, type mismatches
- **Action**: 
  - First attempt: Fix issues maintaining current approach
  - Persistent issues: Evaluate if approach needs revision → `/workflow:plan`
  - Systemic problems: `/workflow:understand` to reassess constraints

## Workflow Integration

**Input**: Approved plan from `/workflow:plan` or direct task description
**Output**: Completed implementation with quality validation

**Next Steps Based on Outcome:**
- ✅ Success → `/workflow:update-memory` for significant changes
- 🔄 Needs Clarification → `/workflow:understand` with specific questions
- 🔀 Better Approach Found → `/workflow:plan` with new insights
- ⚠️ Blocked → Document blockers and return to appropriate phase

**State Preservation**: 
When transitioning to another phase, document:
- Current implementation progress
- Specific issues encountered
- Discoveries or insights gained
- Recommended next actions