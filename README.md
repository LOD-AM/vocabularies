> [!IMPORTANT]
> **This repository has moved to [LOD-AM/knowledge-graph](https://github.com/LOD-AM/knowledge-graph).**
> It is archived and no longer updated. Its full history was merged into
> knowledge-graph in November 2026, together with `ontologies`, `vocabularies`
> and `converter`. Please use, link and cite the new repository.

## Where things are now

| Here (old) | In knowledge-graph (current) |
|---|---|
| `DECISIONS.md` | [`docs/decisions/vocabularies.md`](https://github.com/LOD-AM/knowledge-graph/blob/main/docs/decisions/vocabularies.md) |
| `vocabularies/getty-aat/`, `periodO/`, `pleiades/` | [`vocabularies/`](https://github.com/LOD-AM/knowledge-graph/tree/main/vocabularies) |
| `vocabularies/allotrope/`, `vocabularies/fabio/` | [`ontologies/`](https://github.com/LOD-AM/knowledge-graph/tree/main/ontologies) (Allotrope and FaBiO are documented as ontologies now) |

The old files below are kept as they were, so links from older blog posts on
[lod-am.net](https://lod-am.net) still work. They **don't** reflect the current model:
several terms used here were corrected (see
[knowledge-graph#10](https://github.com/LOD-AM/knowledge-graph/pull/10)). The current rules are in
[CONVENTIONS.md](https://github.com/LOD-AM/knowledge-graph/blob/main/CONVENTIONS.md).

---

# LOD-AM/vocabularies

**Controlled vocabulary information for the Linked Open Data for Ancient Metallurgy (LOD-AM) project.**

## Purpose

This repository stores **only vocabulary-related information** for LOD-AM:
- Which controlled vocabularies we use
- Why we chose them
- How we use them
- Reference URIs and namespaces

## Structure

```
vocabularies/
├── README.md                      # This file
├── DECISIONS.md                   # Vocabulary choice rationale
├── LICENSE                        # License information
└── vocabularies/
    ├── pleiades/
    │   ├── README.md              # Usage notes
    │   └── reference.txt          # Official URI
    ├── periodO/
    │   ├── README.md
    │   └── reference.txt
    ├── getty-aat/
    │   ├── README.md
    │   └── reference.txt
    ├── allotrope/
    │   ├── README.md
    │   └── reference.txt
    └── fabio/
        ├── README.md
        └── reference.txt
```

## Quick Start

1. Read DECISIONS.md for the rationale behind our vocabulary choices
2. Browse vocabularies/ for per-vocabulary usage notes
3. Check vocabularies/*/reference.txt for official URIs and namespaces

## Maintenance Rules

1. **No vocabulary files**: Do not commit external vocabulary TTLs/RDF. Only store references and documentation.
2. **One decisions document**: Keep all rationale in DECISIONS.md.
3. **Minimal examples**: Only include example snippets that demonstrate actual usage patterns.
4. **Decisions first**: Update DECISIONS.md before changing vocabulary usage.

## Current Vocabularies

- **Sites and Site Types**: [Pleiades](https://pleiades.stoa.org/)
- **Cultures and Periods**: [PeriodO](https://perio.do/en/)
- **Feature/Object Types**: [Getty AAT](https://www.getty.edu/research/tools/vocabularies/aat/)
- **Scientific Analytics**: [Allotrope Framework](https://www.allotrope.org/)
- **Literature**: [FABIO](http://purl.org/spar/fabio/)
