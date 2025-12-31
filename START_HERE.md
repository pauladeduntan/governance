# Start here (KinCart governance)

This repository defines how KinCart research decisions become **binding truth** and how drift is prevented.

## If you only read 3 things
1) Decision register (what is committed): ./decision-register.md  
2) Decision records (why it was committed): ./decisions/  
3) Action gates (what must be true before changes): ./action-gates/

## Related blueprint (what is being governed)
Blueprint repo: https://github.com/pauladeduntan/blueprint

Key blueprint constraints:
- Domain language (LOCKED): https://github.com/pauladeduntan/blueprint/blob/main/domain-language.md
- Invariants (LOCKED): https://github.com/pauladeduntan/blueprint/blob/main/invariants.md
- Product definition: https://github.com/pauladeduntan/blueprint/blob/main/product-definition.md
- System flows: https://github.com/pauladeduntan/blueprint/blob/main/system-flows.md
- Cross-repo map (blueprint appendix): https://github.com/pauladeduntan/blueprint/blob/main/appendix/governance-links.md

## Public-safety boundary
This repo documents principles, constraints, and failure-aware governance.
Implementation mechanics (schema/RLS/RPC specifics, deploy steps) are intentionally not published.
