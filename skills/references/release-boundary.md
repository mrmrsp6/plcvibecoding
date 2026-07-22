# Capture and Release Boundary

Use this reference when PLC work depends on traces, engineering snapshots, or deployment.

## Preserve Evidence

- Keep references to traces, snapshots, logs, decoded outputs, or exported project files.
- Record which evidence supports each conclusion.
- Do not discard regression inputs after one successful answer.
- Avoid embedding file paths, case identifiers, or environment identifiers in public reports.

## Deployment Boundary

Treat these actions as requiring explicit user authorization:

- online modification of a controller
- project overwrite or repackaging for deployment
- download to runtime hardware
- change to a production-facing configuration

Generated code, patches, or review comments are planning artifacts only. They do not imply
permission to deploy.

## Public Reporting

Keep reports generic and reusable:

- summarize evidence categories rather than internal collection mechanics
- describe risks and validation needs plainly
- avoid tool names, workflow internals, and project layout
