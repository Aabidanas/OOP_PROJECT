# MatchBack — Java Lost-and-Found Matching System

**CS F213 Object Oriented Programming · BITS Pilani, Dubai Campus · 2026–27**

MatchBack is a planned Java Swing desktop application for reporting lost and found belongings, ranking potential matches using explainable rule-based scoring, and handling ownership claims.

> **Project status:** Repository setup in progress. No application functionality has been implemented or tested in this repository yet.

## Scope

The approved master brief calls for:
- Lost and found item registration, each with a unique report ID
- Explainable rule-based matching and ranked similarity scores (not verified probabilities)
- Search and filtering
- Ownership claims and review, while keeping private identifying details out of public listings
- Local data persistence across application restarts
- A Java Swing dashboard and forms

Initial proposed matching weights: category 30, colour 20, location 20, date proximity 15, description similarity 15 (100 total). These are **proposed**, not a final scoring contract.

## Module ownership

| Member | Responsibility | Java package | Feature branch |
| --- | --- | --- | --- |
| 1 | Core architecture / models | `matchback.model` | `feature/core-models` |
| 2 | Matching engine | `matchback.matching` | `feature/matching-engine` |
| 3 | Swing GUI | `matchback.ui` | `feature/gui` |
| 4 | Storage / search | `matchback.repository` | `feature/storage` |
| 5 | Claims / verification | `matchback.claims` | `feature/claims` |

These packages and responsibilities reflect the master brief. They do not indicate that classes already exist.

## Team workflow

1. Agree on Java version, storage format, project build/run setup, and shared model/interface contracts **before** implementing code that depends on them.
2. Each member works in their own feature branch and package.
3. Commit and push working changes; open a pull request for review before merging into `main`.
4. Do not change shared constructors, class names, method signatures, or data types without coordination with affected members.
5. Track architecture decisions in `docs/INTEGRATION_DECISIONS.md`. A chat discussion alone does not finalize a decision.
6. Verify the integrated application after merges. Never mark a feature implemented or tested without evidence.

## Project dates

- **23–25 November 2026:** Member module implementation and basic tests
- **26–27 November 2026:** Integration and full workflow testing
- **28–29 November 2026:** Fixes, report, screenshots and demo rehearsal
- **30 November 2026:** Submission deadline
- **4–7 December 2026:** Team demonstration and individual viva

## Submission and demo

Provide Java source code or GitHub link and a report (minimum 10 pages) according to the master brief. Prepare a printed report, a working desktop application, and a 5–10 minute demonstration attended by all five members.

## References

Project requirements: *MATCHBACK — MASTER PROJECT BRIEF* and the CS F213 course handout (2026–27). The course handout describes the Java/OOP learning outcomes; the master brief records project-specific requirements and deadlines.
