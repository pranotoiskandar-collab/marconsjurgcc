# Marine conservation jurisprudence in the GCC

Research data for a regional study of marine and coastal conservation law in the six Gulf Cooperation Council states: Bahrain, Kuwait, Oman, Qatar, Saudi Arabia and the United Arab Emirates.

Collected on 18 November 2026. Most records were found through FAOLEX, UNEP LEAP and ECOLEX, and still need checking against the official Arabic gazettes. The `verification` column says what is still to check for each row.

## Files

| File | Contents |
| --- | --- |
| `data/national_instruments.csv` | 81 national and emirate-level laws, decrees, resolutions and reserve designations on marine and coastal protection and fisheries |
| `data/regional_instruments.csv` | ROPME (Kuwait Convention), PERSGA (Jeddah Convention) and GCC instruments |
| `data/treaty_status.csv` | Each state's status in UNCLOS, BBNJ, Ramsar, CMS, Ballast Water, MARPOL Annex VI, ROPME and PERSGA |
| `data/stance_records.csv` | Filings and statements by GCC states in international courts (ICJ, ITLOS) |

## Columns in `national_instruments.csv`

- `state`, `level` (federal, national or emirate), `year`
- `instrument`, `issuer`, `subject`
- `source_type`: where the record was found (official portal, FAOLEX/LEAP record, news report and so on)
- `url`: link to the text or record
- `verification`: what still needs checking

## Caveats

- English texts are mostly unofficial translations; the Arabic text governs.
- News reports are used only where no legal text was found online, and are flagged.
- Treaty status for Ballast Water and some MARPOL annexes comes from a secondary summary and should be checked against IMO status lists.

## Arabic sources (added 2026-11-18)

- `data/arabic_sources.csv` lists 22 key instruments with Arabic titles, Hijri and Gregorian dates, gazette details and status. 11 of them have been checked against Arabic legal portals. The other 11 are left for the local colleague to check.
- `data/arabic_books.csv` lists 19 Arabic books, theses and articles. They cover the region, single countries, international law written in Arabic, and Islamic law.
- `ARABIC_CHECK_GUIDE.md` gives plain-English instructions for the colleague.

## Secondary literature (added 2026-11-19)

- `data/secondary_literature.csv` lists English commentary used as starting points, beginning with Stagstrup's 2025 EJIL:Talk! post on desalination discharges in the Gulf.

## Court cases (added 2026-11-19)

`data/court_cases.csv` lists 21 judgments, awards and court records to use as sources: 9 international (ICJ, ITLOS, UN Compensation Commission, and the early oil arbitrations), 11 national (UAE, Bahrain, Qatar, Oman) and 1 historic customary court (Bahrain's pearling court).

Columns: `id`, `scope`, `state`, `court`, `date`, `case`, `parties`, `citation`, `link`, `arabic_title`, `issue`, `outcome`, `verified` (yes, partly or no), `how_checked`, `why_it_matters`, `paper_section` (section of the working paper that could use it), `colleague_check` (what the Arabic-speaking colleague could check).

What "verified" means:
- **yes**: the judgment or official record was read.
- **partly**: the case exists, but some details come from a news report, a catalogue entry or memory and still need checking against the full text.
- **no**: only a hearing report was found; the outcome is unknown.

Gaps still open:
- **Saudi Arabia and Kuwait**: no national marine judgment was found online. Saudi courts are themselves Sharia courts, so any judgment there would also answer the Sharia question. The Saudi Ministry of Justice judgments portal (sjp.moj.gov.sa) and the Board of Grievances collections need searching in Arabic, ideally by the colleague.
- **Sharia court rulings on the sea**: none found beyond the Saudi point above and the old pearling court records.
- **Official portals**: the UAE Ministry of Justice portal blocked automated reading, and Qatar's Al Meezan search gave no marine judgments. A manual Arabic search may find more.
- Most national rows rest on news reports. Case numbers and full texts should be found where possible.
