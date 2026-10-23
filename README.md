# graphify knowledge graph

A [graphify](https://github.com/safishamsi/graphify) graph of this repo's code, docs and reports, built from `main` at ``. This branch holds only the graph; it shares no history with `main`.

To use it in a clone of the repo:

```bash
git fetch origin graphify
git checkout origin/graphify -- graphify-out
graphify query "your question"
```

`graphify-out/graph.html` is the interactive view and `graphify-out/GRAPH_REPORT.md` the summary.
