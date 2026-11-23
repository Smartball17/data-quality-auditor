# Test report — data-quality-auditor v0.1.0

**Status:** structurally validated; synthetic checks executed; activation and real Manus use not verified.

## Synthetic CSV fixture

A five-row, six-column fixture was created specifically for this test. It contained one extra row with a duplicate candidate ID, one blank email, one `TBD` sentinel, one negative amount, one malformed date, one country outside the declared set, and one status outside the declared set. A standard-library CSV check reported each seeded issue exactly once and preserved the original data. The example contact value was shown only in masked form.

**Acceptance:** pass for these known examples. This demonstrates detection of the seeded cases only, not general statistical accuracy.

## Boundary case

A CSV with headers but no records was recognized as empty. The procedure requires reporting that no data can be profiled and forbids inventing a baseline or quality score.

**Acceptance:** pass by execution of the empty-row check and manual review of reporting instructions.

## Non-trigger case

A request to chart monthly revenue from an already validated dataset should route to Manus `data-analysis`, not this auditor.

**Acceptance:** pass by manual trigger and handoff review.

## Privacy, permissions, and cost

Manual review confirms the Skill masks personal examples, keeps the source unchanged, makes no external API/service calls, and asks before cleaning, deleting, or producing a modified copy. No real personal data or paid services were used. Manus credit usage was not measured.

## Validation limits

The official `quick_validate.py` reported `Skill is valid!`. No automatic activation test, real user-file audit, complex workbook/multi-sheet test, or global Explore catalog check was performed. The latter remains unverified.
