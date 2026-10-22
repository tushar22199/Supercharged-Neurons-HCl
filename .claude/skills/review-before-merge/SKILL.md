
---
name: review-before-merge
description: Review code changes before merging into the shared hackathon branch, checking correctness, security, API compatibility, integration risks, and tests.
---

# Review Before Merge

## Objective
Review proposed changes before merging them into the shared project. Prioritize bugs that could break the working application or hackathon demo.

## Instructions

### 1. Inspect the changes
- Read the Git diff and identify the purpose of each change.
- Inspect relevant surrounding code and callers.
- Check whether changes are limited to the intended feature.
- Identify accidental deletions, unrelated edits, and generated files that should not be committed.
- Never assume code is correct just because it compiles.

### 2. Check correctness
- Look for logic errors, incorrect conditions, missing edge cases, and unsafe assumptions.
- Check null values, empty inputs, invalid formats, and error handling.
- Identify possible crashes, race conditions, duplicate submissions, and inconsistent state.
- Verify that new code preserves existing functionality.

### 3. Check integration compatibility
- Compare API endpoints, HTTP methods, request fields, response formats, and error responses with the agreed contracts.
- Check frontend-to-backend integration and database schema compatibility.
- Verify shared types, imports, environment variable names, and configuration.
- Identify conflicting assumptions between teammates' modules.
- Flag changes to shared files that could disrupt parallel work.

### 4. Check security
- Look for exposed API keys, passwords, tokens, or private configuration.
- Check authentication and authorization where applicable.
- Review input validation, SQL query safety, and sensitive data handling.
- Flag unsafe CORS settings, disabled security controls, and untrusted file uploads.
- Never copy secret values into the review report.

### 5. Check testing and maintainability
- Identify missing tests for important new behavior.
- Check whether existing tests or build steps may fail.
- Prefer focused, meaningful tests over superficial coverage.
- Flag brittle hardcoded values, unnecessary dependencies, and duplicated logic when relevant.
- Do not demand unrelated refactoring during the hackathon.

### 6. Report findings by severity
Use these levels:
- BLOCKER: prevents safe integration or breaks a mandatory demo flow.
- HIGH: likely functional, security, or data-integrity problem.
- MEDIUM: meaningful bug or missing edge-case handling.
- LOW: minor maintainability or style issue.

For each finding, include:
- Severity.
- File and line number when available.
- Concrete problem and its impact.
- A practical fix.

Do not report speculative issues as confirmed defects.

### 7. Recommend a merge decision
Choose one:
- APPROVE: no significant issues found in the reviewed changes.
- APPROVE WITH FOLLOW-UPS: safe to merge, with clearly stated non-blocking improvements.
- REQUEST CHANGES: fix blockers or important issues before merging.

Do not merge, push, or modify files unless explicitly asked.

## Required Output

1. Overall merge recommendation.
2. Findings ordered by severity.
3. API and cross-module compatibility checks.
4. Tests and checks performed, including failures.
5. Remaining risks and suggested next steps.

If no significant issues are found, say so clearly. Do not invent findings to fill the report.
