# Graph Report - nuevo-chat-de-voz-en-tiempo-3  (2026-09-08)

## Corpus Check
- 3 files · ~31,794 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 22 nodes · 24 edges · 4 communities (3 shown, 1 thin omitted)
- Extraction: 100% EXTRACTED · 0% INFERRED · 0% AMBIGUOUS
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `f9dba5f6`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- app-v2.js
- app.js
- Moneda al Aire
- flip

## God Nodes (most connected - your core abstractions)
1. `flip()` - 4 edges
2. `flip()` - 3 edges
3. `tone()` - 2 edges
4. `metalClink()` - 2 edges
5. `render()` - 2 edges
6. `tone()` - 2 edges
7. `render()` - 2 edges
8. `Moneda al Aire` - 2 edges
9. `coin` - 1 edges
10. `rig` - 1 edges

## Surprising Connections (you probably didn't know these)
- None detected - all connections are within the same source files.

## Import Cycles
- None detected.

## Communities (4 total, 1 thin omitted)

### Community 0 - "app-v2.js"
Cohesion: 0.29
Nodes (6): coin, flipBtn, result, rig, shadow, stats

### Community 1 - "app.js"
Cohesion: 0.32
Nodes (7): coin, flip(), flipBtn, render(), result, stats, tone()

### Community 3 - "flip"
Cohesion: 0.50
Nodes (4): flip(), metalClink(), render(), tone()

## Knowledge Gaps
- **11 isolated node(s):** `coin`, `rig`, `shadow`, `flipBtn`, `result` (+6 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **1 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `flip()` connect `flip` to `app-v2.js`?**
  _High betweenness centrality (0.007) - this node is a cross-community bridge._
- **What connects `coin`, `rig`, `shadow` to the rest of the system?**
  _11 weakly-connected nodes found - possible documentation gaps or missing edges._