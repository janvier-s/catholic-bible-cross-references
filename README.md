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
| `01-Genesis.json` | Genesis | Gen | 446 | 1,016 |
| `02-Exodus.json` | Exodus | Ex | 424 | 925 |
| `03-Leviticus.json` | Leviticus | Lev | 386 | 1,056 |
| `04-Numbers.json` | Numbers | Nm | 314 | 575 |
| `05-Deuteronomy.json` | Deuteronomy | Dt | 646 | 2,444 |
| `06-Joshua.json` | Joshua | Jos | 252 | 518 |
| `07-Judges.json` | Judges | Jgs | 206 | 496 |
| `08-Ruth.json` | Ruth | Ru | 24 | 45 |
| `09-1_Samuel.json` | 1 Samuel | 1Sm | 316 | 773 |
| `10-2_Samuel.json` | 2 Samuel | 2Sm | 248 | 462 |
| `11-1_Kings.json` | 1 Kings | 1Kgs | 178 | 290 |
| `12-2_Kings.json` | 2 Kings | 2Kgs | 238 | 375 |
| `13-1_Chronicles.json` | 1 Chronicles | 1Chr | 391 | 918 |
| `14-2_Chronicles.json` | 2 Chronicles | 2Chr | 351 | 537 |
| `15-Ezra.json` | Ezra | Ezr | 46 | 97 |
| `16-Nehemiah.json` | Nehemiah | Neh | 87 | 148 |
| `17-Tobit.json` | Tobit | Tb | 69 | 193 |
| `18-Judith.json` | Judith | Jdt | 126 | 469 |
| `19-Esther.json` | Esther | Est | 63 | 110 |
| `20-1_Maccabees.json` | 1 Maccabees | 1Mc | 156 | 266 |
| `21-2_Maccabees.json` | 2 Maccabees | 2Mc | 124 | 226 |
| `22-Job.json` | Job | Jb | 207 | 386 |
| `23-Psalms.json` | Psalms | Ps | 1,322 | 3,289 |
| `24-Proverbs.json` | Proverbs | Prv | 276 | 532 |
| `25-Ecclesiastes.json` | Ecclesiastes | Ecc | 66 | 138 |
| `26-SongOfSongs.json` | Song of Songs | Sg | 40 | 58 |
| `27-Wisdom.json` | Wisdom | Wis | 317 | 792 |
| `28-Sirach.json` | Sirach | Sir | 479 | 969 |
| `29-Isaiah.json` | Isaiah | Is | 785 | 1,892 |
| `30-Jeremiah.json` | Jeremiah | Jer | 810 | 1,637 |
| `31-Lamentations.json` | Lamentations | Lam | 78 | 149 |
| `32-Baruch.json` | Baruch | Bar | 104 | 208 |
| `33-Ezekiel.json` | Ezekiel | Ez | 623 | 1,154 |
| `34-Daniel.json` | Daniel | Dn | 75 | 165 |
| `35-Hosea.json` | Hosea | Hos | 126 | 330 |
| `36-Joel.json` | Joel | Jl | 51 | 156 |
| `37-Amos.json` | Amos | Am | 82 | 204 |
| `38-Obadiah.json` | Obadiah | Ob | 14 | 28 |
| `39-Jonah.json` | Jonah | Jon | 20 | 44 |
| `40-Micah.json` | Micah | Mi | 47 | 114 |
| `41-Nahum.json` | Nahum | Na | 18 | 39 |
| `42-Habakkuk.json` | Habakkuk | Hb | 25 | 47 |
| `43-Zephaniah.json` | Zephaniah | Zep | 32 | 73 |
| `44-Haggai.json` | Haggai | Hg | 16 | 25 |
| `45-Zechariah.json` | Zechariah | Zec | 114 | 280 |
| `46-Malachi.json` | Malachi | Mal | 38 | 125 |

### New Testament

| File | Book | Code | Groups | Targets |
|------|------|------|--------|---------|
| `47-Matthew.json` | Matthew | Mt | 849 | 2,433 |
| `48-Mark.json` | Mark | Mk | 512 | 1,294 |
| `49-Luke.json` | Luke | Lk | 927 | 2,715 |
| `50-John.json` | John | Jn | 656 | 2,264 |
| `51-Acts.json` | Acts | Acts | 431 | 1,061 |
| `52-Romans.json` | Romans | Rom | 384 | 1,342 |
| `53-1_Corinthians.json` | 1 Corinthians | 1Cor | 271 | 770 |
| `54-2_Corinthians.json` | 2 Corinthians | 2Cor | 158 | 393 |
| `55-Galatians.json` | Galatians | Gal | 123 | 353 |
| `56-Ephesians.json` | Ephesians | Eph | 136 | 343 |
| `57-Philippians.json` | Philippians | Phil | 81 | 275 |
| `58-Colossians.json` | Colossians | Col | 77 | 208 |
| `59-1_Thessalonians.json` | 1 Thessalonians | 1Thes | 70 | 239 |
| `60-2_Thessalonians.json` | 2 Thessalonians | 2Thes | 39 | 107 |
| `61-1_Timothy.json` | 1 Timothy | 1Tim | 73 | 188 |
| `62-2_Timothy.json` | 2 Timothy | 2Tim | 68 | 187 |
| `63-Titus.json` | Titus | Ti | 31 | 159 |
| `64-Philemon.json` | Philemon | Phlm | 17 | 45 |
| `65-Hebrews.json` | Hebrews | Heb | 241 | 738 |
| `66-James.json` | James | Jas | 65 | 162 |
| `67-1_Peter.json` | 1 Peter | 1Pt | 74 | 181 |
| `68-2_Peter.json` | 2 Peter | 2Pt | 49 | 117 |
| `69-1_John.json` | 1 John | 1Jn | 84 | 228 |
| `70-2_John.json` | 2 John | 2Jn | 8 | 20 |
| `71-3_John.json` | 3 John | 3Jn | 10 | 29 |
| `72-Jude.json` | Jude | Jd | 23 | 71 |
| `73-Revelation.json` | Revelation | Rev | 274 | 730 |

**Total: 16,587 reference groups / 41,425 targets across all 73 books.**

## Notes

- Files are numbered in canonical Bible order (`01-Genesis.json` … `73-Revelation.json`), so directory listings sort in reading order instead of alphabetically.
- Data was extracted from the cross-reference apparatuses of four published Catholic Bible editions (including one historic pre-modern translation), normalized to a single book-code and locus scheme, merged, and deduplicated (a target appearing in more than one source is kept once).
- Includes cross-references for the Esther "additions" (Vulgate chapters 11–16), a body of deuterocanonical material specific to the Catholic canon that is sparsely cross-referenced in modern editions.
- Book codes follow standard scholarly abbreviations (e.g. `1Sm` = 1 Samuel, `Sg` = Song of Songs, `Ti` = Titus).
