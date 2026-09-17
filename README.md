# Towards Standardized Benchmarking of SGRT Technologies

Project page for the poster and the talk at Novalis Circle 2026:
<https://ag-kollotzek.github.io/novalis-circle-2026/>

Static HTML and CSS served by GitHub Pages from `main:/`. No JavaScript, no web fonts, no requests to other sites.

## Structure

```
index.html        start page: title, authors, poster and talk, results, data flow, repositories, contact
poster/           detailed A0 poster (in preparation)
talk/             slides of the talk (added after the talk)
analysis/         analysis figures with captions; figures/ holds the PDFs, web images and thumbnails
qa/               yearly QA: tolerances, result per linac, reports and QA plot pages per year (qa/2026/)
assets/           stylesheet, logos, favicon, qr-code.svg
```

## Sources

- `analysis/figures/`: built with `paper_pipeline.py` of
  [surf-etds-analysis](https://github.com/AG-Kollotzek/surf-etds-analysis) at commit `2e9e1e8` with
  [surf-etds-data](https://github.com/AG-Kollotzek/surf-etds-data) `v1.0.0` and `SOURCE_DATE_EPOCH` set to the commit
  time; two builds gave byte-identical PDFs. The PNG/JPEG files are renderings of these PDFs.
- `qa/2026/`: public QA reports of the evaluation of 2026-08-10, built from
  [surf-etds-qa](https://github.com/AG-Kollotzek/surf-etds-qa) at commit `55065d1`; the QA plot pages are the files
  `data/process/L*/single_angle/L*_{RT,32}_Couch0_2026-08-10_QA.pdf` of that commit, the PNGs are renderings of them.
  Personnel appear as role codes only.

## Local preview

```bash
python3 -m http.server 8765
```

## Licence

Text, figures, reports and slides: CC BY 4.0. Code of this site (HTML, CSS): MIT.
