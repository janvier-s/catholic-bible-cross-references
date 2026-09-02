# Catholic Bible Cross References

Cross references covering the full 73-book Catholic canon, merged from four independent cross-reference apparatuses (one per source edition, including a historic pre-modern translation) and deduplicated into a single dataset. All verse loci are structured, integer-based data — no string parsing required.

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
| `Genesis.json` | Genesis | Gen | 446 | 1,016 |
| `Exodus.json` | Exodus | Ex | 424 | 925 |
| `Leviticus.json` | Leviticus | Lev | 386 | 1,056 |
| `Numbers.json` | Numbers | Nm | 314 | 575 |
| `Deuteronomy.json` | Deuteronomy | Dt | 646 | 2,444 |
| `Joshua.json` | Joshua | Jos | 252 | 518 |
| `Judges.json` | Judges | Jgs | 206 | 496 |
| `Ruth.json` | Ruth | Ru | 24 | 45 |
| `1Samuel.json` | 1 Samuel | 1Sm | 316 | 773 |
| `2Samuel.json` | 2 Samuel | 2Sm | 248 | 462 |
| `1Kings.json` | 1 Kings | 1Kgs | 178 | 290 |
| `2Kings.json` | 2 Kings | 2Kgs | 238 | 375 |
| `1Chronicles.json` | 1 Chronicles | 1Chr | 391 | 918 |
| `2Chronicles.json` | 2 Chronicles | 2Chr | 351 | 537 |
| `Ezra.json` | Ezra | Ezr | 46 | 97 |
| `Nehemiah.json` | Nehemiah | Neh | 87 | 148 |
| `Tobit.json` | Tobit | Tb | 69 | 193 |
| `Judith.json` | Judith | Jdt | 126 | 469 |
| `Esther.json` | Esther | Est | 63 | 110 |
| `1Maccabees.json` | 1 Maccabees | 1Mc | 156 | 266 |
| `2Maccabees.json` | 2 Maccabees | 2Mc | 124 | 226 |
| `Job.json` | Job | Jb | 207 | 386 |
| `Psalms.json` | Psalms | Ps | 1,322 | 3,289 |
| `Proverbs.json` | Proverbs | Prv | 276 | 532 |
| `Ecclesiastes.json` | Ecclesiastes | Ecc | 66 | 138 |
| `SongOfSongs.json` | Song of Songs | Sg | 40 | 58 |
| `Wisdom.json` | Wisdom | Wis | 317 | 792 |
| `Sirach.json` | Sirach | Sir | 479 | 969 |
| `Isaiah.json` | Isaiah | Is | 785 | 1,892 |
| `Jeremiah.json` | Jeremiah | Jer | 810 | 1,637 |
| `Lamentations.json` | Lamentations | Lam | 78 | 149 |
| `Baruch.json` | Baruch | Bar | 104 | 208 |
| `Ezekiel.json` | Ezekiel | Ez | 623 | 1,154 |
| `Daniel.json` | Daniel | Dn | 75 | 165 |
| `Hosea.json` | Hosea | Hos | 126 | 330 |
| `Joel.json` | Joel | Jl | 51 | 156 |
| `Amos.json` | Amos | Am | 82 | 204 |
| `Obadiah.json` | Obadiah | Ob | 14 | 28 |
| `Jonah.json` | Jonah | Jon | 20 | 44 |
| `Micah.json` | Micah | Mi | 47 | 114 |
| `Nahum.json` | Nahum | Na | 18 | 39 |
| `Habakkuk.json` | Habakkuk | Hb | 25 | 47 |
| `Zephaniah.json` | Zephaniah | Zep | 32 | 73 |
| `Haggai.json` | Haggai | Hg | 16 | 25 |
| `Zechariah.json` | Zechariah | Zec | 114 | 280 |
| `Malachi.json` | Malachi | Mal | 38 | 125 |

### New Testament

| File | Book | Code | Groups | Targets |
|------|------|------|--------|---------|
| `Matthew.json` | Matthew | Mt | 849 | 2,433 |
| `Mark.json` | Mark | Mk | 512 | 1,294 |
| `Luke.json` | Luke | Lk | 927 | 2,715 |
| `John.json` | John | Jn | 656 | 2,264 |
| `Acts.json` | Acts | Acts | 431 | 1,061 |
| `Romans.json` | Romans | Rom | 384 | 1,342 |
| `1Corinthians.json` | 1 Corinthians | 1Cor | 271 | 770 |
| `2Corinthians.json` | 2 Corinthians | 2Cor | 158 | 393 |
| `Galatians.json` | Galatians | Gal | 123 | 353 |
| `Ephesians.json` | Ephesians | Eph | 136 | 343 |
| `Philippians.json` | Philippians | Phil | 81 | 275 |
| `Colossians.json` | Colossians | Col | 77 | 208 |
| `1Thessalonians.json` | 1 Thessalonians | 1Thes | 70 | 239 |
| `2Thessalonians.json` | 2 Thessalonians | 2Thes | 39 | 107 |
| `1Timothy.json` | 1 Timothy | 1Tim | 73 | 188 |
| `2Timothy.json` | 2 Timothy | 2Tim | 68 | 187 |
| `Titus.json` | Titus | Ti | 31 | 159 |
| `Philemon.json` | Philemon | Phlm | 17 | 45 |
| `Hebrews.json` | Hebrews | Heb | 241 | 738 |
| `James.json` | James | Jas | 65 | 162 |
| `1Peter.json` | 1 Peter | 1Pt | 74 | 181 |
| `2Peter.json` | 2 Peter | 2Pt | 49 | 117 |
| `1John.json` | 1 John | 1Jn | 84 | 228 |
| `2John.json` | 2 John | 2Jn | 8 | 20 |
| `3John.json` | 3 John | 3Jn | 10 | 29 |
| `Jude.json` | Jude | Jd | 23 | 71 |
| `Revelation.json` | Revelation | Rev | 274 | 730 |

**Total: 16,587 reference groups / 41,425 targets across all 73 books.**

## Notes

- Data was extracted from the cross-reference apparatuses of four published Catholic Bible editions (including one historic pre-modern translation), normalized to a single book-code and locus scheme, merged, and deduplicated (a target appearing in more than one source is kept once).
- Includes cross-references for the Esther "additions" (Vulgate chapters 11–16), a body of deuterocanonical material specific to the Catholic canon that is sparsely cross-referenced in modern editions.
- Book codes follow standard scholarly abbreviations (e.g. `1Sm` = 1 Samuel, `Sg` = Song of Songs, `Ti` = Titus).
