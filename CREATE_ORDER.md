# CREATE_ORDER.md

Creation order and sidebar groups for the Timber + Love Grok Bot company (24 bots).
All schedules use timezone **America/Boise**.

Source: Operating Plan Section 9.1 Activation order, Section 2 Org Chart (Amendment A20), and roster order in Section 3.

## Sidebar groups (department folders)

Create these sidebar groups, then place bots as listed.

| Sidebar group | Bots |
|---------------|------|
| CEO | Hank |
| Operations and Governance | Larry (head), Mira, Ivy, Maya |
| Finance and Compliance | Finn (head), Nora, Cora, Remy |
| Design-Build Delivery | Walt (head), Cole, Dana |
| Marketing and Growth | Omar (head), Quinn, Sage, Zoe, Priya |
| Technology and Design | Kai (head), Ada, Sam |
| Portfolio Entities | Rex (head), Stella |
| Quality and Insight | Vera, Dash (independent; report to Hank) |

Reporting rule: only the six department heads (Larry, Finn, Walt, Omar, Kai, Rex) plus Vera and Dash talk to Hank. Hank talks only to Jared.

## Wave activation order (create in this sequence)

Compliance, access, and governance first; revenue-facing bots after their data and approval paths exist.

### Wave 0 — Foundations (days 0–3)

Nothing runs without the queue, registry, audit log, Hank's Grok chat, verified connections, and the run-gate.

| Order | File | Bot | Notes |
|------:|------|-----|-------|
| 1 | `bots/05-sam.md` | Sam | Connections, vault, Login Broker |
| 2 | `bots/06-kai.md` | Kai | Queue and run-gate service (partial) |
| 3 | `bots/03-mira.md` | Mira | Registry and memory |
| 4 | `bots/02-larry.md` | Larry | Mission Control and scheduler inventory |
| 5 | `bots/01-hank.md` | Hank | CEO; Jared's only contact |
| 6 | `bots/20-vera.md` | Vera | Certification only in Wave 0 |

### Wave 1 — Protect (days 3–7)

Licensure clock, books visibility, and inbox control remove the biggest risks first.

| Order | File | Bot | Notes |
|------:|------|-----|-------|
| 7 | `bots/08-cora.md` | Cora | Compliance and licensing |
| 8 | `bots/07-nora.md` | Nora | Read-only books first |
| 9 | `bots/09-ivy.md` | Ivy | Executive inbox and admin |
| 10 | `bots/24-remy.md` | Remy | Receipts and invoice intake |

### Wave 2 — Revenue core (days 7–14)

Leads, delivery, and estimating use the systems of record. Vera and Dash start once there is work and data to verify. Finn goes live only after Nora's books are readable and the eight finance go-live tests in Section 3.23 pass.

| Order | File | Bot | Notes |
|------:|------|-----|-------|
| 11 | `bots/12-omar.md` | Omar | Sales and leads |
| 12 | `bots/10-walt.md` | Walt | Field ops, subs, vendors |
| 13 | `bots/11-cole.md` | Cole | Estimating and pricing |
| 14 | `bots/23-dana.md` | Dana | Design and selections (Design-Build with Walt/Cole; required for delivery) |
| 15 | `bots/04-maya.md` | Maya | Strategic research |
| 16 | `bots/22-finn.md` | Finn | Prepare-only at L1 until go-live tests pass |
| 17 | `bots/20-vera.md` | Vera | Full verification duties begin |
| 18 | `bots/21-dash.md` | Dash | Analytics and attribution |

### Wave 3 — Growth engines (days 14–21)

Paid and organic growth start once tracking and review gates are proven.

| Order | File | Bot | Notes |
|------:|------|-----|-------|
| 19 | `bots/14-quinn.md` | Quinn | Paid media |
| 20 | `bots/13-sage.md` | Sage | Search visibility |
| 21 | `bots/17-ada.md` | Ada | UI, UX, CRO |
| 22 | `bots/06-kai.md` | Kai | Full builds (second activation) |

### Wave 4 — Brand and portfolio (days 21–30)

Public-facing actions begin after Cora and Ada gates have run clean.

| Order | File | Bot | Notes |
|------:|------|-----|-------|
| 23 | `bots/15-zoe.md` | Zoe | Moderation first; Pinterest pins after a clean week |
| 24 | `bots/16-priya.md` | Priya | Content and copy |
| 25 | `bots/19-rex.md` | Rex | Realty and BMH deal flow |
| 26 | `bots/18-stella.md` | Stella | Stay With Us operations |

## Roster numbering (files on disk)

Consistent with plan Section 3 roster order (Hank = 01, then specialists):

| # | File | Bot |
|--:|------|-----|
| 01 | `bots/01-hank.md` | Hank |
| 02 | `bots/02-larry.md` | Larry |
| 03 | `bots/03-mira.md` | Mira |
| 04 | `bots/04-maya.md` | Maya |
| 05 | `bots/05-sam.md` | Sam |
| 06 | `bots/06-kai.md` | Kai |
| 07 | `bots/07-nora.md` | Nora |
| 08 | `bots/08-cora.md` | Cora |
| 09 | `bots/09-ivy.md` | Ivy |
| 10 | `bots/10-walt.md` | Walt |
| 11 | `bots/11-cole.md` | Cole |
| 12 | `bots/12-omar.md` | Omar |
| 13 | `bots/13-sage.md` | Sage |
| 14 | `bots/14-quinn.md` | Quinn |
| 15 | `bots/15-zoe.md` | Zoe |
| 16 | `bots/16-priya.md` | Priya |
| 17 | `bots/17-ada.md` | Ada |
| 18 | `bots/18-stella.md` | Stella |
| 19 | `bots/19-rex.md` | Rex |
| 20 | `bots/20-vera.md` | Vera |
| 21 | `bots/21-dash.md` | Dash |
| 22 | `bots/22-finn.md` | Finn |
| 23 | `bots/23-dana.md` | Dana |
| 24 | `bots/24-remy.md` | Remy |

## Paste rule

Each `bots/NN-<name>.md` **Full system prompt** section already includes the Shared Preamble merged with the role prompt (from `prompts/ready-to-paste/<name>.txt`). Paste that section into the bot's instructions in Grok Bot. Do not create bots via API from this pack.
