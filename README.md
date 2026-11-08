# Repolex Knowledge Graph of google-deepmind/fusion_surrogates

RDF knowledge graph data for [google-deepmind/fusion_surrogates](https://github.com/google-deepmind/fusion_surrogates), parsed by [repolex](https://repolex.ai).

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
rlex download google-deepmind/fusion_surrogates
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── f92669684436699b5350d997bca553624505c2d6
│   │       └── chunk-001.nq.gz
│   └── repolex
│       └── f92669684436699b5350d997bca553624505c2d6
│           └── chunk-001.nq.gz
├── blob
│   ├── 005f955e283ade465116862563c91a3118efdfce.nq.gz
│   ├── 08b9b90f824875a6f3009a0e0e17ceaa744afaf6.nq.gz
│   ├── 08f1f26e40b23140259e055f53cbf0b0cb4071b2.nq.gz
│   ├── 11eb7cf62185e2811623f1a2434dc35ba66b658a.nq.gz
│   ├── 28bdffb07b61b172fdcf0fd98aeaeac9fa99c823.nq.gz
│   ├── 48155ba68d7210198a8bbccd690436bf49f5c1b1.nq.gz
│   ├── 50c4f06e89cfe5b2bd7524fd59540d65288bafe9.nq.gz
│   ├── 59e04a138ceadcc5b16c2d783dcd5bc060832229.nq.gz
│   ├── 6dcf239cb6cd19d3789da3157db72d2eb4c987cb.nq.gz
│   ├── 6f0577da442631d76ba62552e2b778ee781d7eb6.nq.gz
│   ├── 934f78b74d31309257c49a8a9dc414053666c342.nq.gz
│   ├── 9b2b37916f87c7d0aee473165599089161f84842.nq.gz
│   ├── 9ba6022ced01cdc4ef70f28924c65297883ea644.nq.gz
│   ├── 9c29c4e5862d084428c43485ab9c5c27fd230861.nq.gz
│   ├── a5bfe19b4b6d88b929a432b62cfd04fa970fa912.nq.gz
│   ├── aa90c4329e129ac4d3e5f6ebc9d719852dd2c482.nq.gz
│   ├── ab326c91e0124c5365a5b8f2307c11a575300462.nq.gz
│   ├── b1326878dcccaa0b33ff030172676644b9dcaa14.nq.gz
│   ├── c07d11b63df035b551543e3ae81e1ba3c39aa4fb.nq.gz
│   ├── c1466849528efdaada5077e9ecd0de88865b91ab.nq.gz
│   ├── cdf4ce1f38472fdbf495bf5588d7514794512a05.nq.gz
│   ├── d0368388d03d7338f7dbcc734c25311aafd31463.nq.gz
│   ├── d2b95ee1a137ca6277b5f25100c3c7d81df4612d.nq.gz
│   ├── d645695673349e3947e8e5ae42332d0ac3164cd7.nq.gz
│   ├── db5092e656585e5ac5513fc91004a8a11b239a3e.nq.gz
│   ├── e2f0c59e04fab03da077d78661e6f6649c40334e.nq.gz
│   ├── e85d9451a8b06aef26eecd751141c6737e1ae2f9.nq.gz
│   ├── f64f021942f4030aa16bc9d3ff5b66aff30096fc.nq.gz
│   └── ff375f6b2930cbd4505a2e761eb1a8bbc8aed598.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── filetree
│   └── f92669684436699b5350d997bca553624505c2d6.nq.gz
├── issue
│   └── issue.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

13 directories, 37 files
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

[google-deepmind/fusion_surrogates](https://github.com/google-deepmind/fusion_surrogates)

---
*Parsed on 2026-11-08 by [repolex](https://repolex.ai)*
