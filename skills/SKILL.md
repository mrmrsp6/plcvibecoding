---
name: plc-public-workflow-guard
description: Public, general PLC assistance guardrails for evidence collection, request routing, patch planning, capture preservation, prompt separation, and deployment approval. Use when reviewing or supporting PLC or ladder-logic tasks with a conservative, vendor-neutral checklist.
---

# PLC Public Workflow Guard

## Public Scope

Use this skill as a lightweight public checklist for PLC assistance. Keep it generic.
Do not include organization-specific architecture, case-specific data, proprietary validation
rules, or deployment-specific procedures.

## Core Workflow

1. Classify the request as general discussion, read-only analysis, new program design,
   patch planning, review, or deployment-related work.
2. Collect enough evidence before answering: relevant logic excerpts, device usage,
   comments or labels, diagnostics, constraints, and any user-provided context.
3. Separate verified structure from inferred meaning. Mark uncertain, conflicting, or
   missing information instead of presenting it as fact.
4. For patch work, require a clear target, a minimal change, and a validation plan.
   Never guess across missing structure.
5. Treat deployment as a separate approval boundary. A generated patch is
   not permission to modify a live controller or production project.
6. Preserve evidence references that were used to justify the answer, especially for
   later regression checks.

## When More Detail Is Needed

- Read `references/evidence-routing.md` for a public routing and evidence checklist.
- Read `references/patch-safety.md` for generic patch planning constraints.
- Read `references/release-boundary.md` for capture preservation and deployment gating.

Keep final answers practical and modest: describe what is known, what remains uncertain,
and what should be validated before any operational change.
