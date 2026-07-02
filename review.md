# Project Review: WSKZ2025 S17 – Module A – Online Classifieds Promo Landing Site

## Summary

The project task is largely standardized and structurally compliant with the MITS guide. `project-description.md`, `metadata.json`, `README.md`, and `marking/marking-scheme.json` are present and well-formed. Mark totals are consistent (20 points across description and JSON).

Two issues should be resolved before integration: a **missing asset file** referenced in the project description, and **marking-scheme criteria in Russian** for an English-language task. Several marking-scheme requirements (sticky header, footer details) are not documented in `project-description.md`.

---

## Issues Found

### Critical Issues

1. **Missing asset file** — `project-description.md` references `assets/texts/seller-price-list-faq.txt` (For Seller – Price List FAQ section), but this file does not exist in `assets/texts/`. The original task required it. Either add the missing file or confirm an alternative source (e.g. reuse `seller-faq.txt`).

### Important Issues

1. **Marking scheme language mismatch** — All aspect descriptions and judgement score descriptions in `marking/marking-scheme.json` are in Russian, while `metadata.json` declares `"languages": ["EN"]` and the project description is in English. Assessors and international users may need an English translation.

2. **Project description vs marking scheme gaps** — The marking scheme tests requirements not stated in `project-description.md`:
   - Sticky header on all pages (0.25 marks)
   - Footer: second-level navigation menu (0.25 marks)
   - Footer: copyright with current year (0.25 marks)
   - Footer: link to policy page (0.25 marks)
   - Competitor README must document changing the `data-type` attribute (marking scheme), but the project description says changing **link targets** of `Publish` and `View` buttons

3. **Page count ambiguity** — General Description states "four logically connected pages" but Requirements define six page groups (Home, For Seller, For Seller – Price List, For Buyer, Contacts, Policy). This is inherited from the original task; clarify whether subpages/sections count toward the four pages or update the wording.

4. **Repository naming inconsistency** — `metadata.json` uses `WSKZ2025` in `name` but `url` points to `s17-wsk2025-s17-module-a` (without the "z"). Consider aligning repo name and URL when publishing.

### Minor Issues

1. **`wsosSections` includes unused sections** — Sections 1, 4, and 5 are listed in `marking-scheme.json` but have 0 aspect marks. Harmless but could be trimmed to sections 2 and 3 only for clarity.

2. **Mixed-language sub-criterion names** — Some marking sub-criteria mix English and Russian (e.g. "Seller page - Общий дизайн"). Consider consistent English naming.

3. **`.DS_Store` in assets** — macOS metadata file present under `assets/images/`. Safe to remove.

4. **Tag conventions** — Reference projects use `"design implementation"` as a tag; this project uses `"design"`. Optional alignment with repository conventions.

5. **No `status` field in metadata** — Other published tasks (e.g. Module C) include `"status": "published"`. Add when ready for collection upload.

---

## Content Quality Issues

### Duplicate Content

- **README vs metadata description** — Both describe the classifieds landing site in similar terms. Acceptable overlap; README is appropriately shorter.
- **General Description vs Requirements** — Website-wide rules (no frameworks, responsive layout, semantic markup, etc.) appear only in General Description, not repeated in Requirements. No problematic duplication found.

### Language and Clarity

- Project description prose is clear, grammatically correct, and consistent in English.
- Terminology is mostly consistent (`For Seller`, `For Buyer`, `Publish`, `View`).
- "For Seller – Price List" (current) vs original "For Seller – Advantages Page" — aligns with navigation label "Paid Services" and marking scheme name "Seller price list page"; acceptable but worth noting for traceability.

---

## Compliance Checklist

- [x] README.md structure
- [x] project-description.md header hierarchy
- [x] All required sections present (Competition time, Introduction, General Description, Requirements, Assessment, Mark distribution)
- [x] metadata.json valid and complete
- [x] marking-scheme.json valid JSON structure
- [x] Mark distribution aligns with marking scheme (20 total; WSOS 2: 0.5, WSOS 3: 19.5)
- [ ] Assets properly organized — **missing `seller-price-list-faq.txt`**
- [x] No broken internal markdown links
- [x] No unnecessary duplicate content
- [x] Clear and grammatically correct language (project description and README)
- [x] All other referenced asset paths exist (`assets/texts/*.txt`, `assets/map.png`)

---

## Recommendations

1. **Add `assets/texts/seller-price-list-faq.txt`** (or obtain from original competition materials) before publishing.
2. **Translate marking scheme to English** to match task language, or add `"RU"` to `metadata.json` languages if bilingual assessment is intended.
3. **Align project description with marking scheme** — add sticky header, footer requirements (copyright, policy link, second-level menu), and clarify README instructions (`data-type` vs link targets).
4. **Clarify the "four pages" statement** in General Description to avoid competitor confusion.
5. **Clean up working files** after fixes (see below).

---

## Proposed Clean-up (requires confirmation)

The following working files can be removed once issues above are resolved:

| File | Reason |
|------|--------|
| `projectplan.md` | Working plan from standardization process |
| `marking/marking-scheme.xlsx` | Converted to `marking-scheme.json` |
| `.claude/skills/mits-project-task-updater/scripts/xlsx-to-json/marking-scheme-raw.json` | Converter temporary output |
| `.claude/skills/mits-project-task-updater/scripts/xlsx-to-json/marking-scheme-structured.json` | Converter temporary output |
| `.claude/skills/mits-project-task-updater/scripts/xlsx-to-json/new-marking-scheme.json` | Converter temporary output |
| `assets/images/.DS_Store` | macOS metadata artifact |

**Confirm if you want these files deleted.**
