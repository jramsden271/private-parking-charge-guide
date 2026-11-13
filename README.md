# Private parking charge guide — a Claude skill

A [Claude](https://claude.ai) skill that helps people in **England & Wales** deal with a **private parking charge** (a "PCN" from a parking company), from the first ticket through to a court claim. Its guidance follows the advice regulars give on the MoneySavingExpert *Parking Tickets, Fines & Parking* forum.

> **Not legal advice.** This is general information based on publicly shared forum experience. It is **not official** and is **not affiliated with or endorsed by** MoneySavingExpert, the forum's members, the BPA, the IPC, POPLA, the IAS or any parking company. Any decision, and anything you send, is your own responsibility.

**Current version: 1.0** (13 November 2026) — see [CHANGELOG.md](CHANGELOG.md).

## What it does

- Works out what stage you're at from your letters (ticket, Notice to Keeper, debt collector, Letter of Claim, court claim, hearing, CCJ) and what to do next.
- Calculates your actual deadlines, with dates.
- Checks a Notice to Keeper against the Protection of Freedoms Act 2012 (paras 8 and 9).
- Helps draft appeals, complaints, Letter of Claim replies and the case-specific part of a court defence.
- Labels how confident each answer is, and tells you when to ask the forum instead.
- Doesn't push you to pay — but says clearly when paying is the right call.

**Not covered:** council or police tickets (try [FTLA](https://www.ftla.uk/)); only general, low-confidence information for Scotland and Northern Ireland.

## How to install

You need a Claude account on a plan that supports skills, with code execution turned on.

1. **Download** [`dist/private-parking-charge-guide-v1.0.zip`](dist/private-parking-charge-guide-v1.0.zip) (click the file, then the download button). Don't unzip it.
2. In Claude, go to **Settings → Capabilities** and make sure **Code execution and file creation** (sometimes called *Create and edit files*) is switched on.
3. Go to **Customize → Skills**, click **+**, then **Create skill → Upload a skill**, and choose the zip.
4. Check the skill is switched on.
5. Start a **new chat** and describe your situation, or upload a photo/scan of your letter (both sides of a Notice to Keeper). You can also ask for it by name: *"Use the private parking charge guide skill."*

Anthropic's help pages: [Use skills in Claude](https://support.claude.com/en/articles/12512180-use-skills-in-claude).

## Updating

Uploaded skills don't update themselves. When a new version is posted here, delete the old skill in **Customize → Skills** and upload the new zip.

## Please still use the forum

The skill is designed to get you to a sensible first draft quickly — not to replace the forum. Before sending anything important (especially a defence or witness statement), post it on the [MSE parking board](https://forums.moneysavingexpert.com/categories/parking-tickets-fines-parking) for a check, and **redact** your name, address, number plate, reference numbers and QR codes first. Write it in your own words: forum regulars are happy to help people who understand their own case.

## What's in the repo

```
private-parking-charge-guide/        the skill (this folder is what's zipped)
├── SKILL.md                         core rules, triage, stages A–D
└── references/
    ├── notices-and-codes.md         POFA checklists, relevant land, industry Code
    ├── court-claim-and-defence.md   claim form to mediation
    ├── hearing-and-ccj.md           witness statements, hearings, CCJs
    ├── whos-who.md                  operators, debt collectors, solicitors
    └── cases.md                     cases cited on the forum
dist/                                packaged zip(s) for download
```

## Licence

[CC BY 4.0](LICENSE): you can share and adapt this skill, including for your own version, as long as you credit it and link back here. Quoted legislation, Code of Practice extracts and judgments remain under their own terms.

## Feedback

Spotted something wrong or out of date? Open an issue on this repo.
