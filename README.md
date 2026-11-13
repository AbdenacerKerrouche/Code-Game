# 🔐 Code Game: Operation Ironclad

A data-forensics escape room built for **DataSpace Club** members. Teams play detective, analyzing real datasets to crack five codes and unlock a hidden message.

## 🎮 How it works

- **Format:** 4 teams of 5 members, played on Discord
- **Duration:** 30 minutes
- **Goal:** solve all 5 cases and enter the correct code for each one
- **Rules:** no AI tools allowed. Pure data skills and teamwork.

When every code is correct, the vault opens and reveals a message for the team.

## 🕵️ The cases

Each case is a short briefing written as detective field notes. The clues are intentionally cryptic, and there are no step-by-step instructions. Players decide how to translate each clue into code.

| Case | Dataset | Skills tested |
|------|---------|---------------|
| 1. Operation Overdrive | `mtcars` | Multi-condition filtering |
| 2. The Anomaly Year | `house_data1000.csv` | Frequency counts, aggregation |
| 3. The Invisible Message | `house_data1000.csv` | Data visualization (scatter plots) |
| 4. The Impossible Structure | `house_data1000.csv` | Outlier detection |
| 5. The Ghost Asset | `house_data1000.csv` | Cross-referencing several conditions |

## 📁 Repository structure

```
code-game/
├── cases/              # The 5 case briefings (PDF)
├── data/
│   └── house_data1000.csv
|   └── mtcars.csv
├── escape-room.html          # Interactive code-entry interface
└── README.md
```

> `mtcars` is built into R (`mtcars`) and available in Python via `statsmodels` or `seaborn`.

## 💻 The interface

`index.html` is a single self-contained page (HTML, CSS, JavaScript with no dependencies). It:

- shows one input row per case
- validates each code and marks it ✅ or ❌
- triggers a confetti and message reveal when all five are correct

To run it, open `index.html` in any browser, or host it for free with **GitHub Pages**.

## 🛠️ Tools

Python or R for the analysis, vanilla JavaScript for the interface, Discord for running the event.

## 🔁 Run it yourself

1. Share the case PDFs and the dataset with your teams
2. Host `escape-room.html` (GitHub Pages works)
3. Set a timer and let them play

## 👤 Author

**Abdenacer Kerrouche**, DataSpace Club
[LinkedIn](https://linkedin.com/in/abdenacer-kerrouche) · [GitHub](https://github.com/AbdenacerKerrouche)
