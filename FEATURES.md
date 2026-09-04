# Features

What this repository does today, what is committed, and what is only an idea. The three
headings are not the same promise, and the difference is the point of the file.

## Available

Shipping now, in this release.

- **182 categories** across exactly two levels: 20 top-level and 162 subcategories.
- **Stable slugs.** Names get edited; slugs do not, so anything keyed on them survives a release.
- **A checked tree.** Every `parent` and every `children` entry resolves, no name appears twice, and no level-2 node has children.
- **Aliases.** American spellings and common abbreviations resolve to the right node, so `personalization`, `tts`, and `cro` all land somewhere.
- **Compatible with the TiorAI AI tools dataset.** The top level is the same twenty categories, so data labelled with one works with the other.
- **Three files.** Typed JSON, a flat CSV of every node, and a summary CSV of the top level.
- **A JSON Schema** that rejects a level-3 node and a malformed slug. The checks JSON Schema cannot express, such as a parent that points at nothing, run in the build and block the release.

## Planned

Committed. These have a decided shape and will land; nothing is listed here to make the
repository look busier than it is.

- **Aliases from the issue tracker.** What people type and fail to resolve is the best evidence of a missing alias, and better than guessing.
- **A review each time a top-level category passes twelve children**, which is the point at which it is really two categories.

## Ideas

Not committed, and possibly never. Listed because a contributor may want to argue for one, or
build it. Opening an issue about any of them is welcome.

- **A crosswalk to other public taxonomies**, so a directory could migrate onto this tree without re-labelling by hand. Useful, and a substantial piece of work that would need those taxonomies to be stable.
- **Translated names and descriptions.** Held back for the same reason as elsewhere in the portfolio: a confidently wrong translation is worse than none.
- **Per-node example queries**, showing what someone searching for that category actually types. Would make the selection rule visible instead of stated.
- **A third level.** Listed here only to record that it was considered and rejected, so the decision does not get relitigated every year.

---

Anything absent from all three lists is absent on purpose. See
[CONTRIBUTING.md](CONTRIBUTING.md) for what belongs here and what does not.
