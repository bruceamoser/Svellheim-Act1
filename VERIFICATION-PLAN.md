# Act 1 — Restore the Flame: Verification Plan

> **Source of Truth**: `Era-of-Embers/campaign/docs/04-Campaign/01-Restore-the-Flame/Act-1/`
> **Target**: `Svellheim-Act1/data/`
>
> **Key Principle**: The director will NOT have access to the campaign adocs during play.
> The Foundry journal entries are the **runtime game documents** — they must be
> complete, self-sufficient references for running each beat at the table.
> Nothing the director needs to know can be missing from the journals.

---

## Campaign Doc → Journal Page Mapping

| # | Campaign Doc (Source of Truth) | Journal Page | Status |
|---|-------------------------------|-------------|--------|
| 0 | `00-Act-1-Overview.adoc` | *(no journal page — overview only)* | — |
| 1 | `01-The-Konungs-ferd.adoc` | Beat 1 — The Konungs-ferð (The King's Call) | ⬜ |
| 2 | `02-The-Road-to-Hrafnborg.adoc` | Beat 2 — The Road to Hrafnborg | ⬜ |
| 3 | `03-The-Quiet-Summons.adoc` | Beat 3 — The Quiet Summons | ⬜ |
| 4a | `04a-The-Coastal-Road.adoc` | Beat 4 — The Road to Stairwatch *(combined 4a+4b)* | ⬜ |
| 4b | `04b-The-Mountain-Road.adoc` | Beat 4 — The Road to Stairwatch *(combined 4a+4b)* | ⬜ |
| 5 | `05-Finding-Lew.adoc` | Beat 5 — Finding Lew | ⬜ |
| 6 | `06-The-Great-Green.adoc` | Beat 6 — The Great Green *(combined 6+6a+6b)* | ⬜ |
| 6a | `06a-The-Ashen-Woods.adoc` | Beat 6 — The Great Green *(sub-beat)* | ⬜ |
| 6b | `06b-The-Bone-Fields.adoc` | Beat 6 — The Great Green *(sub-beat)* | ⬜ |
| 7 | `07-The-Reluctant-Hearth.adoc` | Beat 7 — The Reluctant Hearth | ⬜ |
| 8 | `08-The-Long-Road-Home.adoc` | Beat 8 — The Long Road Home | ⬜ |
| 9 | `09-The-Siege-of-Hrafnborg.adoc` | Beat 9 — The Siege of Hrafnborg | ⬜ |

## Campaign Doc → Montage Test Mapping

| Campaign Doc | Montage Test Data File | Status |
|-------------|----------------------|--------|
| `montages-act1.adoc` | `beat-02-road-to-hrafnborg.json` | ⬜ |
| `montages-act1.adoc` | `beat-04-montage-1-coastal-road.json` | ⬜ |
| `montages-act1.adoc` | `beat-04-montage-2-titans-stair.json` | ⬜ |
| `montages-act1.adoc` | `beat-06-great-green-ashen-woods.json` | ⬜ |
| `montages-act1.adoc` | `beat-06-great-green-bone-fields.json` | ⬜ |
| `montages-act1.adoc` | `beat-08-long-road-home.json` | ⬜ |
| `montages-act1.adoc` | `beat-09-breaking-the-siege-line.json` | ⬜ |

## Campaign Doc → Negotiation Test Mapping

| Campaign Doc | Negotiation Test Data File | Status |
|-------------|--------------------------|--------|
| `negotiations-act1.adoc` | `beat-04-negotiation-greypass.json` | ⬜ |
| `negotiations-act1.adoc` | `beat-05-negotiation-lew-tosferd.json` | ⬜ |
| `negotiations-act1.adoc` | `beat-05-negotiation-rath.json` | ⬜ |
| `negotiations-act1.adoc` | `beat-07-negotiation-kaelen.json` | ⬜ |
| `negotiations-act1.adoc` | `beat-08-negotiation-thyra-greyfen.json` | ⬜ |

## Player Handouts

| Campaign Doc | Player Journal | Status |
|-------------|---------------|--------|
| Various beat docs → player-facing sections | `Act-1-Restore-the-Flame-Player-Handouts.journal.json` | ⬜ |

## Supporting Reference Docs

| Campaign Doc | Purpose |
|-------------|---------|
| `encounters-act1.adoc` | Encounter stat blocks / compositions |
| `items-act1.adoc` | Item definitions → cross-ref with Svellheim-Entities |
| `monsters-act1.adoc` | Monster definitions → cross-ref with Svellheim-Entities |
| `npcs-act1.adoc` | NPC definitions → cross-ref with Svellheim-Entities |
| `required-art-act1.adoc` | Art asset checklist |

---

## Verification Rules

### Purpose
The campaign adocs are the source of truth for **what** content the journals must contain.
The Foundry journals are the **runtime documents** the director uses at the table — they
must be complete enough to run each beat without referencing the adocs.

### Content Completeness
1. **Every beat's journal page must contain everything the director needs to run it:**
   - Read-aloud / narrative text (exact wording from campaign doc)
   - GM notes, pacing guidance, and tone cues
   - Encounter composition and when to trigger it
   - NPC motivations, dialogue cues, and key information
   - Loot and rewards
   - Transition instructions to the next beat
2. **Narrative text** — read-aloud text, GM notes, transitions must match campaign doc wording exactly.
3. **No missing information** — if the campaign doc says it, the journal must have it.

### Entity References
4. **Entities (monsters, NPCs, items)** — reference via `@UUID[Item.xxx]{Name}` links to the Svellheim-Entities module. Do NOT duplicate full stat blocks or item descriptions inline. The director clicks the link to open the entity in Foundry.
5. **Context around references** — the journal MUST still contain enough context to know *when* and *why* to use an entity (e.g. "2× @UUID[...]{Draugr Thrall} + 1× @UUID[...]{Barrow-Warden} emerge from the barrows when the party disturbs the cairn").

### Process
6. **One beat at a time** — read campaign doc, then journal page, compare, fix.
7. **Montage/Negotiation data files** — verify stats (SL, FL, difficulty, motivations, arguments, twists) match campaign docs.

---

## Progress Log

| Date | Beat | Action | Notes |
|------|------|--------|-------|
| | | | |
