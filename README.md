# Catholic Bible Cross References

Cross references from the RSV-CE (Revised Standard Version, Catholic Edition) Old Testament, covering Genesis through Jeremiah. Each file maps source passages to related passages elsewhere in Scripture.

## Format

Each JSON file is an array of objects:

```json
[
  { "source": "Gen 1:1", "target": "Jn 1:1" },
  { "source": "Gen 1:26, 27", "target": "Gen 5:1" },
  { "source": "Gen 1:26, 27", "target": "Mt 19:4" },
  { "source": "Gen 2:9", "target": "Rev 22:2" },
  { "source": "Gen 2:9", "target": "Rev 22:14" }
]
```

- **source** — the passage being referenced from
- **target** — the related passage elsewhere in Scripture

## Books Included

| File | Book | References |
|------|------|------------|
| `genesis.json` | Genesis | 150 |
| `exodus.json` | Exodus | 318 |
| `leviticus.json` | Leviticus | 199 |
| `numbers.json` | Numbers | 129 |
| `deuteronomy.json` | Deuteronomy | 272 |
| `joshua.json` | Joshua | 29 |
| `judges.json` | Judges | 12 |
| `ruth.json` | Ruth | 1 |
| `1_samuel.json` | 1 Samuel | 18 |
| `2_samuel.json` | 2 Samuel | 29 |
| `1_kings.json` | 1 Kings | 49 |
| `2_kings.json` | 2 Kings | 48 |
| `1_chronicles.json` | 1 Chronicles | 61 |
| `2_chronicles.json` | 2 Chronicles | 77 |
| `ezra.json` | Ezra | 11 |
| `nehemiah.json` | Nehemiah | 3 |
| `esther.json` | Esther | 2 |
| `job.json` | Job | 7 |
| `the_psalms.json` | Psalms | 173 |
| `the_proverbs.json` | Proverbs | 14 |
| `the_prophet_isaiah.json` | Isaiah | 249 |
| `jeremiah.json` | Jeremiah | 65 |

**Total: 1,916 cross references across 22 books**

## Reference Conventions

- **Verse ranges** use an en-dash: `"Ex 1:1–4"`
- **Multiple verses** are comma-separated: `"Gen 1:26, 27"`
- **Targets point both directions** — OT references link to NT and vice versa, and OT books cross-reference each other
- **Targets may be chapters** (e.g. `"Gen 5"`) or specific verses (e.g. `"Jn 1:1"`)

## Scope

This covers the Pentateuch, Historical Books, Wisdom Literature, and Major Prophets. The remaining OT books (Minor Prophets, Daniel, Ezekiel) and the New Testament are not included as source books in this dataset, though they appear frequently as targets.
