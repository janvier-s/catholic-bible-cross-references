# Catholic Bible Cross References

Cross references extracted from the Parallel Notes section of a Catholic Bible. Each file maps source passages to related passages elsewhere in Scripture.

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

### Old Testament

| File | Book | References |
|------|------|------------|
| `genesis.json` | Genesis | 150 |
| `exodus.json` | Exodus | 318 |
| `leviticus.json` | Leviticus | 199 |
| `numbers.json` | Numbers | 129 |
| `deuteronomy.json` | Deuteronomy | 273 |
| `joshua.json` | Joshua | 29 |
| `judges.json` | Judges | 12 |
| `ruth.json` | Ruth | 1 |
| `1_samuel.json` | 1 Samuel | 21 |
| `2_samuel.json` | 2 Samuel | 44 |
| `1_kings.json` | 1 Kings | 51 |
| `2_kings.json` | 2 Kings | 56 |
| `1_chronicles.json` | 1 Chronicles | 72 |
| `2_chronicles.json` | 2 Chronicles | 83 |
| `ezra.json` | Ezra | 11 |
| `nehemiah.json` | Nehemiah | 4 |
| `esther.json` | Esther | 2 |
| `job.json` | Job | 7 |
| `psalms.json` | Psalms | 176 |
| `proverbs.json` | Proverbs | 14 |
| `ecclesiastes.json` | Ecclesiastes | 1 |
| `isaiah.json` | Isaiah | 251 |
| `jeremiah.json` | Jeremiah | 66 |
| `ezekiel.json` | Ezekiel | 147 |
| `daniel.json` | Daniel | 63 |
| `hosea.json` | Hosea | 23 |
| `joel.json` | Joel | 30 |
| `amos.json` | Amos | 32 |
| `obadiah.json` | Obadiah | 7 |
| `jonah.json` | Jonah | 3 |
| `micah.json` | Micah | 11 |
| `nahum.json` | Nahum | 6 |
| `habakkuk.json` | Habakkuk | 13 |
| `zephaniah.json` | Zephaniah | 17 |
| `haggai.json` | Haggai | 1 |
| `zechariah.json` | Zechariah | 30 |
| `malachi.json` | Malachi | 17 |

### New Testament

| File | Book | References |
|------|------|------------|
| `matthew.json` | Matthew | 1,309 |
| `mark.json` | Mark | 584 |
| `luke.json` | Luke | 108 |
| `john.json` | John | 1,019 |
| `acts.json` | Acts | 161 |
| `romans.json` | Romans | 83 |
| `1_corinthians.json` | 1 Corinthians | 415 |
| `2_corinthians.json` | 2 Corinthians | 160 |
| `galatians.json` | Galatians | 62 |
| `ephesians.json` | Ephesians | 42 |
| `philippians.json` | Philippians | 58 |
| `colossians.json` | Colossians | 42 |
| `1_thessalonians.json` | 1 Thessalonians | 141 |
| `2_thessalonians.json` | 2 Thessalonians | 52 |
| `1_timothy.json` | 1 Timothy | 10 |
| `2_timothy.json` | 2 Timothy | 7 |
| `titus.json` | Titus | 3 |
| `philemon.json` | Philemon | 8 |
| `hebrews.json` | Hebrews | 139 |
| `james.json` | James | 19 |
| `1_peter.json` | 1 Peter | 21 |
| `2_peter.json` | 2 Peter | 22 |
| `1_john.json` | 1 John | 87 |
| `2_john.json` | 2 John | 6 |
| `3_john.json` | 3 John | 4 |
| `jude.json` | Jude | 7 |
| `revelation.json` | Revelation | 17 |

**Total: 7,392 cross references across 67 books**

## Reference Conventions

- **Verse ranges** use an en-dash: `"Ex 1:1–4"`
- **Multiple verses** are comma-separated: `"Gen 1:26, 27"`
- **Targets point both directions** — OT links to NT, NT links to OT, and books cross-reference each other
- **Targets may be chapters** (e.g. `"Gen 5"`) or specific verses (e.g. `"Jn 1:1"`)
