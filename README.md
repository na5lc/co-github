# co-github

A simple script to fill your GitHub contribution graph by generating backdated commits automatically.

---

## What It Does

Generates a series of commits with random past dates (within the last year) and pushes them to your repository — making your GitHub contribution graph look active.

---

## How It Works

- Uses `moment.js` to calculate backdated timestamps
- Writes date data to `data.json`
- Commits each entry with the backdated timestamp using `simple-git`
- Pushes all commits to your GitHub repository

---

## Installation

```bash
git clone https://github.com/na5lc/co-github.git
cd co-github
npm install
```

---

## Usage

```bash
node index.js
```

You can customize the number of commits by changing the `n` value in the `makeCommits(n)` call.

---

## Dependencies

| Package | Purpose |
|---|---|
| `simple-git` | Git operations from Node.js |
| `moment` | Date formatting & manipulation |
| `jsonfile` | Reading & writing JSON files |
| `random` | Generating random week/day offsets |

---

## ⚠️ Note

This is for **learning and experimentation** only. Use responsibly.

---

## License

MIT © [Nafees](https://github.com/na5lc)
