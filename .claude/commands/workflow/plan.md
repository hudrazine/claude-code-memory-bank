---
description: Analyze options and create implementation strategy
---
# Detailed Analysis & Strategy Planning

## Task
Think deeply about implementation strategy and develop comprehensive options.

$ARGUMENTS

## Process

### 1. Technical Deep Dive
Building on initial understanding:
- Validate critical assumptions through code examination
- Analyze existing patterns and architectural constraints
- Examine edge cases and boundary conditions
- Review related tests for expected behaviors

*For complex analyses, use TodoWrite to track findings and decisions*

### 2. Risk Assessment
Identify and evaluate potential risks:
- **High-impact changes**: Database schemas, API contracts, authentication flows
- **Performance implications**: Algorithm complexity, data volume, caching needs
- **Security considerations**: Input validation, access control, data exposure
- **Compatibility concerns**: Breaking changes, dependency updates, browser support

*Document critical risks in TodoWrite for tracking during implementation*

### 3. Implementation Strategies
Develop multiple viable approaches:

**For each approach:**
- Implementation method and key steps
- Alignment with project patterns and coding principles
- Required changes and their scope
- Estimated complexity and timeline
- Specific risks and mitigation strategies

### 4. Comparative Analysis
Create decision matrix:
- **Correctness**: How well each solves the problem
- **Maintainability**: Long-term code health impact
- **Performance**: Runtime and resource implications
- **Risk Level**: Potential for introducing issues
- **Effort**: Implementation and testing time

### 5. Edge Case Planning
For the recommended approach:
- Null/undefined/empty state handling
- Boundary conditions and limits
- Error scenarios and recovery paths
- Concurrent access considerations (if applicable)
- Data integrity safeguards

## Output

### Implementation Options

Present 2-3 viable options in this format:

**Option 1: [Descriptive Name]**
- **Approach**: Brief description of implementation method
- **Key Changes**:
  - Specific files and components affected
  - New patterns or dependencies introduced
- **Pros**:
  - Technical advantages
  - Alignment with existing patterns
- **Cons**:
  - Potential drawbacks
  - Technical debt or complexity
- **Risk Level**: Low/Medium/High with justification
- **Estimated Time**: Realistic implementation timeframe

**Option 2: [Descriptive Name]**
[Same structure as Option 1]

### Recommendation

**Recommended Approach**: Option [X]

**Justification**:
- Why this option best balances requirements and constraints
- How it aligns with project architecture and patterns
- Risk mitigation strategies for identified concerns

### Next Steps

Upon approval:
1. **Document approved plan** in `memory-bank/plans/` directory
2. Implementation via `/workflow:execute` command
3. Specific validation steps planned
4. Any additional preparation needed

---

**⚠️ IMPORTANT: Wait for explicit user confirmation before proceeding to implementation**

## Plan Documentation (Upon Approval)

Save approved plans to `memory-bank/plans/` with descriptive filenames (e.g., `YYYY-MM-DD-feature-name-plan.md`).

Include:
- Selected option and rationale
- Technical approach and key steps
- Identified risks and mitigation strategies
- Success criteria for validation

This documentation serves as reference for implementation and future sessions.

## Guidelines

- Present genuine alternatives, not strawman options
- Be transparent about trade-offs and uncertainties
- Include "do nothing" option if status quo is viable
- Consider both immediate and long-term impacts
- Reference specific code examples when relevant

## Workflow Integration

**Input**: Findings from `/workflow:understand` phase
**Output**: Implementation options awaiting user approval
**Next Steps**:
- After approval → Document plan → `/workflow:execute`
- Need more analysis → Return to `/workflow:understand`
- Significant blockers → Discuss alternatives with user

**State Preservation**: 
Document selected option and key decisions in TodoWrite for the implementation phase. Create permanent plan document in `memory-bank/plans/` after approval.