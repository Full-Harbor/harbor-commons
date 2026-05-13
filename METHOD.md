# Harbor Commons — Method

## What Harbor Commons is actually proving

Harbor Commons is not just a website.
It is a working proof that public nonprofit records can be turned into shared, reusable infrastructure for a field that normally treats analysis as bespoke labor.

The core method is simple:
1. Start from public records
2. Preserve source provenance
3. Extract structured fields conservatively
4. Keep judgment separate from raw evidence
5. Publish only what is appropriate for the public layer

## Design principles

### 1. Receipts first
Every meaningful claim should resolve back to a filing, schedule, extracted field, or quoted document.

### 2. Public methods, private judgment
Generic extraction logic, schemas, and source-handling patterns belong in the public layer.
Application-specific scoring, private cohort flags, and strategic interpretation do not.

### 3. Build once, reuse across a field
The point is not to help one organization do analysis once.
The point is to reduce duplicated labor for dozens or hundreds of organizations that face the same questions.

### 4. Example 1, not the limit
Sailing is the first worked example because that is where the method was built.
Nothing in the underlying logic depends on sailing being the permanent boundary.

## Components

### IRS filing extraction
Harbor Commons depends on reproducible IRS 990 / 990-EZ / 990-PF extraction logic. That logic now lives publicly in [`irs-990-extract`](https://github.com/Full-Harbor/irs-990-extract).

### PDF ingestion and provenance
When the source is a PDF rather than structured XML, Harbor Commons uses a canonical pipeline that hashes, OCRs, chunks, and preserves provenance. That logic now lives publicly in [`pdf-goat`](https://github.com/Full-Harbor/pdf-goat).

### Product-facing public layer
Harbor Commons is the human-usable surface where those methods become something boards, practitioners, and funders can actually use.

## What gets published here

- Product framing
- Public method summaries
- Architecture logic
- Field-level positioning

## What does not get published here

- Private grantmaking cohorts
- Named judgment calls about live organizations
- Application-specific research tracks
- Sensitive internal scoring layers

## What success looks like

A small-field organization, network, or funder can fork the method, adapt it to its own domain, and start from infrastructure instead of from scratch.
