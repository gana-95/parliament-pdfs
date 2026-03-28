# 🏛️ Lok Sabha Debate PDFs

A public archive of English debate transcripts from the Indian Parliament (Lok Sabha), sourced from the [Sansad Digital Library](https://eparlib.sansad.in/handle/123456789/2963706) and updated automatically every night.

This repository is the **data store** for the [gana-95/speech-scraper](https://github.com/gana-95/speech-scraper) pipeline. New PDFs are committed here each midnight by an automated job running on a GCP VM.

---

## What's in Here

```
debates/
├── 2023/
│   ├── debate_DD-Mon-2023.pdf
│   └── ...
├── 2024/
│   └── ...
└── 2025/
    └── ...
```

Each PDF is an official English transcript of a Lok Sabha debate session, organised by year. File names reflect the debate date as published in the source library.

---

## Update Frequency

This repository is updated **every night at midnight (IST)** by the scraper pipeline. Each automated commit is tagged with the upload date, so you can track exactly when PDFs were added.

---

## Using This Data

You can clone the full archive or pull individual files directly via the GitHub raw URL.

```bash
# Clone the full archive
git clone https://github.com/gana-95/parliament-pdfs.git

# Pull only the latest changes (after an initial clone)
git pull
```

**Direct file URL format:**
```
https://raw.githubusercontent.com/gana-95/parliament-pdfs/main/debates/YEAR/filename.pdf
```

This dataset is well-suited for NLP research, political science analysis, speech pattern studies, topic modelling, and building search tools over Indian parliamentary proceedings.

---

## Data Source & Rights

All PDFs are sourced from the [Lok Sabha Digital Library](https://eparlib.sansad.in/handle/123456789/2963706), the official open-access archive of Lok Sabha proceedings maintained by the Parliament of India. The data is in the public domain.

---

## Related

- **Scraper pipeline:** [gana-95/speech-scraper](https://github.com/gana-95/speech-scraper) — source code, setup guide, and deployment details
- **Upstream source:** [Sansad Digital Library](https://eparlib.sansad.in/handle/123456789/2963706)

---

*This archive is maintained for academic and research use.*
