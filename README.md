# Catholic Bible Cross References

Cross references covering the full 73-book Catholic canon, merged from three independent cross-reference apparatuses (one per source edition) and deduplicated into a single dataset. All verse loci are structured, integer-based data — no string parsing required.

## Format

Each JSON file is an array of reference groups, one per source passage:

```json
[
  {
    "chapter": 1,
    "verse": 1,
    "targets": [
      { "book": "Jn", "chapter": 1, "verse": 1 }
    ]
  },
  {
    "chapter": 2,
    "verse": 1,
    "verse_end": 3,
    "targets": [
      { "book": "Ex", "chapter": 20, "verse": 11 }
    ]
  }
]
```

- **chapter / verse** — where the source passage begins. `verse` is omitted when the group refers to a whole chapter.
- **verse_end** — present when the source passage is a verse range within the same chapter.
- **chapter_end** — present when the source passage spans multiple chapters.
- **targets** — the related passages elsewhere in Scripture, each shaped the same way (`book`, `chapter`, optional `verse` / `verse_end` / `chapter_end`).
- Book codes are abbreviations (see table below); target passages may point to any book in the canon, including deuterocanonical books, in either direction (OT↔NT, book↔book).

## Books Included

### Old Testament

| File | Book | Code | Groups | Targets |
|------|------|------|--------|---------|
| `Genesis.json` | Genesis | Gen | 435 | 977 |
| `Exodus.json` | Exodus | Ex | 422 | 922 |
| `Leviticus.json` | Leviticus | Lev | 386 | 1,056 |
| `Numbers.json` | Numbers | Nm | 313 | 574 |
| `Deuteronomy.json` | Deuteronomy | Dt | 646 | 2,444 |
| `Joshua.json` | Joshua | Jos | 252 | 515 |
| `Judges.json` | Judges | Jgs | 206 | 495 |
| `Ruth.json` | Ruth | Ru | 24 | 45 |
| `1Samuel.json` | 1 Samuel | 1Sm | 316 | 773 |
| `2Samuel.json` | 2 Samuel | 2Sm | 248 | 461 |
| `1Kings.json` | 1 Kings | 1Kgs | 176 | 286 |
| `2Kings.json` | 2 Kings | 2Kgs | 238 | 374 |
| `1Chronicles.json` | 1 Chronicles | 1Chr | 386 | 910 |
| `2Chronicles.json` | 2 Chronicles | 2Chr | 339 | 507 |
| `Ezra.json` | Ezra | Ezr | 46 | 93 |
| `Nehemiah.json` | Nehemiah | Neh | 86 | 146 |
| `Tobit.json` | Tobit | Tb | 69 | 193 |
| `Judith.json` | Judith | Jdt | 122 | 455 |
| `Esther.json` | Esther | Est | 56 | 100 |
| `1Maccabees.json` | 1 Maccabees | 1Mc | 154 | 251 |
| `2Maccabees.json` | 2 Maccabees | 2Mc | 122 | 218 |
| `Job.json` | Job | Jb | 207 | 386 |
| `Psalms.json` | Psalms | Ps | 1,296 | 3,134 |
| `Proverbs.json` | Proverbs | Prv | 274 | 527 |
| `Ecclesiastes.json` | Ecclesiastes | Ecc | 64 | 130 |
| `SongOfSongs.json` | Song of Songs | Sg | 40 | 58 |
| `Wisdom.json` | Wisdom | Wis | 307 | 755 |
| `Sirach.json` | Sirach | Sir | 396 | 816 |
| `Isaiah.json` | Isaiah | Is | 765 | 1,728 |
| `Jeremiah.json` | Jeremiah | Jer | 790 | 1,502 |
| `Lamentations.json` | Lamentations | Lam | 78 | 149 |
| `Baruch.json` | Baruch | Bar | 101 | 199 |
| `Ezekiel.json` | Ezekiel | Ez | 621 | 1,148 |
| `Daniel.json` | Daniel | Dn | 72 | 158 |
| `Hosea.json` | Hosea | Hos | 123 | 310 |
| `Joel.json` | Joel | Jl | 49 | 142 |
| `Amos.json` | Amos | Am | 80 | 180 |
| `Obadiah.json` | Obadiah | Ob | 12 | 24 |
| `Jonah.json` | Jonah | Jon | 19 | 36 |
| `Micah.json` | Micah | Mi | 46 | 93 |
| `Nahum.json` | Nahum | Na | 18 | 33 |
| `Habakkuk.json` | Habakkuk | Hb | 24 | 40 |
| `Zephaniah.json` | Zephaniah | Zep | 32 | 65 |
| `Haggai.json` | Haggai | Hg | 15 | 20 |
| `Zechariah.json` | Zechariah | Zec | 109 | 254 |
| `Malachi.json` | Malachi | Mal | 34 | 107 |

### New Testament

| File | Book | Code | Groups | Targets |
|------|------|------|--------|---------|
| `Matthew.json` | Matthew | Mt | 794 | 2,202 |
| `Mark.json` | Mark | Mk | 466 | 1,141 |
| `Luke.json` | Luke | Lk | 881 | 2,519 |
| `John.json` | John | Jn | 645 | 2,165 |
| `Acts.json` | Acts | Acts | 410 | 971 |
| `Romans.json` | Romans | Rom | 383 | 1,312 |
| `1Corinthians.json` | 1 Corinthians | 1Cor | 270 | 735 |
| `2Corinthians.json` | 2 Corinthians | 2Cor | 155 | 379 |
| `Galatians.json` | Galatians | Gal | 123 | 343 |
| `Ephesians.json` | Ephesians | Eph | 134 | 314 |
| `Philippians.json` | Philippians | Phil | 81 | 270 |
| `Colossians.json` | Colossians | Col | 76 | 200 |
| `1Thessalonians.json` | 1 Thessalonians | 1Thes | 70 | 226 |
| `2Thessalonians.json` | 2 Thessalonians | 2Thes | 38 | 101 |
| `1Timothy.json` | 1 Timothy | 1Tim | 71 | 172 |
| `2Timothy.json` | 2 Timothy | 2Tim | 68 | 182 |
| `Titus.json` | Titus | Ti | 30 | 153 |
| `Philemon.json` | Philemon | Phlm | 17 | 45 |
| `Hebrews.json` | Hebrews | Heb | 232 | 657 |
| `James.json` | James | Jas | 60 | 135 |
| `1Peter.json` | 1 Peter | 1Pt | 70 | 138 |
| `2Peter.json` | 2 Peter | 2Pt | 48 | 107 |
| `1John.json` | 1 John | 1Jn | 84 | 203 |
| `2John.json` | 2 John | 2Jn | 8 | 19 |
| `3John.json` | 3 John | 3Jn | 10 | 29 |
| `Jude.json` | Jude | Jd | 23 | 66 |
| `Revelation.json` | Revelation | Rev | 269 | 667 |

**Total: 16,130 reference groups / 39,240 targets across all 73 books.**

## Notes

- Data was extracted from the cross-reference apparatuses of three published Catholic Bible editions, normalized to a single book-code and locus scheme, merged, and deduplicated (a target appearing in more than one source is kept once).
- A handful of loci are preserved exactly as printed in their source even though they look like typos (e.g. a verse range where the end verse is lower than the start) — these are not extraction bugs, just faithfully reproduced print errors.
- Book codes follow standard scholarly abbreviations (e.g. `1Sm` = 1 Samuel, `Sg` = Song of Songs, `Ti` = Titus).
