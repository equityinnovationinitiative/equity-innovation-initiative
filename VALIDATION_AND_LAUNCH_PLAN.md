# Validation and implementation strategy

## Current conclusion
A local, offline, functioning **deterministic** prototype screens document manifests and provides an interactive public explanation. Nine unit tests pass. It does not parse original contract documents, verify digital signatures, use an AI model, or establish compliance with applicable procurement rules. Accordingly it is **not yet independently validated** for real-world procurement decisions. This is the defensible finish line for the current prototype, not full deployment.

## Next technical evidence gate
1. Obtain permissioned, timestamped **historical** contract-file documents and associated metadata; preserve original hashes, provenance, revisions and as-of availability.
2. Build a document extraction layer (PDF/text, OCR only when required), with page-specific source citations, explicit uncertainty, and human-verifiable excerpts.
3. Map applicable FAR/agency requirements and exceptions as of each award date, with procurement-counsel review. Do not assume every document is mandatory in every acquisition.
4. Blindly label independent examples with at least two expert reviewers and resolve disagreement. Measure precision, recall, false positives, missed issues, and time-to-review by alert category. Avoid claiming performance from synthetic tests.
5. Add an optional LLM-assisted *explanation* component with source-constrained retrieval, audit logging, redaction, prompt-injection testing, and mandatory human approval. Compare against deterministic baseline; deploy AI only if it improves measured performance.
6. Independent security, accessibility, privacy and procurement/legal review before any government pilot. Do not expose controlled or sensitive contract files in a public website.

## Product choice
**Public-facing website + interactive demo** first, not native mobile app. Audiences are procurement professionals, OIG staff, researchers, watchdog groups and journalists; they need sources, reproducible outputs and downloadable reports. The eventual internal government product would be a secure, permissioned web application/API integrated into existing systems—not this public site.

## Proposed website structure
Home: one-sentence promise and three-minute demo; Case Study: real records and limitations; Try Demo: synthetic examples; Methods: reproducible code, source provenance and error reporting; Pilot: evaluation criteria and security boundaries; Contact: requests for expert review. Publish corrections and version history.

## Outreach sequence
- Stage 1: recruit two independent reviewers (one federal acquisition specialist and one software/data-quality specialist); ask for critique, not endorsement.
- Stage 2: publish corrected demonstration and a concise 2–3-minute walkthrough video. Show one clearly synthetic pre-award alert and one reconciled real-data analysis; distinguish them visually.
- Stage 3: approach nonpartisan procurement research groups, university public administration programs, inspector general innovation teams, and agency acquisition offices with a **narrow pilot proposal**.
- Stage 4: invite independent journalism and broader public discussion only after technical review. Avoid partisan branding and unverified fraud allegations.
- Stage 5: propose a limited, read-only pilot using non-sensitive records, with pre-agreed metrics and stop conditions. Any authorized internal integration is a separate security and governance project.

## Pilot success criteria (targets to agree with host, not measured results)
- Reproducible evidence links for every actionable alert.
- Measured precision/recall on an independent labeled sample, with explicit acceptable thresholds agreed by host.
- Lower median time for reviewers to locate relevant documents compared with manual baseline.
- Clear human override, correction, audit trail, retention policy and independent oversight.
- No automatic legal, enforcement, or adverse personnel determinations.

## 90-day plan (5–10 hours/week)
Weeks 1–2: publish demo and methods; expert feedback. Weeks 3–5: obtain permitted sample documents and implement extraction. Weeks 6–8: label independent test set and run blind evaluation. Weeks 9–10: refine, publish correction log and record video. Weeks 11–13: outreach to 5–10 relevant organizations, seek one scoped pilot conversation. **External access and responses are dependencies, not guaranteed outcomes.**

## Low-cost budget
Existing remaining personal allocation: **$230**. Development and testing so far: $0 additional. Optional later: domain ~$12–25/year; static hosting often free; small contingency for video/hosting. Do not purchase until project name and launch content are approved. Verify current provider prices before spending.

## Intellectual property and trust
Publish enough source and methodology for independent reproduction, choose a clear code license before public release, maintain a conflict-of-interest disclosure, publish errors and corrections, and prohibit claims that the system identifies fraud or wrongdoing from metadata alone.
