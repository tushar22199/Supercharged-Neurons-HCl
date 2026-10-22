
---
name: case-analysis
description: Analyze hackathon problem statements, identify requirements, plan the MVP, design APIs, and divide implementation across four teammates.
---

# Hackathon Case Analysis

## Objective
Turn the provided hackathon case statement into an actionable implementation plan. Prioritize a working, reliable demo within the available time.

## Instructions

### 1. Understand the problem
- Read the complete problem statement before proposing a solution.
- Identify the target users, their problem, and the expected outcome.
- Extract every explicit functional and technical requirement.
- Separate mandatory requirements, optional enhancements, and judging criteria.
- List ambiguities and state assumptions clearly.

### 2. Define the MVP
- Identify the smallest end-to-end solution that satisfies the core requirements.
- Prioritize features by importance, implementation time, and demo impact.
- Define acceptance criteria for each mandatory feature.
- Keep optional features out of the critical path until the MVP works.

### 3. Select the architecture
- Respect the required technology stack and any stated restrictions.
- Prefer a simple architecture that the team can build and explain.
- Identify the frontend, backend, database, AI components, and external integrations as applicable.
- Define the data flow from user input to final output.
- Do not introduce unnecessary technologies or services.

### 4. Define interfaces before parallel work
- Specify API endpoints, HTTP methods, request bodies, response bodies, and error formats.
- Identify database entities, important fields, and relationships.
- Define shared types and expected environment variables.
- Flag dependencies between team members before implementation begins.

### 5. Divide work across four teammates
Propose four concrete, independently testable assignments:
1. Frontend and user experience.
2. Backend APIs and database.
3. Core business logic, AI functionality, or domain-specific processing.
4. Integration, automated tests, and a meaningful technical feature.

Adapt these assignments to the actual case. Do not leave the fourth teammate responsible only for documentation or project management.

For every assignment, specify:
- Files or modules owned.
- Inputs and outputs.
- Dependencies on other teammates.
- Acceptance criteria.
- A clear integration point.

Avoid assigning multiple teammates to edit the same files simultaneously.

### 6. Plan execution
Provide:
- A prioritized task checklist.
- A suggested time budget based on the actual deadline.
- Integration checkpoints.
- A testing plan.
- A demo sequence that proves the mandatory requirements.
- Major risks and fallback options.

### 7. Keep the project reliable
- Keep the main branch runnable.
- Use small, focused commits and separate feature branches when appropriate.
- Never hardcode API keys, passwords, or other secrets.
- Do not claim that a feature works unless it has been verified.
- Prefer a tested basic implementation over an ambitious, unfinished solution.

## Required Output

Return the analysis in this order:

1. Problem summary.
2. Mandatory requirements and judging priorities.
3. Assumptions and unresolved questions.
4. MVP scope and acceptance criteria.
5. Recommended architecture and data flow.
6. API contracts and database design.
7. Four teammate assignments.
8. Time-boxed execution plan.
9. Testing and integration checklist.
10. Demo plan, risks, and fallback strategy.

Be specific, concise, and implementation-oriented. Do not start changing project files during analysis unless explicitly asked.
