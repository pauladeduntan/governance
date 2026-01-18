# Start Here (KinCart Governance)

This repository defines how KinCart research decisions become binding truth and how drift is prevented, unless explicitly superseded by a later decision.

## If You only Read 3 Things

1) Decision Register (What Is Committed): ./decision-register.md  
2) Decision Records (Why It Was Committed): ./decisions/  
3) Action Gates (What Must Be True Before Changes): ./action-gates/

## Related Blueprint (What Is Being Governed)

Blueprint Repository: https://github.com/pauladeduntan/blueprint

Key Blueprint Constraints:

- Domain Language (Locked): https://github.com/pauladeduntan/blueprint/blob/main/domain-language.md
- Invariants (Locked): https://github.com/pauladeduntan/blueprint/blob/main/invariants.md
- Product Definition: https://github.com/pauladeduntan/blueprint/blob/main/product-definition.md
- System Flows: https://github.com/pauladeduntan/blueprint/blob/main/system-flows.md
- Cross-Repo Map (Blueprint Appendix): https://github.com/pauladeduntan/blueprint/blob/main/appendix/governance-links.md

## Why Governance Exists

KinCart has explicit non-negotiables (emotional safety over optimisation, visibility over reminders) and known drift surfaces. Governance exists to prevent accidental introduction of enforcement cues, surveillance interpretations, or identity exposure.

Activity is treated as a high-risk drift surface and is governed explicitly to prevent performance-feed interpretations and to preserve exit safety defaults.

## Public-Safety Boundary

This repository documents principles, constraints, and failure-aware governance.

Implementation mechanics and build steps are intentionally not published. Public artefacts must also avoid roadmap and delivery language and must not become copy-and-paste build recipes.
