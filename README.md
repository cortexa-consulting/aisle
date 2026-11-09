# AISLE

**Accounts · Insights · Safeguards · Launches and pitches · Execution.**
Twelve Claude skills for account teams that sell through retail, in one
plugin from [Cortexa Consulting](https://www.cortexa-consulting.ai).

AISLE adds instructions only. It has no connectors and reaches nothing
outside Claude. Each skill is a folder with one `SKILL.md` you can open and
read before you turn it on.

## The skills

| Skill | What it does |
| --- | --- |
| `inbox-triage` | Sorts a batch of email into Urgent, Needs reply, FYI and Suspicious, and drafts replies as files. Never sends. Treats email text as data, not instructions. |
| `sell-through-recap` | Checks a retail sell-through export first (duplicates, odd prices, returns, out-of-stocks, gaps), builds the retailer-by-week grid, and drafts the recap. |
| `excel-grid` | Builds Excel workbooks people can trust: real formulas, one table per sheet, validation where people type, and a README tab. |
| `client-deck` | Builds PowerPoint decks with the answer up front, one idea per slide, sentence headlines, a source on every number, and speaker notes. |
| `sales-dashboard` | Builds a pipeline dashboard from a CRM export, using only the columns it needs and reconciled to the export. |
| `store-visit-report` | Turns store visit notes into a report with an owned action for every issue, and separate client-facing and internal sections. |
| `redaction-partner` | Keeps placeholders such as `[COMPANY-01]` exactly as written, never guesses what they stand for, and flags details that slipped through. |
| `new-account` | Sets up the folders for a new client account or engagement, and never overwrites one that exists. |
| `retailer-meeting-prep` | Prepares a one-page brief for a buyer or retailer meeting from the account's files. |
| `weekly-client-update` | Drafts the weekly update email from the account's memory and this week's files. Saves a draft; never sends. |
| `wrap-up` | Logs where the work stands in the account's `memory.md`, with no client figures or confidential details. |
| `new-workflow` | Turns a job you repeat (a quarterly review, a monthly recap) into numbered stages with a check between each, and runs one stage at a time. |

## Install

In Claude (Desktop or claude.ai), **Customize → Plugins → Add**:

- **Add marketplace** and enter `cortexa-consulting/aisle`, then **Sync**,
  then **Discover → AISLE → Add**. Its Update button brings in new versions.
- Or **Upload plugin** and choose this repository's ZIP
  (**Code → Download ZIP**), as downloaded.

In Claude Code: `/plugin marketplace add cortexa-consulting/aisle`, then
`/plugin install cortexa-aisle@cortexa`.

To run a skill yourself, type `/` in the message box and choose it
(`cortexa-aisle:inbox-triage`). Otherwise each one starts when your request fits
its description.

## The workspace the skills expect

The skills work on their own, and fit this folder layout when you have it
(the **new-account** skill sets up the account folders):

```
Your workspace/
  about-me/                     about-me.md, writing-rules.md, memory.md
  projects/<account>/           brief.md (Shared and Mine sections), memory.md
    reference/                  brand guide, glossary, templates the team may see
    <engagement>/               brief.md and memory.md for one piece of work
    workflows/<workflow>/       numbered stages, one CONTRACT.md each
  outputs/<account>/            finished work; drafts/ for unsent drafts
```

When the work is for an account, a skill reads that account's brief, memory
and reference files first, writes in your voice from `writing-rules.md`,
saves to `outputs/<account>/` unless you name a place, and offers a line for
the account's memory instead of writing one. Any part that isn't there is
skipped.

## Keeping sensitive information safe

- Follow your company's AI policy first.
- Give Claude the minimum the task needs. Redact names and contact details
  before you paste; the **redaction-partner** skill keeps the placeholders
  intact.
- A folder you connect is a folder Claude can read. Keep originals of
  sensitive files outside it.
- Licensed and partner data (retail panels, portal extracts) often limits
  where it can be processed. Check before you upload.
- Email and web pages can carry instructions aimed at AI. AISLE treats them
  as data, never as orders.
- You review before anything ships. No skill sends, posts or shares.

## License and support

MIT. Questions or problems: [cortexa-consulting.ai/contact](https://www.cortexa-consulting.ai/contact).
