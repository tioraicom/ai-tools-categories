# AI Tools Categories

**English** · [العربية](README.ar.md)

> A two-level taxonomy of AI tool categories with stable slugs, parents, aliases, and
> descriptions, ready to drop into a directory or a dataset.

<!-- counts:start -->
![Categories](https://img.shields.io/badge/categories-182-informational)
<!-- counts:end -->
![Contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen)
[![License: CC BY 4.0](https://img.shields.io/badge/license-CC%20BY%204.0-lightgrey)](LICENSE)

20 top-level categories and 162 subcategories, as JSON and CSV. Every node has a stable
slug, a parent, a one-line description, and the other names it commonly goes by. It is the
part of a directory nobody wants to design from scratch and everybody ends up designing
badly.

The top level is deliberately the same twenty categories used by the TiorAI AI tools dataset,
so the two fit together: adopt the top level alone and stay compatible with published data, or
adopt both levels and get the detail. A competing second top level would have made two TiorAI
repositories disagree with each other in public.

Maintained by [TiorAI](https://tiorai.com/), which catalogues AI tools for a living.

<!-- last-reviewed:start -->
**Last reviewed:** 2026-09-04
<!-- last-reviewed:end -->

## Contents

- [What's in the dataset](#whats-in-the-dataset)
- [Schema](#schema)
- [How categories are selected](#how-categories-are-selected)
- [Using the data](#using-the-data)
- [Known limitations](#known-limitations)
- [Suggest a category](#suggest-a-category)
- [Contributing](#contributing)
- [Disclaimer](#disclaimer)
- [License](#license)
- [About TiorAI](#about-tiorai)

## What's in the dataset

```text
data/
├── categories.json        all 182 nodes, typed, with parents and children
├── categories-flat.csv    the same 182 nodes, one row each
├── categories.csv         the 20 top-level categories with a subcategory count
└── schema.json            JSON Schema for categories.json
```

### The top level

| Category | Slug | Subcategories |
|---|---|---:|
| Writing and content | `writing-and-content` | 9 |
| Image generation and editing | `image-generation-and-editing` | 8 |
| Video | `video` | 8 |
| Audio, music, and voice | `audio-music-and-voice` | 9 |
| Coding and development | `coding-and-development` | 12 |
| Developer infrastructure and models | `developer-infrastructure-and-models` | 12 |
| Chatbots and assistants | `chatbots-and-assistants` | 7 |
| Automation and agents | `automation-and-agents` | 7 |
| Productivity and workflow | `productivity-and-workflow` | 8 |
| Presentations and documents | `presentations-and-documents` | 6 |
| Design and creative | `design-and-creative` | 7 |
| Marketing and advertising | `marketing-and-advertising` | 10 |
| SEO and search | `seo-and-search` | 10 |
| Sales and CRM | `sales-and-crm` | 7 |
| Customer support | `customer-support` | 6 |
| Data and analytics | `data-and-analytics` | 7 |
| Research and knowledge | `research-and-knowledge` | 8 |
| Education and learning | `education-and-learning` | 7 |
| Business and finance | `business-and-finance` | 8 |
| Health and lifestyle | `health-and-lifestyle` | 6 |

The full tree is in the data files. It is not reproduced here, because a README that lists
182 rows is a data file with worse formatting.

## Schema

One record per category, at either level. The machine-readable version is
[`data/schema.json`](data/schema.json).

| Field | Type | Notes |
|---|---|---|
| `name` | string | Display name, sentence case |
| `slug` | string | Stable identifier, unique across both levels. Derived from the name, but it does not change when the name does |
| `parent` | string or null | Slug of the level-1 parent. `null` at level 1 |
| `level` | integer | `1` or `2`. There is no level 3, on purpose |
| `description` | string | One sentence, 5 to 22 words |
| `aliases` | array of strings | Other names for the same category, including American spellings and common abbreviations |
| `children` | array of strings | Slugs of the level-2 children. Empty at level 2 |
| `last_reviewed` | string | ISO `YYYY-MM-DD` |

The tree is checked before release: every `parent` resolves, every `children` entry
resolves, no name appears twice anywhere in the tree, and no level-2 node has children of
its own.

## How categories are selected

A category earns a place when it answers a question a person actually arrives with. "Text to
image" is a category because people search for it. "Generative visual synthesis" is not,
because nobody does.

The rules the tree is built to:

- **Two levels, never three.** A third level is where taxonomies go to die: it produces
  nodes with one member, and it forces a judgement call on every new tool.
- **Six to twelve children per top-level category.** Below six, the level is not carrying its
  weight and the children belong one level up. Above twelve, the category is really two.
- **Named by the job, not the technology.** `Meeting assistants`, not `Multimodal
  transcription and summarisation`.
- **Aliases carry the variants.** `personalization`, `tts`, `cro`, and `localization` are
  aliases rather than separate nodes, so a lookup succeeds whichever a user types.
- **No vendor-specific nodes.** A category named after one product is a product page.

What is deliberately absent: a third level, categories that exist only as a marketing
phrase, industry verticals (a taxonomy of tools is not a taxonomy of customers), and any node
that could not hold at least a handful of distinct products.

## Using the data

Build the tree:

```python
import json

nodes = json.load(open("data/categories.json"))
by_slug = {n["slug"]: n for n in nodes}
for top in (n for n in nodes if n["level"] == 1):
    print(top["name"])
    for c in top["children"]:
        print("   ", by_slug[c]["name"])
```

Resolve whatever a user typed, aliases included:

```python
def resolve(q, nodes):
    q = q.strip().lower()
    for n in nodes:
        if n["slug"] == q or n["name"].lower() == q:
            return n
        if q in [a.lower() for a in n["aliases"]]:
            return n
    return None
```

Roll a level-2 slug up to its top-level category:

```python
def top_level(slug, by_slug):
    n = by_slug[slug]
    return by_slug[n["parent"]] if n["parent"] else n
```

Validate before you depend on it:

```bash
pip install check-jsonschema
check-jsonschema --schemafile data/schema.json data/categories.json
```

Slugs are the contract. Names get edited for clarity; slugs do not change, so anything you
key on them keeps working across releases.

## Known limitations

- **A taxonomy is an opinion.** This one is shaped by what people search for and what a
  directory has to file. Another defensible tree would put document extraction under
  automation rather than documents, and would not be wrong.
- **Some tools belong in several places.** The taxonomy does not solve that; it gives you
  stable nodes to file against, and the decision of whether to allow multiple assignments is
  yours.
- **No vertical categories.** Healthcare, legal, and education appear as work, not as
  industries. A tool sold to hospitals is still a transcription tool.
- **Two levels means some nodes are broad.** `Workflow automation` covers a great deal. That
  is the cost of refusing a third level, and it is a cost worth paying.

## Suggest a category

- [Suggest a category](../../issues/new?template=suggest-a-category.yml) — a form, two
  minutes.
- [Report a broken link](../../issues/new?template=report-a-broken-link.yml) — for anything
  here that points somewhere it should not.

The most useful suggestions are the ones with evidence behind them: a category you needed and
could not find a node for, and the tools that would sit in it. A proposal for a node with two
plausible members will be turned down, politely and with the reason.

## Contributing

Read [CONTRIBUTING.md](CONTRIBUTING.md). One category per pull request, name it by the job it
does, and say which existing node it would be taken out of.

## Disclaimer

This is an editorial taxonomy, not a standard. It is published because a usable shared tree is
more valuable than a perfect private one, and it will change as the field does. Nothing here
is an endorsement of any product, and no product is named in the dataset at all.

## License

[CC BY 4.0](LICENSE). Use it in a commercial directory, adapt it, extend it, as long as you
credit TiorAI and say what you changed.

The licence covers the category names, descriptions, and structure. It does not cover the
TiorAI name or logo.

## About TiorAI

[TiorAI](https://tiorai.com/) is an AI tools directory. Filing several thousand products means
having a tree to file them in; this is that tree, published separately so other people do not
have to invent their own.

- [AI tools directory](https://tiorai.com/tools/)
