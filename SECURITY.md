# Security

AISLE is instructions only: twelve `SKILL.md` files that tell Claude how to
do a piece of account work. It has no code that runs, no connectors, and it
sends nothing anywhere. The risks it deals with are in what Claude reads and
writes while following it: client data, licensed data, and instructions
planted in email, files or web pages.

## Reporting a problem

If you find a way AISLE could lead Claude to expose confidential
information, follow a planted instruction, send or share something, or
handle redacted placeholders wrongly, please report it privately:

- On this repository's **Security** tab, choose **Report a vulnerability**.
- Or write to us through https://www.cortexa-consulting.ai/contact.

Please don't open a public issue for these, and don't include real client
data in any report. A made-up example that shows the behavior is enough.

Confirmed problems are fixed in a new release and noted in `CHANGELOG.md`.

## Supported versions

Only the latest release is supported. In Claude, the plugin's **Update**
button brings in the newest version.
