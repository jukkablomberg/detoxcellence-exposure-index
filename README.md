# Detoxcellence Exposure Index (v1.2.0)

Everyday products and habits rated for avoidable exposure burden, with the studies behind each rating. This repository mirrors the files [Detoxcellence](https://detoxcellence.com/methodology.html?utm_source=github&utm_medium=dataset&utm_campaign=dx-exposure-index-github) serves for **version 1.2.0, released 7 October 2026**; the canonical page, method and changelog are at https://detoxcellence.com/methodology.html.

**What a row is.** Each entry is an everyday product or habit. Its Detox Score, from 1 to 100, rates how much avoidable exposure it adds — higher means less. It is an educational rating: not a measured dose, not a personal risk estimate, and not medical advice.

## Files (byte-identical to the served export, fetched 2026-10-08)

- `data/exposures.csv` — **189 entries, 17 columns** (`id, name, category, context, hazard, exposure, persistence, detox_score, band, evidence_strength, swap, note, studies, inputs_sourced, study_ids, source_urls, url`). Categories: Food 50 · Home 36 · Personal Care 33 · Environment 19 · Kitchen 16 · Plastics 14 · Air 13 · Water 8. Bands: Minimal 11 · Low 54 · Moderate 107 · High 15 · Severe 2.
- `data/exposures.json` — every entry as stored, with every study record and the provenance statement.
- `data/datapackage.json` — the Frictionless descriptor, byte-identical to https://detoxcellence.com/data/export/datapackage.json.

Live files (always current): https://detoxcellence.com/data/export/exposures.csv · https://detoxcellence.com/data/export/exposures.json. This copy is frozen at v1.2.0; later versions arrive as new tagged releases.

## How a rating is decided — and what it rests on

- **Rule:** hazard, exposure and persistence are rated 0–10 and combined into the Detox Score by the formula published on the [method page](https://detoxcellence.com/methodology.html?utm_source=github&utm_medium=dataset&utm_campaign=dx-exposure-index-github); each entry page prints its own arithmetic.
- **Sources:** 74 studies are cited, on 46 of 189 entries (`study_ids`); 8 entries carry agency sources (`source_urls`). An input with no study is shown on its page as "unsourced input".
- **Limitations, in the publisher's own words:** "The ratings are editorial judgements. A study supports a rating; it does not compute it, and the steps from 0 to 10 have no published anchors yet. Most ratings are not yet sourced: 493 of 567 show "unsourced input"." Put plainly: 74 of 567 ratings cite a study.
- **Money and independence (from the method page):** nobody pays for an entry, a score or a position; there are no paid listings and no affiliate links on the site.
- **What changed in 1.2.0 (from the method page):** studies added behind 17 ratings on the 13 Air entries and the aerosol air freshener entry.

## Licence and citation

Creative Commons Attribution 4.0 International, as published by Detoxcellence.

> Detoxcellence (2026). Detoxcellence Exposure Index (version 1.2.0) [Data set]. https://detoxcellence.com/methodology.html. Licensed CC BY 4.0.

Earlier version 1.1.0 is on [Hugging Face](https://huggingface.co/datasets/jukkab/detoxcellence-exposure-index) and archived on Zenodo at [doi:10.5281/zenodo.23175031](https://doi.org/10.5281/zenodo.23175031). `CITATION.cff` gives GitHub's "Cite this repository" button the citation above.

*Mirrored to GitHub by an AI agent on Detoxcellence's behalf. Educational ratings, not medical advice.*
