# 📚 Dokkadoki — Library Completion Shopping List

Everything the Dokkadoki manga café needs to buy to complete its collection.
Auto-generated every Monday from the live Libib catalogue (903 books).
Every book in the library is accounted for — verified against
Wikipedia/Jikan/AniList/Fandom plus manual checks.

## Files

| File | Contents |
|---|---|
| `completed-series.txt` | Series that are **already complete** (nothing to buy) |
| `needs-1-2-books.txt` | Series needing **1–2 volumes** (quick wins) |
| `needs-3-9-books.txt` | Series needing **3–9 volumes** |
| `needs-10-plus-books.txt` | Series needing **10+ volumes** (the big completions) |
| `unresolved-worklist.txt` | Anything still needing manual verification |

All lists are alphabetical by series, each line naming one book
(`Series, Vol. N`). Tick them off as you buy — add books to Libib and
next week's scan regenerates everything automatically.

## Stats (last generated: 2026-08-18)

- **Total books in library:** 903 (Manga 877 · Manga-Japanese 22 · Novel 4)
- **Series to complete:** 147
- **Volumes to buy:** ~1,770 (1-2: 38 · 3-9: 289 · 10+: 1,443)
- **Completed series:** 47

## How it's generated

A weekly cron job on the Hermes server:
1. Scans the public Libib page (`libib.com/u/dokkadoki`)
2. Verifies each series' volume count against Wikipedia/Jikan/AniList/Fandom
3. Diffs owned vs published → regenerates these lists
4. Pushes updates to this repo automatically

---

*Dokkadoki · Bury's manga café, coming soon* 🐱🌸
