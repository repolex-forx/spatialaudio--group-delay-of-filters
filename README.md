# Repolex Knowledge Graph of spatialaudio/group-delay-of-filters

RDF knowledge graph data for [spatialaudio/group-delay-of-filters](https://github.com/spatialaudio/group-delay-of-filters), parsed by [repolex](https://repolex.ai).

> **Note**: This data is experimental and subject to change without notice.

## How to use this data

The easiest way to get started is to install the [rlex](https://github.com/repolex-ai/rlex) query tool:

```bash
cargo install --git https://github.com/repolex-ai/rlex
```

Verify the install:

```bash
rlex --help
```

**rlex is designed to be used primarily by LLMs in a terminal.** Start up your favorite AI assistant and ask it to use rlex. It handles the SPARQL — you just ask questions in plain English.

To load this repo's data:

```bash
rlex download spatialaudio/group-delay-of-filters
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── 59fc4858d4ad6b80395ba47c162fc512117f46b6
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── 59fc4858d4ad6b80395ba47c162fc512117f46b6
│           └── chunk-001.nq.gz
├── blob
│   ├── 049a940cfeb940deac6cec166e90a768d53d53e4.nq.gz
│   ├── 24241b9e959bf13cb755eee314d4e62f3bea7eed.nq.gz
│   ├── 6f45667cb22486a670f6c8b54030bad77254ed39.nq.gz
│   ├── 8aa5672bde759c7917793d63f8a9a6dc191dbf35.nq.gz
│   ├── 8ed4052a48b73805c0a4260e330b8e26597f5197.nq.gz
│   ├── 9088e0852798ea71c7edb9e8003c68fb2bfde4a6.nq.gz
│   ├── 99b19b1d7bea31465b1d5829681bc14b4df02800.nq.gz
│   └── dba5aa4af4142f6e7ebcea8335ccaa0fe4e8ff93.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── 59fc4858d4ad6b80395ba47c162fc512117f46b6.nq.gz
└── tag
    └── tag.nq.gz

11 directories, 14 files
```

| Directory | What it contains |
|-----------|-----------------|
| `blob/` | Per-file AST graphs, content-addressed by git blob SHA. Each file in the source repo gets its own graph. |
| `aggregate/ast/` | Combined AST graph per parsed commit. Merges all blob graphs for a snapshot of the entire codebase at that point. |
| `aggregate/lsp/` | Language Server Protocol enrichment: resolved symbols, definitions, references, and type information. |
| `aggregate/dataflow/` | Interprocedural data flow edges between functions and modules. |
| `aggregate/repolex/` | Combined graph (AST + LSP + dataflow) per commit. |
| `commit/` | Git commit metadata (author, date, message, parent links). |
| `branch/` | Branch metadata. |
| `tag/` | Tag metadata. |
| `filetree/` | File tree snapshots per commit (which files existed and their blob SHAs). |
| `audit/` | Code architecture and graph audit reports per commit. |

## Source repository

[spatialaudio/group-delay-of-filters](https://github.com/spatialaudio/group-delay-of-filters)

---
*Parsed on 2026-10-28 by [repolex](https://repolex.ai)*
