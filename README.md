# Repolex Knowledge Graph of asimov-modules/asimov-telegram-module

RDF knowledge graph data for [asimov-modules/asimov-telegram-module](https://github.com/asimov-modules/asimov-telegram-module), parsed by [repolex](https://repolex.ai).

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
rlex download asimov-modules/asimov-telegram-module
```

Consult `rlex --help` for other options, including SPARQL queries, HTTP server, and interactive visualization.

## Data structure

All data is stored as gzip-compressed [N-Quads](https://www.w3.org/TR/n-quads/) (`.nq.gz`), a standard RDF format that can be loaded into any triplestore or graph database.

```
.
├── aggregate
│   ├── ast
│   │   └── a8e8d662fd4faca68d0f5b7a27186d5445ae535a
│   │       └── chunk-001.nq.gz
│   ├── lsp
│   │   └── a8e8d662fd4faca68d0f5b7a27186d5445ae535a.nq.gz
│   └── repolex
│       └── a8e8d662fd4faca68d0f5b7a27186d5445ae535a
│           └── chunk-001.nq.gz
├── blob
│   ├── 2010ffe2bd517131a8f610125a69425d2c4491e2.nq.gz
│   ├── 2391f73aa051d3804285ce744f2e9a1c7e08993d.nq.gz
│   ├── 2fa3bbf1fe5f7be3f38806f19c9b23c7ce10a6de.nq.gz
│   ├── 4115f586ac0fffeb0b8eeb638de8ee6c790755cb.nq.gz
│   ├── 50ac667f7af2c0bc6b400c19fa1ec62ed076dbb0.nq.gz
│   ├── 50ce4ffc99f4f3aca9546b45c5293cacde15f7f2.nq.gz
│   ├── 5dc50bcc4043313cb30c4702b021d658692f3cd0.nq.gz
│   ├── 5f5cf896c81688e4360b37f1bcda92f7bc6f7423.nq.gz
│   ├── 63fdd52957d7418fe0a5515ee337523dd07c5de4.nq.gz
│   ├── 752679f4ac7394215f21b3f587789e002a0fd4f3.nq.gz
│   ├── 75e3b65f99b29f48ab230e3eab3de8d0b7a9229f.nq.gz
│   ├── 7f60b03d440f5e965d54f58e4e8e68fbf0abc09b.nq.gz
│   ├── 88ede0b6c3d0ee68688940cb6f575e3728652a9e.nq.gz
│   ├── 90fe8c9cd2c6b23f6d7e4cf013fddea00f77197a.nq.gz
│   ├── 9c558e357c41674e39880abb6c3209e539de42e2.nq.gz
│   ├── af9908b08f4b33c32a0080af73f53bc0fa0cdce4.nq.gz
│   ├── bcab45af15a0f1b0166daf8cbf18b17cd8649277.nq.gz
│   ├── bccde52db3f3259f931a8fea887222d5e64fab0b.nq.gz
│   ├── cc8ba103fcc456c60baced7776eadbbfcd47fbe2.nq.gz
│   ├── cf42f6893594e2f8be2b722de51123d65e4d61c4.nq.gz
│   ├── dc75511c29cbba83faa4539565efc4cdd0e66702.nq.gz
│   ├── e3e57a8ce4ccbf74759a6df8fa4a3980ff1c9209.nq.gz
│   ├── efb98088164f5786b17e83ed384971fc3c74f93c.nq.gz
│   ├── f06390fe06caa951ead481b062cb7a10769d4815.nq.gz
│   └── f8268bbea008c201341f5e4b02249abae8de2242.nq.gz
├── branch
│   └── branch.nq.gz
├── commit
│   └── commit.nq.gz
├── dep
│   └── a8e8d662fd4faca68d0f5b7a27186d5445ae535a.nq.gz
├── filetree
│   └── a8e8d662fd4faca68d0f5b7a27186d5445ae535a.nq.gz
├── pr
│   └── pr.nq.gz
└── tag
    └── tag.nq.gz

14 directories, 34 files
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

[asimov-modules/asimov-telegram-module](https://github.com/asimov-modules/asimov-telegram-module)

---
*Parsed on 2026-09-28 by [repolex](https://repolex.ai)*
