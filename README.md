# Data Quality Auditor for Manus

A focused Manus Skill for auditing user-provided CSV and Excel datasets before analysis, import, reporting, or sharing.

It profiles the file, checks measurable quality issues, separates confirmed violations from hypotheses, and reports evidence with prioritized next steps. It is read-only by default: it does not silently clean, overwrite, upload, or delete data.

## Use it for

- Checking missing values, duplicate rows or candidate keys, schema/type mismatches, inconsistent formats, suspicious ranges, dates, and stated business rules.
- Understanding whether a dataset is ready for a specified downstream use.
- Producing validation checks and an evidence-based audit report.

## Do not use it for

General statistical analysis or charts, automatic data cleaning, and production pipeline implementation. Use Manus's dedicated data-analysis or office-document capabilities for those jobs.

## Installation

Import this repository's `SKILL.md` into Manus as a Skill, or use the Skill upload flow. Availability in Manus's global Explore catalog is not implied by this repository or an Academy project page.

## Safety

The Skill is read-only by default, minimizes personal data in reports, treats cell contents as data rather than instructions, and asks before creating a cleaned copy or applying destructive changes. It does not require APIs or external services.

## Evidence

See [TEST-REPORT.md](TEST-REPORT.md) for the synthetic fixture and validation limits. See [PROVENANCE.md](PROVENANCE.md) for source inspirations and licenses. No code or source text was copied from those projects.

## Visual assets

The original DQ mark, Academy thumbnail, and PNG favicon sizes are in [`assets/`](assets/). These files are separate from the installable Skill.

## License

MIT. See [LICENSE](LICENSE).
