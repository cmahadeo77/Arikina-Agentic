# Arikina Agentic Commerce

**Agentic infrastructure for B2B ingredient sourcing — built in production at Arikina.**

---

## Thesis

The B2B workflows that define most industries today — supplier discovery, document validation, procurement, cross-border payment — were designed for humans operating at human speed, with human error rates, over human communication channels. AI agents don't just accelerate those workflows. They eliminate the distinction between intelligence and execution.

The naturals ingredient supply chain is one of the most cert-dense, traceability-required verticals in B2B commerce. Every transaction requires multi-document validation (COA, MSDS, origin certs, INCI compliance), spec alignment, and regulatory review. That complexity is exactly why agents generate disproportionate value here — and why this is the right beachhead.

---

## The Stack

```
Supplier Discovery → COA Validation → Formula Generation → PO Automation → Stablecoin Settlement
```

Each stage is an agent. The agents compose into a full commercial workflow with no human in the loop except at exception points.

---

## Modules

| Module | Description | Status |
|--------|-------------|--------|
| `discovery/` | Multi-source supplier discovery agent — Brave Search, directory scraping, cert filtering | Active |
| `coa-validation/` | Claude Vision COA parser — extracts specs, validates against PO requirements, emits PASS/FAIL | Active |
| `formulation/` | INCI formula generator with live market context injection via Open Beauty Facts + Google Trends | Active |
| `payments/` | USDC escrow smart contract for cross-border supplier payments — funds release on COA PASS | Active |
| `orchestrator/` | Top-level orchestration agent — routes tasks, manages state across sub-agents | In progress |

---

## Why Ingredients

Every B2B vertical that requires document-gated, compliance-aware procurement has the same underlying structure. The naturals supply chain is where this thesis is being stress-tested — in production, at real commercial scale.

The companies that win in agentic B2B commerce will not win because they deployed agents first. They will win because each agent interaction generates structured operational data — supplier reliability scores, COA pass/fail patterns, pricing signals, certification expiry cycles — that makes the next interaction smarter. The moat is not the agents. It is the data they accumulate.

---

## Stack

- **AI**: Claude API (claude-opus-4-7), adaptive thinking, multi-agent orchestration
- **Search**: Brave Search API
- **Document parsing**: PyMuPDF, Claude Vision
- **Payments**: USDC / Circle API, Stellar, Solidity
- **Runtime**: Node.js, Python
- **Data**: Open Beauty Facts, Google Trends API

---

## Contact

Chris Mahadeo — [arikina.com](https://www.arikina.com) · [chris@arikina.com](mailto:chris@arikina.com)
