---
description: Initialize Memory Bank structure for a new project
---

# Initialize Memory Bank System

## Your Task

Initialize the Memory Bank system adaptively based on the current project state.

### 1. **Comprehensive Project Analysis**

Use the Task tool to analyze the project with the following prompt:

"Analyze the current project directory and provide a detailed report including:
1. Current working directory path
2. Memory Bank directory status (exists/not exists)
3. List of existing Memory Bank files if any
4. Project type detection (look for package.json, requirements.txt, go.mod, Cargo.toml, pom.xml, build.gradle, .csproj, README.md, etc.)
5. Main technologies and frameworks detected
6. Project structure overview
7. Existing documentation files
8. Any other relevant project characteristics

Please provide a structured analysis that will help determine the best initialization strategy for the Memory Bank system."

### 2. **Adaptive Initialization Strategy**

Based on the Task tool's analysis results:

   **If Memory Bank doesn't exist:**
   - Create fresh Memory Bank structure
   - Use detected project information for initial content
   - Guide user through any missing information

   **If Memory Bank partially exists:**
   - Preserve all existing files
   - Create only missing files
   - If `projectbrief.md` exists, read and use it to inform other files

   **If projectbrief.md already exists:**
   - Read and parse its content thoroughly
   - Use it as the foundation for other files
   - Skip redundant questions
   - Maintain consistency with existing documentation

### 3. **Intelligent Information Gathering**

   **From the Task tool's analysis:**
   - Extract project name from configuration files
   - Parse README.md for project description
   - Identify technologies from dependency files
   - Understand repository structure

   **Interactive refinement:**
   - Present detected information to user for confirmation
   - Ask only for missing critical information
   - Clarify project goals and requirements
   - Respect user's time by minimizing questions

### 4. **Create/Update Memory Bank Files**

   Create these files (only if they don't exist):
   - `memory-bank/projectbrief.md` - Foundation document with project overview
   - `memory-bank/productContext.md` - Product vision, problems solved, user goals
   - `memory-bank/activeContext.md` - Current state, recent changes, next steps
   - `memory-bank/systemPatterns.md` - Architecture, design patterns, key decisions
   - `memory-bank/techContext.md` - Technology stack, setup, dependencies
   - `memory-bank/progress.md` - Development status, completed features, roadmap

   For each file:
   - Check existence before creating
   - Populate with meaningful content from analysis
   - Include helpful section comments
   - Maintain consistency across all files

### 5. **Finalize Setup**
   - Display comprehensive summary:
     * Files created vs preserved
     * Detected project information
     * Key decisions made during initialization
   - Provide contextual next steps:
     * For new projects: suggest `/workflow:understand` to explore
     * For existing projects: suggest `/workflow:plan` for next feature
     * For updated Memory Banks: suggest reviewing changes
   - Confirm Memory Bank is ready for use

## Important Implementation Guidelines

- **Preservation First**: Never overwrite existing files without explicit user permission
- **Intelligent Defaults**: Use Task tool analysis to provide smart defaults
- **Consistency**: If projectbrief.md exists, all other files must align with it
- **User Control**: Always show what will be done before doing it
- **Platform Agnostic**: Task tool ensures cross-platform compatibility
- **Meaningful Content**: No empty templates - populate with real project information

## Success Criteria

- Task tool provides comprehensive project analysis
- Existing Memory Bank files are preserved and respected
- New files contain project-specific, meaningful content
- User effort is minimized through intelligent detection
- The Memory Bank accurately reflects project reality
- Clear guidance provided for next steps