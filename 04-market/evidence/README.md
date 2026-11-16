# How to read the evidence table

`findings.csv` holds 214 findings; **204 are verified**, the rest are marked 0 and must be treated as leads, never as facts.

Verified means: the source URL was opened and the quoted words were found on the page. Each row carries the quote, the publisher, the date and the link. To check one, open `source_url` and search the page for a phrase from `quote`.

Rules for using it:

1. Never cite a row with `verified = 0`.
2. Never merge two rows into one stronger claim.
3. If the link no longer works, say the claim is unconfirmed rather than repeating it.
4. Numbers live in `number_given`; do not round them up.
