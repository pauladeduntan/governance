# KinCart - Governance (Research)

This repository documents KinCart’s research governance: how decisions become truth, how constraints prevent drift, and how emotionally safe coordination remains protected under breakdown and repair.

Start here: [START_HERE.md](https://github.com/pauladeduntan/governance/blob/main/START_HERE.md)

KinCart is a non-commercial research artefact. This is not a product backlog or delivery tracker. External participation is limited to peer review and collaborative learning, with no milestones, deadlines, output expectations, or IP transfer.

## What This Repository Is Responsible For

- Defining what is committed versus what is merely suggested (Decision Register and Decision Records).
- Defining action gates (what must be true before changes are accepted).
- Preventing access-control drift at the principle level: access boundaries must remain consistent with membership, boundary integrity, and exit safety.
- Governing known drift surfaces, especially Activity (prevent performance-feed interpretation, prevent identity exposure after exit, and enforce anti-amplification constraints).
- Keeping public documentation implementation-light (principles and failure modes, not recipes).

## Where Artefact Truth Lives

- Blueprint Repository (Public): locked product definition, domain language, invariants, and public-safe appendices. This repository points to it and does not duplicate it.
- Implementation Materials (Not Published Here): any schemas, RLS, RPCs, operational scripts, deploy steps, or build instructions are intentionally excluded from public repositories.

## How To Use This Repository

1) Check the Decision Register to see what is committed.
2) If you want to change something, add or extend a Decision Record first.
3) Only then update the Blueprint artefacts and link back to the governing decision.

## Public-Safe Rule

This repository may describe invariants and failure modes, but must avoid copy-and-paste build recipes that enable cloning. Public artefacts must also avoid roadmap and delivery language (for example, MVP, post-MVP, rollout, scaling).
