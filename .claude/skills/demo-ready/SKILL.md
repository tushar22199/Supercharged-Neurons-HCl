
---
name: demo-ready
description: Prepare a hackathon project for final judging by verifying core features, testing the end-to-end demo, checking deliverables, and preparing technical explanations.
---

# Demo Ready

## Objective
Determine whether the application is ready for a live hackathon demonstration. Find critical failures early and prepare the team to explain the implementation honestly and confidently.

## Instructions

### 1. Verify mandatory requirements
- Read the original case statement and acceptance criteria.
- Create a checklist of mandatory requirements.
- Map each requirement to its implementation and a verification step.
- Mark each item as VERIFIED, FAILED, PARTIAL, or NOT TESTED.
- Never mark a feature verified without evidence.

### 2. Test the end-to-end workflow
- Identify the main user journey that demonstrates the core value.
- Check frontend-to-backend requests and database persistence.
- Verify AI or external service integrations when applicable.
- Check success states, error states, empty inputs, and loading behavior.
- Test the complete workflow in the same order planned for the live demo.
- Confirm that required services, environment variables, and seed data are available.

### 3. Find demo blockers
Prioritize:
1. Application fails to start.
2. Main user journey fails.
3. Backend, database, or external integration is unavailable.
4. Required data cannot be demonstrated.
5. Authentication or permissions block expected usage.
6. Important errors or confusing UI behavior appear during the demo.

Recommend the smallest reliable fix for each blocker. Avoid risky last-minute refactors.

### 4. Verify technical quality
- Run relevant tests and build checks.
- Check browser console and server logs where available.
- Verify API error handling and data persistence.
- Ensure secrets are not committed.
- Check that the README's setup instructions match the actual project.
- State any tests or checks that could not be run.

### 5. Prepare the live demo
Create a short, reproducible demo script containing:
- Opening problem statement.
- Target user and key benefit.
- Step-by-step actions to perform.
- Expected visible results.
- Technical differentiator.
- A fallback if a network or external service fails.

Prefer a reliable, tested workflow over a long feature tour. Use only real functionality and clearly label any simulated data.

### 6. Prepare individual explanations
For each teammate, outline:
- Their actual contribution.
- The files and modules they implemented.
- The technical decisions they made.
- One challenge they solved and how they solved it.
- How their module connects to the rest of the application.
- Likely technical questions and concise answers.

Do not invent contributions or claim understanding of code that has not been reviewed.

### 7. Check final deliverables
Review:
- Working live demo and deployment status.
- GitHub repository and commit history.
- README with setup, architecture, features, and known limitations.
- Team presentation with problem, solution, architecture, implementation, results, and future improvements.
- Environment and startup instructions.
- Final known-issues list.

## Required Output

1. Readiness summary.
2. Mandatory-requirement verification checklist.
3. End-to-end test results.
4. Blockers ordered by severity and recommended fixes.
5. Demo script with expected results.
6. Individual teammate explanation guide.
7. README and presentation checklist.
8. Final go/no-go recommendation.

Distinguish verified results from assumptions and untested areas. Do not claim deployment, testing, or successful execution without evidence.

Do not modify files, deploy, push commits, or change configuration unless explicitly asked.
