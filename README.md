# KinCart — governance (research)

This repository documents KinCart’s **research governance**: how decisions become truth, how constraints prevent drift, and how emotionally safe coordination remains protected under failure.

**Start here:** `START_HERE.md`

KinCart is a **non-commercial research artefact**. This is not a product backlog or delivery tracker. External participation is limited to peer review / collaborative learning with **no milestones, deadlines, output expectations, or IP transfer**.

## What this repo is responsible for
- Defining **what is committed** vs what is merely suggested (decision register + decision records)
- Defining **action gates** (what must be true before changes are accepted)
- Preventing access-control drift: **Auth → RLS → RPC** must remain consistent
- Keeping public documentation **implementation-light** (principles and failure modes, not recipes)

## Where “product truth” lives
- **Blueprint repo (public):** frozen product definition, domain language, invariants, and public-safe appendices  
  *(This repo points to it; it does not duplicate it.)*
- **Implementation repo (private):** code, migrations, and any executable enforcement

## How to use this repo
1. Check the decision register to see what is committed.
2. If you want to change something, add/extend a decision record first.
3. Only then update blueprint artefacts and link back to the governing decision.

## Public-safe rule
This repository may describe invariants and failure modes, but should avoid “copy/paste build recipes” that enable cloning.
