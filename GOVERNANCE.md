# Repository Governance

## Authority
Human approval remains the highest authority. This repository may inform or implement governed actions but cannot self-authorize actions above its authority ceiling.

## Change classes
- **EXECUTE:** validated, authorized, reversible or appropriately controlled
- **HOLD:** insufficient evidence or uncertainty
- **ESCALATE:** ambiguity, elevated risk, destructive/access/policy impact
- **DEFER:** intentionally postponed
- **SIMULATE:** non-production evaluation

## Evidence
Every production claim should identify:
1. source
2. timestamp
3. result
4. artifact/hash where applicable
5. recovery or rollback path
