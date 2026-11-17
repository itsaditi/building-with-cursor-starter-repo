---
name: edge-case-audit
description: Use when auditing domain logic for production edge cases, race conditions, and failure modes.
---
Review the target domain service and check for:
1. Invalid state transitions (e.g., duplicate state updates, out-of-order events).
2. Idempotency gaps on mutating operations.
3. Boundary conditions (empty lists, zero/negative values, missing IDs).
4. Concurrency hazards (double-assigning a courier or inventory item).
Report only high-impact findings with concrete fixes.