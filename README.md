# Catholic Bible Cross References

Cross references extracted from the **Ignatius Bible (RSV-CE)** "Parallel Notes" section.

Each JSON file contains an array of cross reference objects with `source` and `target` fields.

```json
[
  { "source": "Gen 1:1", "target": "Jn 1:1" },
  { "source": "Gen 1:26, 27", "target": "Gen 5:1" },
  { "source": "Gen 1:26, 27", "target": "Mt 19:4" }
]
```

## Books Included

| File | Cross References |
|------|-----------------|
| genesis.json | 150 |
| exodus.json | 318 |
| leviticus.json | 199 |
| numbers.json | 129 |
| deuteronomy.json | 272 |
| joshua.json | 29 |
| judges.json | 12 |
| ruth.json | 1 |
| 1_samuel.json | 18 |
| 2_samuel.json | 29 |
| 1_kings.json | 49 |
| 2_kings.json | 48 |
| 1_chronicles.json | 61 |
| 2_chronicles.json | 77 |
| ezra.json | 11 |
| nehemiah.json | 3 |
| esther.json | 2 |
| job.json | 7 |
| the_psalms.json | 173 |
| the_proverbs.json | 14 |
| the_prophet_isaiah.json | 249 |
| jeremiah.json | 65 |

**Total: 1,916 cross references across 22 books**

## Notes

- Some targets are shorthand (e.g. `"10"`) referring to the same chapter as the previous reference
- Source references may contain multiple verses (e.g. `"Gen 1:26, 27"`)
- Verse ranges use en-dash (e.g. `"Ex 1:1–4"`)
