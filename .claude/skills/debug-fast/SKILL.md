
---
name: debug-fast
description: Diagnose and fix coding errors quickly, including frontend bugs, Java and Spring Boot errors, API failures, database issues, AI integration problems, and build failures.
---

# Fast Debugging

## Objective
Find the root cause of a bug and implement the smallest reliable fix while preserving existing functionality.

## Instructions

### 1. Understand the failure
- Read the complete error message, stack trace, and relevant logs.
- Identify the expected behavior and the actual behavior.
- Determine which component is failing: frontend, backend, API, database, AI integration, configuration, or build system.
- Reproduce the problem when possible.
- Do not guess at the root cause without evidence.

### 2. Inspect before editing
- Read the relevant source files and their callers.
- Check recent changes and Git diffs when useful.
- Inspect API contracts, environment variables, dependency versions, and request/response formats.
- Check whether another teammate's module or shared interface is involved.
- Avoid broad refactors during urgent debugging.

### 3. Fix systematically
- State the most likely root cause and supporting evidence.
- Propose the smallest appropriate change.
- Preserve existing behavior and project conventions.
- Do not replace real functionality with hardcoded demo data unless explicitly requested as a temporary fallback.
- Never expose, print, or commit secrets.
- Do not disable authentication, validation, security checks, or tests merely to make the error disappear.

### 4. Verify the fix
- Run the narrowest relevant test or reproduction first.
- Run available build, type-check, or test commands when practical.
- Inspect the resulting logs and responses.
- Check for regressions in related functionality.
- Clearly state which checks passed, failed, or could not be run.

### 5. Work efficiently under a deadline
- Fix blockers before cosmetic issues.
- Prefer a minimal, reversible patch.
- If a complete fix is too risky, explain a safe temporary workaround and its limitations.
- Do not make unrelated edits.
- Do not claim success without verification.

## Required Output

Return:

1. Symptom and impact.
2. Evidence from logs or source code.
3. Root cause, or the leading hypothesis if unconfirmed.
4. Exact files that need changing.
5. Minimal fix and reasoning.
6. Verification commands and results.
7. Remaining risks or follow-up work.

If modifying the repository, summarize the changes made. If the evidence is insufficient, ask for the smallest missing piece of information instead of inventing an explanation.
