# AIC-001 — Real Address Screening v2.3

## Data and result
Input: USAspending contract transaction history export for award 75ACF121P00005 (17 rows). The 17 rows contain **one distinct UEI** (`PC1AM3TAQXD8`) and **one reported recipient address**: 6363 DE ZAVALA RD STE 200, San Antonio, TX 78249-2104. **Zero address-pattern alerts** were generated.

This is a **valid negative control**, not evidence that the recipient has been externally verified or that no irregularities exist. The input does not include multiple recipient businesses. It cannot support claims of multi-business address clusters or cross-agency networks.

## Engine
`real_address_engine.py` accepts a USAspending-format CSV, groups transaction rows by recipient UEI, standardizes common street suffixes, and flags three-or-more distinct UEIs at one reported address, multiple reported addresses for one UEI, incomplete addresses, and PO box patterns. PO boxes are informational unless additional rules establish a physical location requirement.

The engine does not check USPS deliverability, actual building occupancy, property dimensions, ownership, registered agents, payments, or fraud. The threshold of three is exploratory, not a regulatory standard.

## Reproduce
`python real_address_engine.py Contract_75ACF121P00005_TransactionHistory_1.csv --output real_address_screening.json`

`python -m unittest discover -p 'test_*.py'`

## Next independent validation
Acquire a legally reusable multi-award USAspending recipient export, retain source and download date, screen distinct UEIs across awards, manually verify a stratified sample of both flagged and unflagged cases, and report precision and false positives. No outside registry or postal verification has been performed yet.
