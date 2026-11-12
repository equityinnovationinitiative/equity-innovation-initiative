# Real-data findings — AIC-001

**Source:** User-supplied USAspending award CSV export for HHS contract PIID `75ACF121P00005` (Family Endeavors, Pecos Emergency Intake Site). Original downloadable records remain outside this package; no sensitive source data is republished here.

- 17 transaction actions; 88 federal-account funding records; zero records in the provided subaward export.
- Total summed federal action obligations: **$713,907,435.33**.
- Federal-account funding amounts sum to the same amount; **reconciliation passes**.
- 16 exploratory screening alerts: 4 modification description/reference differences; 7 report-date-before-action-date relationships; 4 obligation changes above an **arbitrary $50M threshold**; 1 empty subaward export notice.
- Modification description references that differ from the action's modification number: P00006 refers to P00005; P00012, P00013, P00014 refer to P00007. These may reflect legitimate descriptions of previous actions.
- Aggregate award totals repeated on transaction rows are **not historical ceiling snapshots**. Cannot infer a ceiling breach by comparing them to an initial ceiling.
- Obligations are **not** payments, losses, fraud, or proof of wrongdoing. Empty subaward export is **not** proof of no subcontracting.
- Public exports alone cannot establish whether any flagged detail was visible at the historical action date. An early-warning claim requires contemporaneous records or an authorized archived dataset.

**Official audit context (not independently discovered by this prototype):** HHS OIG published a 2026 audit identifying procurement shortcomings for this award, including planning and pre-award evaluation issues. See: https://oig.hhs.gov/reports/all/2026/acfs-529-million-sole-source-contract-award-for-unaccompanied-alien-children-services-was-based-on-an-unsolicited-proposal-double-the-cost-estimate-and-noncompliant-with-pre-award-requirements/

**USAspending award page:** https://www.usaspending.gov/award/CONT_AWD_75ACF121P00005_7590_-NONE-_-NONE-

No finding of illegal activity or fraud is made here.
