# Evidence and Routing Checklist

Use this reference for public PLC analysis or planning tasks.

## Route Lightly

- Keep non-PLC conversation outside the PLC workflow.
- Route read-only questions to analysis.
- Route requests to create or modify logic to design or patch planning.
- Route download, overwrite, or deployment requests to an approval-gated path.

Avoid organization-specific route names, prompt text, automation mechanics, or exact
product-specific heuristics.

## Evidence Checklist

Collect the smallest evidence set that can support a useful answer:

- project or program summary
- relevant logic excerpts
- device or tag usage
- comments, labels, or user annotations
- diagnostic messages or symptoms
- known constraints, timing assumptions, and safety limits
- vendor or platform rules when they are already known from public documentation or the user

## Confidence Handling

Use a small public vocabulary:

- `confirmed`: directly supported by evidence
- `inferred`: plausible but not directly proven
- `uncertain`: needs more evidence
- `conflicting`: evidence disagrees
- `blocked`: cannot proceed safely

Do not let scenario guesses replace missing logic structure. Ask focused questions when
the missing information affects safety, outputs, polarity, timing, units, or target identity.
