# 📚 Dokkadoki — Library Completion Shopping List

Everything the Dokkadoki manga café needs to buy to complete its collection.
Auto-generated every Monday from the live Libib catalogue (903 books, 106 series).

## Files

| File | Contents |
|---|---|
| `shopping-list-full.txt` | **Every** missing volume, one per line (`Series, Vol. N`) |
| `shopping-list-12plus.txt` | Only series needing **12+ volumes** (the big completions) |
| `shopping-list-small.txt` | Series needing **under 12 volumes** (quick wins) |

## How to use

- Tick books off as you buy them — add them to Libib and next week's scan
  regenerates this list automatically
- Open the raw files on your phone while out and about:
  - `shopping-list-full.txt`
  - `shopping-list-12plus.txt`
  - `shopping-list-small.txt`

## Stats (last generated: 2026-08-17)

- **Total books in library:** 903 (Manga 877 · Manga-Japanese 22 · Novel 4)
- **Series to complete:** 106
- **Individual volumes to buy:** ~1,175

## How it's generated

A weekly cron job on the Hermes server:
1. Scans the public Libib page (`libib.com/u/dokkadoki`)
2. Verifies each series' volume count against Wikipedia/Jikan/AniList
3. Diffs owned vs published → regenerates these lists
4. Pushes updates to this repo automatically

---

*Dokkadoki · Bury's manga café, coming soon* 🐱🌸
