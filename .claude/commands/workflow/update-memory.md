---
description: Update Memory Bank with significant learnings
---
# Memory Bank Documentation Update

## Task
Think longer about project evolution and comprehensively review all Memory Bank files to preserve important learnings, decisions, and project state for future Claude Code sessions. Ensure they accurately reflect the current project state and recent developments.

## Process

### 1. Comprehensive Review

Review all Memory Bank files in order:
1. **projectbrief.md** - Core project information
2. **productContext.md** - Product decisions and user experience
3. **systemPatterns.md** - Architecture and design patterns
4. **techContext.md** - Technologies and tools
5. **activeContext.md** - Current focus and next steps
6. **progress.md** - Development milestones and status

### 2. Update Criteria

Document changes when:
- **New patterns established**: Coding patterns, architectural decisions, workflows
- **Significant features completed**: Major functionality, integrations, systems
- **Important discoveries made**: Technical insights, constraint clarifications, solutions
- **Project direction changes**: Scope adjustments, priority shifts, approach changes
- **Challenges resolved**: How problems were solved for future reference

### 3. Update Guidelines

**For projectbrief.md:**
- Core requirements changes
- Scope adjustments
- Major goal revisions
- Fundamental constraint updates

**For productContext.md:**
- User experience insights
- Problem definition refinements
- Solution approach changes
- Value proposition updates

**For activeContext.md:**
- Current development phase and focus
- Recently completed work
- Active challenges and blockers
- Next priority actions
- Important decisions in progress

**For progress.md:**
- Feature completion status
- Development milestone achievements
- Recent updates with dates
- Current challenges and risks

**For systemPatterns.md:**
- New design patterns adopted
- Architectural decisions made
- Integration approaches established
- Security or performance patterns

**For techContext.md:**
- New technologies added
- Configuration changes
- Development workflow updates
- Environment setup changes

### 4. Quality Checks

Before finalizing:
- Ensure updates are factual and accurate
- Verify consistency across files
- Check that next steps are clear
- Confirm critical information isn't lost
- Use clear, concise language
- Date significant updates
- Focus on "what" and "why", not just "how"

### 5. Optional: Changelog Management

*For larger projects with extensive history:*

**Check for archiving needs:**
- If today is the 1st of the month, archive previous month's entries
- If `progress.md` exceeds 300 lines, consider archiving older entries
- Archive process:
  1. Extract entries from previous month(s) from `progress.md`
  2. Create/update `changelog/YYYY-MM-monthname.md` file
  3. Update `changelog/index.md` with archive summary
  4. Remove archived entries from `progress.md`

**Changelog file naming:**
- Format: `YYYY-MM-monthname.md` (e.g., `2025-05-may.md`)
- Lowercase month names for consistency

## Output

**Files Updated:**
- [filename]: Brief summary of changes

**Key Additions:**
- Important patterns documented
- Major decisions recorded
- Significant learnings captured

**Memory Bank Status:**
- Current completeness assessment
- Any gaps identified
- Recommendations for future sessions

*If changelog was archived:*
- Archived entries: [Month Year]
- Files created/updated: [changelog filenames]
- Lines moved from progress.md: [count]

## Key Principles

- **Be selective**: Document significant changes, not every detail
- **Think future-first**: What would help the next session?
- **Maintain clarity**: Avoid internal jargon or unclear references
- **Preserve context**: Don't remove historical information
- **Focus on value**: Document what matters for project success

## Workflow Integration

**Input**: Recent work, discoveries, and learnings
**Output**: Updated Memory Bank files
**Next**: Continue with `/workflow:understand` or end session

Remember: The Memory Bank is the only persistent link between Claude Code sessions.