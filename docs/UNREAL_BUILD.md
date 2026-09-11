# SOVEREIGN CONSEQUENCE — Unreal Production Build

## Foundation
Narrative Pro 2 + Ultra Game Template 1.3 for shell/narrative/meta systems after ownership reconciliation.

## Fab
RTS/RPG Unit Template as unit/command prototype; Squad & Team Combat AI for tactical coordination; OverCrowd for visual crowds; Building System Multiplayer for construction; environments/maps as prototyping content. HKH Attribute System only if chosen as sole unit-stat implementation.

## Architecture
Strategic simulation is data-oriented and decoupled from rendered actors. Aggregate population/economy/diplomacy runs at appropriate simulation ticks. Tactical battles instantiate only relevant entities. Save games store canonical strategic state, not transient visual actors.

## AI
Strategic AI has goals, beliefs/knowledge constraints, resource budgets and explainable decision traces for debugging. Tactical AI uses squad objectives/formation/cover/target policies. No LLM call is required in realtime simulation.

## Testing
Deterministic/seeded scenario tests, economy conservation/invariants, AI soak, large-unit performance, crowd LOD, multiplayer authority if enabled, save migration and scenario-editor validation.
