# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

**Important: This is NOT a software development project.** This is a prompt engineering and file management project for the Claude Code Memory Bank system.

This repository serves two primary purposes:
1. **Prompt Engineering**: Development and refinement of the Memory Bank system methodology for Claude Code
2. **File Management**: Storage and version control of the core files that constitute the Claude Code Memory Bank

Claude Code Memory Bank is an experimental adaptation of Cline Memory Bank, designed specifically for Claude Code. It provides:
- A hierarchical documentation structure (Memory Bank) for use in other projects
- Custom slash commands for workflow management
- Best practices for context preservation across sessions

Note: This project itself does not use the Memory Bank system (as that would be excessive for a methodology project). Instead, it contains the reference implementation and documentation that other projects can adopt.

## Project Contexts

1. Claude Code memory management：
   - Local documentation: @references/claude-code-manage-memory.md
   - Web documentation: [Manage Claude's memory - Anthropic](https://docs.anthropic.com/en/docs/claude-code/memory)

2. Claude Code custom slash commands:
   - Local documentation: @references/claude-code-slash-commands.md
   - Web documentation: [Slash Commands - Anthropic](https://docs.anthropic.com/en/docs/claude-code/slash-commands#custom-slash-commands)

3. Cline Memory Bank (Original):
   - Local documentation: @references/cline-memory-bank.md
   - Web documentation: [Cline Memory Bank](https://docs.cline.bot/prompting/cline-memory-bank)

4. Claude Code Memory Bank (Customized for this project):
   - Local documentation: @.claude/claude-memory-bank.md

## Project Structure

### Directory Structure
```
claude-code-memory-bank/
├── CLAUDE.md                    # This file - Project guidance for Claude Code
├── README.md                    # Project overview and usage instructions
├── LICENSE                      # Unlicense (public domain)
├── references/                  # Reference documentation
│   ├── claude-code-manage-memory.md    # Claude Code memory management features
│   ├── claude-code-slash-commands.md   # Claude Code custom slash commands
│   └── cline-memory-bank.md           # Original Cline Memory Bank documentation
└── .claude/                     # Claude Code Memory Bank implementation
    ├── claude-memory-bank.md    # Core Memory Bank system documentation (conceptual layer)
    └── commands/                # Custom slash commands
        ├── init-memory-bank.md # Quick Memory Bank initialization
        ├── commit.md           # Git commit workflow command
        └── workflow/           # Memory Bank workflow commands
            ├── understand.md   # Context analysis command
            ├── plan.md        # Planning command
            ├── execute.md     # Execution command
            └── update-memory.md # Memory update command
```

### File Descriptions

#### Core System Files
- **`.claude/claude-memory-bank.md`**: The conceptual layer that defines how the Memory Bank system works. This is the primary prompt engineering artifact.
- **`.claude/commands/`**: Custom slash commands that implement the Memory Bank workflow for use in other projects.

#### Reference Documentation
- **`references/`**: Contains documentation about Claude Code features and the original Cline Memory Bank, serving as reference material for the adaptation.

Note: The Memory Bank files (projectbrief.md, productContext.md, etc.) are NOT part of this repository. They are created in individual projects that adopt the Memory Bank system.

## Custom Slash Commands

This project includes custom slash commands for Claude Code workflow management, stored in `.claude/commands/`:

### Memory Management Workflow Commands
- `/workflow:understand` - Analyzes project context and task requirements
- `/workflow:plan` - Creates detailed analysis and implementation strategies
- `/workflow:execute` - Implements tasks with systematic quality checks
- `/workflow:update-memory` - Updates Memory Bank documentation after task completion
- `/init-memory-bank` - Initialize Memory Bank structure for new projects
- `/commit` - Custom git commit workflow command

These commands are reference implementations that can be copied to other projects adopting the Memory Bank system.

## Technical Architecture

### How the Memory Bank System Works
The Memory Bank system (designed for use in other projects) operates through a combination of Claude Code's features:

1. **Context Loading**: Memory Bank files are loaded into Claude Code's context using `@imports` in CLAUDE.md
2. **Workflow Phases**: The system defines four distinct phases (understand, plan, execute, update-memory) that build on each other
3. **State Preservation**: Each phase produces artifacts that inform the next phase, creating a continuous workflow
4. **Documentation Hierarchy**: Files are structured from general (projectbrief) to specific (activeContext), allowing for efficient context loading

### Integration with Claude Code
- **CLAUDE.md**: Serves as the entry point, can import Memory Bank files
- **Custom Slash Commands**: Extend Claude Code's functionality with project-specific workflows
- **@imports**: Claude Code's native feature for loading additional context files
- **Persistent Documentation**: Unlike conversation history, Memory Bank files persist across sessions

### This Repository as Reference Implementation
This repository contains:
- The core Memory Bank system documentation (`.claude/claude-memory-bank.md`)
- Reference implementations of workflow commands
- Documentation and guides for adopting the system
- No actual Memory Bank files (those belong in individual projects)

### Differences from Cline Memory Bank
- Adapted for Claude Code's specific features (CLAUDE.md, slash commands)
- Simplified workflow commands tailored to Claude Code's capabilities
- Leverages Claude Code's @import system instead of manual context loading

## Development Notes

- This is an experimental adaptation of Cline Memory Bank for Claude Code
- The system leverages Claude Code's CLAUDE.md and custom slash commands
- No traditional build/test scripts - this is a documentation-focused project
- For implementation details, refer to `.claude/claude-memory-bank.md`

--- End of Contents ---