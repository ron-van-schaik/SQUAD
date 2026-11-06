# DIT Squad

## Coordinator

| Name | Role | Notes |
|------|------|-------|
| Squad | Coordinator | Routes work, enforces handoffs and reviewer gates. |

## Members

The following are the **exact seven DIT specialist roles** approved for this team.
Only these specialists are used as domain destinations in `routing.md`.

| Name | Role | Charter | Status |
|------|------|---------|--------|
| Lead & Intake Coordinator | Intake, triage, accountable ownership, and coordination | `.squad/agents/lead-intake-coordinator/charter.md` | Active DIT specialist |
| Cloud Process Analyst | Cloud-related process analysis and process clarity | `.squad/agents/cloud-process-analyst/charter.md` | Active DIT specialist |
| Service Delivery Analyst | Service delivery analysis and outcome clarity | `.squad/agents/service-delivery-analyst/charter.md` | Active DIT specialist |
| Evidence & Audit Specialist | Evidence quality, traceability, and audit readiness | `.squad/agents/evidence-audit-specialist/charter.md` | Active DIT specialist |
| Technical Operations Challenger | Operational challenge, assumptions, and risk surfacing | `.squad/agents/technical-operations-challenger/charter.md` | Active DIT specialist |
| Data & Automation Engineer | Data and automation work within approved scope | `.squad/agents/data-automation-engineer/charter.md` | Active DIT specialist |
| Quality Reviewer & Scribe | Independent quality review and focused work notes | `.squad/agents/quality-reviewer-scribe/charter.md` | Active DIT specialist |

## Built-in Squad Support (not DIT roles)

These four standard identities are framework support roles, not additional DIT
specialists and not domain-routing destinations. Their existing canonical charters
remain in place.

| Name | Role | Charter | Status |
|------|------|---------|--------|
| Scribe | Durable decision curator | `.squad/agents/scribe/charter.md` | Built-in support; not a DIT role |
| Ralph | Work monitor | `.squad/agents/ralph/charter.md` | Built-in support; not a DIT role |
| Rai | Responsible AI reviewer | `.squad/agents/Rai/charter.md` | Built-in support; not a DIT role |
| Fact Checker | Verification and devil's advocate | `.squad/agents/fact-checker/charter.md` | Built-in support; not a DIT role |

The DIT specialist named **Quality Reviewer & Scribe** is distinct from the fixed
Squad support identity **Scribe**. The DIT specialist reviews work quality and
captures bounded work notes; the built-in Scribe alone curates canonical durable
decisions.

## Optional Coding Agent

<!-- copilot-auto-assign: false -->

| Name | Role | Charter | Status |
|------|------|---------|--------|
| @copilot | Coding Agent | — | Optional platform agent; not one of the seven DIT roles or four built-in support identities |

@copilot is not enabled for automatic assignment by this setup.

### Mogelijkheden (bestaande standaardinformatie)

**🟢 Geschikt bij expliciete toewijzing:**
- Bugfixes met duidelijke reproductiestappen
- Tests toevoegen of flaky tests repareren
- Lint-/formatteer- en stijlcorrecties
- Dependency-updates en versie-bumps
- Kleine, geïsoleerde functies met duidelijke specificatie
- Boilerplate/scaffolding en documentatiefixes

**🟡 Alleen met review:**
- Middelgrote functies met duidelijke acceptatiecriteria
- Refactors met bestaande testdekking
- API-uitbreidingen volgens bestaand patroon
- Migraties met een vastgelegd schema

**🔴 Niet automatisch toewijzen:**
- Architectuur- of systeemontwerp
- Integratie van meerdere systemen
- Ambigue eisen, security-kritische of performance-kritische wijzigingen
- Werk dat afstemming tussen teams vereist

## Projectcontext

- **Project:** SQUAD
- **Created:** 2026-11-02
- **Identiteit aanvrager:** `git config user.name` was leeg tijdens inrichting; er is geen naam of e-mailadres afgeleid of vastgelegd.
- **Bekende scope:** Inrichting van het goedgekeurde DIT-team met zeven rollen, verantwoordelijkheden, samenwerking en routing.
- **Onbekende context:** Er is geen DIT-uitbreiding, organisatiestructuur, cloudprovider, bedrijfssysteem, tool of broninventaris opgegeven; neem niets daarvan aan.
- **Uitsluitingen fase 1:** Inventariseer geen kennisbronnen of tools en wijzig geen bedrijfssystemen.
- **Vastgelegde teamkennis:** De rolgrenzen en scopebeperkingen staan in `.squad/decisions.md` en de `history.md`-bestanden van de specialisten.
