# The Equity & Innovation Initiative — website preview

Open `index.html` in a modern browser. The public-facing landing page and interactive AIC-001 demonstration run entirely offline. This is a **preview**, not a published website. No domain, hosting, organization registration, or contact inbox has been created.

## What is included
- `index.html`: mission-led, responsive website with a six-scenario interactive synthetic demonstration
- `engine.py`, `manifest_cases.json`, `demo_results.json`, `test_engine.py`: reproducible screening prototype and tests
- `REAL_DATA_SUMMARY.md`: analysis of supplied USAspending award export, distinct from synthetic examples
- `VALIDATION_AND_LAUNCH_PLAN.md`: external validation requirements
- `OUTREACH_EMAIL.md`: draft for future expert review outreach

## Reproduce the engine
From this folder run `python -m unittest -v` and `python engine.py manifest_cases.json --out demo_results.json`. The page embeds a snapshot of `demo_results.json`; after changing test scenarios, the page must be regenerated before the browser demo reflects them.

## Publication checklist
Confirm final name and domain availability, have a legal/technical reviewer check claims, decide whether to publish the prototype code and documentation, add a verified contact channel and privacy policy before collecting personal data, test accessibility and mobile layout, and select hosting. Do not present the proof of concept as AI-powered or production ready.
