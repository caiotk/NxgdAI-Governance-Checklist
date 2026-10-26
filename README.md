# NexGuide.AI — AI Governance Checklist

Twelve controls to build, run and evidence responsible AI at enterprise scale. Each control comes with the evidence an auditor will ask for, a quick test you can run this week, a suggested owner, and an indicative mapping to **ISO/IEC 42001**, the **NIST AI RMF** and the **EU AI Act**, plus an *Also maps to* column for **ISO/IEC 27090:2026** (AI security), **EN 18286:2026** (the EU AI Act harmonised quality-management standard), **IEEE 2863-2026** (organisational AI governance) and Australia's **Guidance for AI Adoption (AI6)**.

## Pick your format

| Format | Use it for | Link |
|---|---|---|
| **Web** | Work through it in the browser — status per control, notes, progress ring, CSV export, print. Progress is saved in your browser only. | [caiotk.github.io/NxgdAI-Governance-Checklist](https://caiotk.github.io/NxgdAI-Governance-Checklist/) |
| **Markdown** | Read on GitHub, copy into a wiki, Notion or a pull request. | [CHECKLIST.md](CHECKLIST.md) |
| **Excel** | Assign owners and dates, filter, report. Status dropdowns, colour coding and a live Dashboard sheet. | [sheets/ai-governance-checklist.xlsx](sheets/ai-governance-checklist.xlsx) |
| **Google Sheets** | Share and edit as a team. | [sheets/checklist.csv](sheets/checklist.csv) — see below |

### Open in Google Sheets

Either:

- **Upload the Excel file**: in Google Drive, *New → File upload → `ai-governance-checklist.xlsx`*, then *Open with → Google Sheets*. Dropdowns, colours and the Dashboard formulas carry across.
- **Import the CSV live**: in a new sheet, put this in cell A1:

  ```
  =IMPORTDATA("https://raw.githubusercontent.com/caiotk/NxgdAI-Governance-Checklist/main/sheets/checklist.csv")
  ```

  Then *Edit → Copy*, *Paste special → Values only* if you want to edit the rows.

## The twelve controls

| # | Control | Area |
|---|---|---|
| 01 | AI inventory completed | Foundations |
| 02 | Risk classification framework defined | Foundations |
| 03 | Governance committee established | Accountability |
| 04 | AI policies documented | Accountability |
| 05 | Model documentation standardised | Transparency |
| 06 | Bias and fairness testing implemented | Trustworthiness |
| 07 | Explainability requirements defined | Trustworthiness |
| 08 | Security and privacy controls applied | Protection |
| 09 | Continuous monitoring enabled | Operations |
| 10 | Incident response process established | Operations |
| 11 | Regulatory compliance reviews scheduled | Assurance |
| 12 | Generative AI usage rules created | Foundations |

**Status scale:** Not started → In progress → Implemented → **Evidenced** (or Not applicable). A control is only audit-ready when it is *Evidenced* — implemented, and you can show the proof.

## Editing the checklist

All four formats are generated from one file, [`data/checklist.json`](data/checklist.json). Change it there, then rebuild:

```bash
pip install openpyxl
python3 scripts/build.py
```

That regenerates `CHECKLIST.md`, `sheets/checklist.csv`, `sheets/ai-governance-checklist.xlsx` and `docs/index.html`. GitHub Pages serves the web version from `/docs` on `main`.

## Framework mapping note

The ISO/IEC 42001, NIST AI RMF, EU AI Act and *Also maps to* references are indicative — they point you to the relevant clause, function, article or practice. Verify against the current official text before relying on them for compliance.

- EU AI Act application dates have shifted under the Digital Omnibus (Regulation (EU) 2026/1744): high-risk obligations apply from 2 Dec 2027 (Annex III) and 2 Aug 2028 (Annex I).
- **EN 18286:2026** was cited in the Official Journal on 14 Oct 2026 (Implementing Decision (EU) 2026/2274). It gives a presumption of conformity with the Art. 17 quality-management requirements it covers — not Art. 17(2)–(4). ISO/IEC 42001 is not a harmonised standard.
- **ISO/IEC 27090:2026** and **IEEE 2863-2026** are guidance, not certifiable standards.
- Australia's **Australian Standards for AI** were announced on 15 Jul 2026 with legislation expected in early 2027; until then, the voluntary Guidance for AI Adoption (AI6) applies.

The full, sourced crosswalk is in [ai-governance-compliance-as-code](https://github.com/caiotk/ai-governance-compliance-as-code).

## Licence

[CC BY 4.0](LICENSE) — free to share and adapt, with attribution to NexGuide.AI.

---

*Strong governance builds trust. Responsible AI drives sustainable innovation.*
