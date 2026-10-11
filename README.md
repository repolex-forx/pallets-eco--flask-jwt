# Repolex Knowledge Graph of pallets-eco/flask-jwt

RDF knowledge graph data for [pallets-eco/flask-jwt](https://github.com/pallets-eco/flask-jwt), parsed by [repolex](https://repolex.ai).

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
rlex download pallets-eco/flask-jwt
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── c27084114e258863b82753fc574a362cd6c62fcd
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── c27084114e258863b82753fc574a362cd6c62fcd
│           └── chunk-001.nq.gz
├── blob
│   ├── 17b8937aa633874f7bb2eb3b3419e9fb9285c831.nq.gz
│   ├── 2157003210165ccee6849f7672742f86bf1fa818.nq.gz
│   ├── 31e658d208288c4d4d2321fd8820c38ef7c7497b.nq.gz
│   ├── 34526d7cc779e29f988342250bbd39fd8bbea351.nq.gz
│   ├── 3fc9dc7b608c0e394b216a5213bb1307d4f61646.nq.gz
│   ├── 5e6279fe2636fbb2c0d68a3c84a71be7f949ed2d.nq.gz
│   ├── 62d10c3d74e57d41cae2a5899d8ae957c6e80d80.nq.gz
│   ├── 673f940c28375e9ae36a829e3ff56d17cda2b6aa.nq.gz
│   ├── 78ed6c5a32f09972bc9b9e3900f8234a012f07ac.nq.gz
│   ├── 8a05a51e8698babbed33230457f17c9073042d81.nq.gz
│   ├── 8aeca3f5562008b655d6e07b9c3a509e5d856960.nq.gz
│   ├── 953d69ba2e925a6a31adb4eb1fb3d1c280233bb4.nq.gz
│   ├── 96eb605f5e85704ad41dc61b213a1626bba0c140.nq.gz
│   ├── b0c8e3752599a9bd5b12220d7c8c645e39970710.nq.gz
│   ├── ba7553f1023507a3104acce3d296b2888b7275d0.nq.gz
│   ├── bf7b494fc7044e1395c1c821f2babc309277bf78.nq.gz
│   ├── bf9d492d1c1024c862efaa8febb1fe24ae8fcee6.nq.gz
│   ├── d80b931db53cb64b6fef27981eed218c3780ed3e.nq.gz
│   ├── da4c30d424a1cf7774dbe2c38334322113df1b10.nq.gz
│   ├── e908d1704dbca4c3e34c0f73331876256528ec67.nq.gz
│   ├── e9fda0a6e1c44bbbcb2064636b680e36d98a6e01.nq.gz
│   ├── f8446aeaa4b518378f0e34ecf85c3ceb7c248b70.nq.gz
│   ├── f864b788f318ea618925ef504d1957e35486b91e.nq.gz
│   └── fb87ce4185ccd7efcbb2a9b7cc5409ac4f20d76f.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── c27084114e258863b82753fc574a362cd6c62fcd.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 32 files
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

[pallets-eco/flask-jwt](https://github.com/pallets-eco/flask-jwt)

---
*Parsed on 2026-10-11 by [repolex](https://repolex.ai)*
