# Patch Safety Checklist

Use this reference for generic PLC patch planning and review.

## Required Before Planning

- Identify the target program, block, rung, network, tag, or device as specifically as possible.
- State the observed behavior and the intended behavior.
- Check nearby logic that could be affected by the change.
- Identify assumptions that still need confirmation.

## Patch Constraints

- Prefer the smallest change that satisfies the stated intent.
- Preserve existing structure and naming where possible.
- Do not rewrite unrelated logic.
- Do not invent missing devices, tags, interlocks, or safety conditions.
- Keep comments and executable logic separate.
- Include a validation plan that can be run offline or in a safe test environment first.

## Review Outcome

When evidence is incomplete, return a guarded plan rather than a confident patch. Include:

- the proposed change boundary
- the evidence used
- missing evidence or assumptions
- suggested tests
- rollback or review notes when appropriate
