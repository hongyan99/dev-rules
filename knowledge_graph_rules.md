# Knowledge Graph Rules

## Purpose
This document outlines rules and guidelines for using the Knowledge Graph (KG) to maintain project context across multiple sessions.

## Core Principles

1. **Continuity First**: The Knowledge Graph serves as persistent memory across sessions
2. **Single Source of Truth**: Keep KG information consistent with project files
3. **Structured Representation**: Use consistent entity and relation types
4. **Accessible Context**: Store information in a way that's easy to retrieve

## Entity Types

Use these standard entity types for consistency:

| Entity Type | Purpose | Example |
|------------|---------|---------|
| Project | Main project container | "Expense Data Project" |
| Component | Code modules and structures | "Config Module" |
| Issue | Problems and bugs | "LLM Response Parsing Issue" |
| Status | Current working state | "Current Working State" |
| Session | Record of work done | "Session 2023-03-22" |
| Adapter | External service adapters | "GPT Adapter" |
| Documentation | Project structure info | "Project File Structure" |
| Configuration | Settings and options | "Default Settings" |
| Meta | KG usage information | "Session Starter" |
| Rule | Rules for development | "CONVERSATION_RULE" |

## Relation Types

Use these standard relation types for consistency:

| Relation Type | Purpose | Example |
|--------------|---------|---------|
| has_component | Links project to parts | Project → Component |
| has_issue | Shows problem areas | Component → Issue |
| part_of | Shows hierarchy | Subcomponent → Component |
| uses | Shows dependencies | Component → Service |
| configured_by | Configuration relationship | Adapter → Config |
| related_to | Loose connection | Component → Component |
| affects | Impact relationship | Issue → Status |
| implements | Implementation relationship | Component → Interface |
| documents | Documentation relationship | Session → Status |
| references | Reference relationship | Rule → Component |
| addresses | Work on an issue | Session → Issue |
| discusses | Session topic | Session → Component |

## Usage Guidelines

### When to Update

- **New Components**: Add when creating new modules or services
- **New Issues**: Add when bugs or problems are identified
- **Status Changes**: Update when project state changes
- **Sessions**: Add new session entity after each working session
- **Issue Resolution**: Update when issues are fixed
- **Major Decisions**: Document important architectural choices

### Information Storage

- **Keep it Relevant**: Only store information needed for context
- **Focus on Structure**: Emphasize relationships between components
- **Store Locations**: Include file paths for easier navigation
- **Prioritize Issues**: Ensure current problems are clearly identified
- **Update Status**: Keep the "Current Working State" entity updated

### Access Patterns

- **Project Entry**: Start with the main project entity
- **Current Status**: Check "Current Working State" for overview
- **Issues**: Query for entity type "Issue" to see all problems
- **Component Details**: Look up specific components by name
- **Session History**: Query entity type "Session" for work history

## Synchronization

- **Rule Files**: Keep KG information synchronized with `project_context.md`
- **New Components**: Add components to both KG and project files
- **Issue Tracking**: Update issue status in both KG and project files
- **Session Records**: Document sessions in both KG and session history

## Reserved Names

- **CONVERSATION_RULE**: Entry point for conversation context
- **Session Starter**: Contains KG usage hints for new sessions

## Example KG Queries

```
# Get all project components
search_nodes(query="Component")

# Check current issues
search_nodes(query="Issue")

# Get specific component details
open_nodes(names=["Config Module"])

# Get project history
search_nodes(query="Session")
```

## Maintenance

- **Periodically review** for outdated information
- **Remove resolved issues** that are no longer relevant
- **Update relation types** if project structure changes
- **Ensure entry points** remain accessible
- **Clean up obsolete entities** that no longer apply

---

*Created: 2023-03-22 | Last Updated: 2023-03-22*