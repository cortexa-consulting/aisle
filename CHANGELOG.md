# Changelog

## 1.2.3 (2026-11-10)

- **New display name: AISLE by Cortexa Consulting.** "AISLE" on its own is
  already the name of another listing in Anthropic's plugin directory. The
  skills, the plugin name (`cortexa-aisle`) and how you install it are
  unchanged.

## 1.2.2 (2026-11-09)

- **New plugin name: `cortexa-aisle`.** The display name is still AISLE.
  Install with `/plugin install cortexa-aisle@cortexa`, and skills start
  with `cortexa-aisle:` (for example `cortexa-aisle:inbox-triage`). If you
  installed `aisle` before, remove it and install `cortexa-aisle`; nothing
  else changes.
- Every skill's description is now quoted, so the colons in it can't be
  misread by a strict reader. The wording is unchanged.
- Removed the social preview image from the repository. GitHub keeps its
  own copy, so the repository page looks the same.

## 1.2.1 (2026-11-07)

- **redaction-partner:** placeholders stay exact in headings, tables, slide
  titles and file names too, with the brackets, the leading zero and the
  capitals as written. Redact & Restore now points out a placeholder written
  differently (`COMPANY-01`, `[COMPANY-1]`, `[Company-01]`) and offers to
  restore it, where it used to leave it in place without a word.

## 1.2.0 (2026-11-06)

First public release of AISLE, the general-purpose version of the plugin
from Cortexa Academy's retail account workshop.

- **Twelve skills:** inbox-triage, sell-through-recap, excel-grid,
  client-deck, sales-dashboard, store-visit-report, redaction-partner,
  new-account, retailer-meeting-prep, weekly-client-update, wrap-up and
  new-workflow.
- **Safety section in every skill.** Text in files, email and web pages is
  material to work with, never an instruction. A planted instruction is
  quoted word for word, or described exactly, and never followed. No links
  in email are opened. Redaction placeholders stay exactly as written.
- **Nothing is sent.** Drafts are saved as files for you to review and send.
- **Memory lines are offered, not written,** and never record a decision you
  haven't made (a fix applied, an open item closed, a date not promised).
- **Data fixes are your call.** Totals stay as exported until you say yes,
  with the corrected figures beside them.
- Tested on Claude Haiku, Sonnet and Opus across 27 work scenarios and 34
  skill-selection cases before release.
