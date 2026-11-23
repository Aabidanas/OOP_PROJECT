# MatchBack — Team Decisions & Integration

This file records **proposed and approved** shared decisions. Do not infer approval merely because a proposal appears here.

## Approved baseline from the master brief

- Application: Java desktop lost-and-found matching system using Swing.
- Storage: local file handling (exact file format pending).
- Matching: explainable rule-based scores, with weights initially proposed at 30/20/20/15/15.
- Module ownership: `matchback.model`, `matchback.matching`, `matchback.ui`, `matchback.repository`, `matchback.claims`.
- AI integration is outside the initial implementation.
- `main` should contain reviewed code; members use their named feature branches.
- Submission: 30 November 2026; demo: 4–7 December 2026.

## Pending team decisions (not yet approved)

| Decision | Affected modules | Status |
| --- | --- | --- |
| Java/JDK version and build/run procedure | All five | Pending |
| Shared `ItemReport` fields, constructors, accessors, validation | Model, matching, UI, storage, claims | Pending |
| `LostItem` / `FoundItem` status names and transition rules | Model, UI, storage, claims | Pending |
| Matching interface signature, inputs, `MatchResult` contract | Model, matching, UI | Pending |
| Local storage format, path and schema/versioning | Model, storage, claims, UI | Pending |
| Claim interface, private verification data handling | Model, claims, UI, storage | Pending |
| Service/coordinator wiring between Swing and modules | UI, matching, storage, claims, model | Pending |

## Decision template

### Decision ID: D-XXX — Title
- **Status:** Proposed / Approved / Superseded
- **Date:**
- **Owners and affected modules:**
- **Decision and rationale:**
- **Exact Java API signatures or schema, if relevant:**
- **Migration/compatibility implications:**
- **Evidence of team approval (issue/PR link):**

## Integration acceptance checklist

- [ ] All member branches are reviewed before merging into `main`
- [ ] Application compiles and starts with the documented JDK
- [ ] Lost/found registration works and creates unique report IDs
- [ ] Reports persist after application restart
- [ ] Suggested matches show scores and explanations
- [ ] Claims and private identifiers are handled safely
- [ ] Search/filter and dashboard interactions work
- [ ] Error cases are checked without crashing
- [ ] Report, UML, screenshots, and demo are ready

**Important:** Checklist items are unverified until tested. This file is not proof of implementation.
