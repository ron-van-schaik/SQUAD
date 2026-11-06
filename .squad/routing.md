# Work Routing

Select one accountable DIT specialist for each task. Preserve the user's requested
scope; the owner may ask for narrowly bounded input, but may not expand the work
without approval.

## Routing Table

| Work Type | Route To | Examples | Responsibility boundary |
|-----------|----------|----------|--------------------------|
| New request, unclear ownership, intake, prioritization, or coordination | Lead & Intake Coordinator | intake, prioritization, handoff | Clarifies the requested outcome, assigns one accountable owner, and coordinates handoffs. Does not silently broaden scope. |
| Cloud-related processes, process steps, roles, handoffs, or process clarity | Cloud Process Analyst | cloud process, process steps, dependencies | Analyzes processes only; does not presume a provider, platform, or system. |
| Service delivery flow, service outcomes, delivery handoffs, or delivery measures | Service Delivery Analyst | service delivery, service outcomes, delivery measures | Analyzes delivery and makes findings traceable to the stated request. |
| Evidence quality, audit trail, traceability, or audit readiness | Evidence & Audit Specialist | evidence, traceability, audit readiness | Defines/assesses evidence and traceability needs; does not claim compliance absent stated criteria and evidence. |
| Operational assumptions, feasibility questions, dependencies, failure modes, or risk challenge | Technical Operations Challenger | operational assumptions, failure modes, risk | Challenges and explains operational implications; does not change company systems. |
| Data handling, data structure, or automation design/implementation explicitly in scope | Data & Automation Engineer | data structure, automation design, data handling | Works only within an explicitly approved boundary; no system changes are implied by this route. |
| Independent quality review, acceptance criteria, completeness, or focused work notes | Quality Reviewer & Scribe | quality review, acceptance criteria, completeness | Reviews the deliverable and records bounded work notes; distinct from built-in Scribe. |

When a task crosses domains, the Lead & Intake Coordinator selects one owner
according to the primary requested outcome. Add another specialist only for a
specific, separately bounded contribution that the owner cannot cover. Review is
not automatic; the coordinator applies the repository's governance and review
requirements when relevant.

## Issue Routing

| Label | Action | Who |
|-------|--------|-----|
| `squad` | Triage the request and assign one accountable specialist | Lead & Intake Coordinator |
| `squad:{specialist-id}` | Work the assigned issue within the approved scope | Named DIT specialist |

Specialist IDs are the lowercase role slugs: `lead-intake-coordinator`,
`cloud-process-analyst`, `service-delivery-analyst`, `evidence-audit-specialist`,
`technical-operations-challenger`, `data-automation-engineer`, and
`quality-reviewer-scribe`.

Scribe, Ralph, Rai, and Fact Checker are built-in Squad support identities, not
DIT roles or ordinary issue-routing destinations. Invoke them only for their
framework support functions. The optional `@copilot` entry is not enabled for
automatic assignment.

## Collaboration and Routing Rules

1. Assign exactly one accountable specialist per work item.
2. Do not fan out speculatively or start anticipatory downstream work. Split only
   independently deliverable outcomes with distinct owners.
3. Keep collaboration bounded to a concrete question, artifact, or review need;
   the accountable owner retains responsibility for the result and handoff.
4. Route quick factual questions directly when no specialist judgment is needed.
5. Scope expansion, knowledge-source/tool inventories, and company-system changes
   require explicit user approval; they are outside the approved setup phase.
6. Route decisions that affect team-wide behavior through `.squad/decisions.md`;
   only the coordinator records accepted decisions there.
