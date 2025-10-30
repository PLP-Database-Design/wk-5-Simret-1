# 🧪 Final Group Test Report Template — Word Puzzle Game Plus

**Level:** Intermediate QA | **Week 5:** Test Management

**Course:** Software Testing & Quality Assurance  
**Module:** Test Management (Week 5)  
**Project Type:** Group Assessment  
**Submission Date:** 2025-11-30

## Team Information

| Role | Name | Responsibilities |
|------|------|------------------|
| Test Manager | Simret | Planning, scheduling, coordination, metric tracking |
| Risk Analyst | Simret | Risk identification, prioritization, test design linkage |
| Test Executor | Simret | Execution, evidence capture, defect logging |

## Group Rules

- Each student must belong to only one group.
- Duplicate membership or multiple submissions will result in invalidation.
- Every group member must contribute towards this project

## Project Overview

**System Under Test:** Word Puzzle Game Plus  
**Technology Stack:** HTML, CSS, JavaScript  
**Environment:** Chrome Browser (Desktop)

### Features Under Test

| Feature | Description | Risk Category |
|---------|-------------|---------------|
| Reset Game | Clears score and progress instantly | High |
| Leaderboard | Stores top 3 scores in localStorage | Medium |
| Bonus Round | Every 3 puzzles → doubles score | Critical |

## Test Plan

### Objectives

- Validate correctness and stability of new features: Reset Game, Leaderboard, and Bonus Round.

- Assess data integrity, state management, and UI consistency after user actions.

- Identify, prioritize, and mitigate high-risk areas through risk-based testing.

- Ensure defect tracking, metrics monitoring, and controlled regression testing.

### Scope

**In Scope:**
- Functional testing of:

Reset Game (state reset and persistence)

Leaderboard (localStorage top-3 logic)

Bonus Round (scoring arithmetic and triggers)

- UI behavior and event sequencing

- Cross-browser validation (Chrome focus)

- Risk-based and boundary testing

**Out of Scope:**
- Backend integrations (none implemented)

- Performance load testing

- Accessibility beyond basic ARIA role checks

### Tools & Resources

- Chrome DevTools
- Screenshots

### Schedule

| Phase | Planned Duration | Actual Duration | Status |
|-------|------------------|-----------------|--------|
| Test Planning | 1 day | 1 day | Complete |
| Risk Analysis | 1 day | 1 day | Complete |
| Test Design | 2 days | 2 days | Complete |
| Test Execution | 2 days | 2 days | Complete |
| Monitoring & Reporting | 1 day | 1 day | Complete |


## Risk Analysis

### Risks

| ID | Feature | Risk Description | Likelihood | Impact | Priority | Mitigation Strategy |
|----|---------|------------------|------------|--------|----------|---------------------|
| R1 | Reset Game | State not cleared (score persists) | 3 | 4 | 12 - High | Verify variables reset; unit test on reset() |
| R2 | Leaderboard | Incorrect sorting or missing score | 2 | 5 | 10 - High | Test various score sequences; clear storage |
| R3 | Leaderboard | localStorage unavailable (quota, privacy) | 3 | 3 | 9 - Medium | Mock localStorage and fallback UI |
| R4 | Bonus Round | Incorrect score multiplier (math bug) | 3 | 5 | 15 - Critical | Verify modulo logic; regression after each fix |
| R5 | UI Controls | Reset or Submit unresponsive | 2 | 4 | 8 - Medium | Test event listeners and disable states |
| R6 | Data Integrity | Score overflow or NaN due to invalid data | 2 | 4 | 8 - Medium | Validate score type and boundary inputs |
### Risk Coverage
- Total Risks: 6

- Tested Risks: 5

- Untested Risks: 1 (R3 non-functional fallback)

- Risk Coverage Ratio: 5/6 = 83%


## Test Cases

| ID | Feature | Objective | Expected Result | Actual Result | Status | Risk Link |
|----|---------|-----------|----------------|---------------|--------|-----------|
| | | | | | | |
| | | | | | | |
| | | | | | | |
| | | | | | | |
| | | | | | | |
| | | | | | | |
| | | | | | | |
| | | | | | | |

## Defects

| ID | Issue Title | Severity | Risk ID | Status | GitHub Link |
|----|-------------|----------|---------|--------|-------------|
| | | | | | |

## Metrics

- Test Case Pass Percent: 
- Defect Density: 
- Risk Coverage Percent: 
- Regression Success Rate: 

### Defect Summary

- Total Defects Logged: 
- Critical High: 
- Fix Rate: 

## Test Control & Project Management

### Phases

| Phase | Deliverable | Actual Output | Variance | Owner |
|-------|-------------|---------------|----------|-------|
| | | | | |

**Progress Tracking Method:**  
**Change Control Notes:**

## Lessons Learned

- Most Defect Prone Feature: 
- Risk Analysis Impact: 
- Team Communication Effectiveness: 
- Improvements for Next Cycle: 

## Attachments

- 

## Sign Off

| Name | Role | Initials | Date |
|------|------|-----------|------|
| | Test Manager | Simret | Oct 30, 2025 |
| | Risk Analyst | Simret | Oct 30, 2025 |
| | Test Executor | Simret | Oct 30, 2025 |

## Overall Summary

**Statement:** 
- Risk-Based Testing Impact:
Risk analysis directly focused testing on the most error-prone logic (bonus scoring, leaderboard persistence). This improved time efficiency and prevented redundant low-value tests.

- Trade-offs:
Limited time prevented deep usability testing. Focus on high-risk features ensured coverage of most impactful defects.

- Collaboration Insights:
GitHub Issues streamlined communication between testers and developers. Immediate evidence uploads (screenshots) improved turnaround time for fixes.

I- mprovements:

Automate localStorage clearing between runs.

Implement unit tests for score calculation.

Add CI pipeline to track test metrics automatically.

Most Defect-Prone Feature: Bonus Round logic (arithmetic and trigger condition).

**Test Status:** ☐ Completed / ☐ In Progress / ☐ Deferred
