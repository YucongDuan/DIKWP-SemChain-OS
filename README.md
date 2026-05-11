# DIKWP SemChain OS

**DIKWP SemChain OS** is an open-source semantic blockchain layer for AI trust, evidence custody, semantic provenance, and cross-industry auditability.

It is not a cryptocurrency, token system, or public-chain speculation tool. It is a local-first, permissioned, tamper-evident semantic ledger that turns AI outputs, RAG claims, agent actions, hardware command proposals, compliance assertions, educational records, legal evidence, and health-navigation records into DIKWP semantic blocks.

Each semantic block contains:

- `D`: data / source / observation
- `I`: information / relation / context
- `K`: knowledge / mechanism / rule
- `W`: wisdom / risk / value boundary
- `P`: purpose / intent contract
- `R`: reliability / proof / residual / kill condition

The system produces a hash-chain ledger, Merkle anchor, DIKWP block cards, W3C-VC-like semantic credentials, and verification reports.

## Why it matters

AI systems increasingly produce claims, tool calls, recommendations, and decisions across organizations. Ordinary logs record events, but they do not preserve semantic accountability. DIKWP SemChain OS records not only **what happened**, but **what claim was made, what evidence supported it, what purpose it served, what risks existed, and what would kill or downgrade the claim**.

## Quickstart

```bash
pip install -e .
semchain build-demo --claims examples/sample_semantic_claims.json --out outputs/demo
semchain verify outputs/demo/semantic_chain_ledger.jsonl
semchain static-audit src --out outputs/demo/static_boundary_audit_report.json
```

Optional local UI:

```bash
pip install -e .[app]
streamlit run src/dikwp_semchain/app.py
```

## Governance boundary

This project does not provide financial instruments, anonymous token issuance, sanctions evasion, privacy bypass, credential forgery, or enforcement automation. It creates a verifiable semantic evidence layer for human-reviewed AI collaboration.
