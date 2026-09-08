# Online Ecosystem Ethics Framework (OEEF)

**A framework for assessing the ethics, social impact and environmental impact of online
ecosystems — and three scorecards built with it.**

Published by [Hive IT](https://hiveit.co.uk), Sheffield. Live at
**[scorecards.hiveit.ai](https://scorecards.hiveit.ai/)**.

Framework **version 4.0**. Everything here is free to read, share and adapt with credit —
see [Licence](#licence).

---

## What this is

Procurement and design decisions about digital technology are made every day on incomplete
information: which host, which framework, which AI provider. Carbon, water, labour conditions,
military supply, lobbying and data governance rarely reach the table, because the evidence is
scattered and hard to compare.

OEEF is an attempt to make that evidence comparable and checkable. It has two halves:

- **The framework** — the method. Thirteen criteria across three pillars, a 0–4 scale, an
  explicit separation of *how well something performs* from *how good the evidence is*, and a
  stated rule for every value judgement in the scoring. It is written so that a third party can
  build a conforming scorecard for a domain we have never covered.
- **The scorecards** — the method applied, to 126 real entries, with a cited source behind
  each score and a note recording what was searched.

On evidence coverage, the honest position: the AI and cloud scorecards are sourced on **every
criterion for every entry**. The tech-stack scorecard has one documented gap — criterion 7
(workers and labour conditions) for **8 of its 92 entries**, all private companies with no
reachable public register or filing. Those eight say so in the note rather than carrying a
number nobody could check.

It is not a certification scheme, a ranking, or a substitute for your own due diligence. It is
a starting point that shows its working, so you can disagree with it precisely.

---

## The scorecards

| Scorecard             | Covers                                                       |                                                   |
| --------------------- | ------------------------------------------------------------ | ------------------------------------------------- |
| **AI providers**      | 20 AI providers and model families — frontier hosted models, open-weight families, fully open research models | [Open](https://scorecards.hiveit.ai/ai.html)      |
| **Cloud and hosting** | 14 hosting and cloud providers — hyperscalers, independent European and UK hosts, and hosts built on someone else's cloud | [Open](https://scorecards.hiveit.ai/hosting.html) |
| **Tech stack**        | 92 technologies — frameworks, libraries, runtimes, databases, CMSs, infrastructure and hosted services, with a stack builder and an environmental impact calculator | [Open](https://scorecards.hiveit.ai/stack.html)   |

Each page runs entirely in the browser. There is no account and nothing to install; the
assessment happens on your machine and no record of it is sent anywhere. The only thing any
page loads from another host is an anonymous page-view counter — everything else, including the
fonts and the scoring engine, is served from this site. Links to sources go out to the
publishers we cite, and are followed only if you click them.

## The framework and the methodologies

The framework holds what is universal. Each scorecard publishes its own methodology document
holding the domain-specific bindings — which criteria apply to which kinds of entity, in which
state, and what counts as a competent search. The framework requires this: without it, a reader
cannot tell where a tool's judgements came from.

| Document                          | What it covers                                               |                                                              |
| --------------------------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| **Framework v4.0**                | The method: the thirteen criteria, the scoring logic, the applicability rules, worked examples | [Read](https://scorecards.hiveit.ai/guide-framework.html) · [Markdown source](https://scorecards.hiveit.ai/ethics-framework.md) |
| **AI scorecard methodology**      | Entity taxonomy, applicability matrix, constants, search standards for the AI domain | [Read](https://scorecards.hiveit.ai/guide-methodology-ai-ethics-scorecard.html) |
| **Cloud and hosting methodology** | The same, for infrastructure providers, including the upstream-attribution rules | [Read](https://scorecards.hiveit.ai/guide-methodology-cloud-hosting-scorecard.html) |
| **Tech-stack methodology**        | The same, for software and hosted services, including how a stack score is composed | [Read](https://scorecards.hiveit.ai/guide-methodology-tech-stack-scoring.html) |
| **Impact calculator methodology** | The carbon and water model: constants, sources, band derivations, worked examples, and its restatement history | [Read](https://scorecards.hiveit.ai/guide-stack-impact-calculator-methodology.html) |

The methodology documents are written to be **peer reviewed**. They state their deviations from
the framework, the decisions still open, and the places where a value is a judgement rather than
a measurement — including where a constant's original derivation could not be reconstructed.
If that sounds like an invitation to find fault, it is.

---

## How to read a score

**Scores run 0–4** on each of thirteen criteria, grouped into three pillars: Environmental,
Social & supply chain, and Ethics & governance.

**Every score carries an assurance level** — Verified, Self-reported, Estimated or Unknown —
recording how good the evidence is. This is *never* multiplied into the score. Earlier versions
did that, and it hid both answers at once: strong performance on weak evidence became
indistinguishable from weaker performance on strong evidence. Read the two together.

**Read them in this order:**

1. **Red flags first.** A flag takes precedence over any number. It marks something a decision
   should turn on regardless of the average.
2. **Then the pillar scores**, with evidence coverage and the assurance mix.
3. **Then the weak-pillar flag**, which fires whenever any pillar scores zero.
4. **The single overall percentage last, and never on its own.** It is a secondary output. It
   combines the pillars with a weighted geometric mean, so a weak pillar cannot be averaged away
   by strong ones, and it is dismissible on every page.

**Equal pillar weights are the default.** Earlier versions used a 40/30/30 split; that implied a
precision the evidence cannot support. You can set your own weights where a decision genuinely
warrants it, but the equally-weighted result is what gets reported alongside.

**A low score is not always a criticism, and a gap is not a failure.** The framework separates
*not applicable* (the criterion cannot apply to this kind of thing) from *not disclosed*
(nothing was found after a competent search, and the search standard is published so you can
re-run it). Where a criterion is inherited from a provider further down the stack, that is
declared rather than silently scored.

### What these scores are not

- **Not comparable across entity types or domains.** Comparing a database engine's total with a
  hyperscaler's is meaningless, and the framework says so explicitly. Composing a stack is the
  supported way different kinds of thing interact.
- **Not audited.** Assurance levels record what kind of evidence sits behind each cell; only
  cells marked Verified rest on independent verification.
- **Not permanent.** Every assessment carries a date and a twelve-month maximum review window.
  Company conduct changes, and disclosures improve.
- **Estimates, where the calculator is concerned.** The carbon and water figures are
  order-of-magnitude estimates from a published model, not measurements of your site.

---

## Found something wrong?

Corrections are genuinely wanted, and several of the figures published here exist in their
current form because someone checked a claim that had been taken on trust.

- **A score you can show is wrong** — open an issue with the evidence. A published document,
  filing, register entry or audited report is the most useful thing you can bring; we will say
  in the version history what changed and why.
- **A methodological objection** — open an issue against the relevant methodology document. The
  framework records at least one rule we are openly unsure about (how a corporate steward's
  conduct should bear on the open-source project it stewards) and invites exactly this.
- **If you are the company being assessed** and you publish something our search missed, that is
  the easiest kind of correction to make. Point us at it.

Nothing changes silently. Any change to a score or a published figure is recorded in the
version history of the document it affects.

---

## Versions and provenance

|                               |                                        |
| ----------------------------- | -------------------------------------- |
| Framework                     | **v4.0**, published 13 August 2026     |
| Scorecard methodologies       | **v1.0**, approved 13 August 2026      |
| Impact calculator methodology | **v1.6**, 13 August 2026               |
| Evidence base                 | last reviewed and restated August 2026 |

All four scorecards declare the framework version they conform to, in the page and in their
methodology document. The carbon arithmetic is cross-checked against the Green Web Foundation's
[co2.js](https://github.com/thegreenwebfoundation/co2.js) reference implementation on every
release, segment by segment.

Figures produced with earlier versions of the impact calculator are **not** carried forward
silently — where a constant moved, the methodology's changelog says by how much the published
figures changed and that they must be restated. That record is deliberately kept in full.

---

## Licence

| What                                                         | Licence                                                   |
| ------------------------------------------------------------ | --------------------------------------------------------- |
| Framework text, methodology documents, scorecard content and notes | [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) |
| Code — page templates, scoring engine, build scripts         | [Apache 2.0](LICENSE)                                     |

You may copy, adapt and use this work, including commercially, provided you credit **Hive IT**
and the **Online Ecosystem Ethics Framework (OEEF)**. If you build a conforming scorecard of
your own, the framework asks you to publish a methodology document and a conformance statement
alongside it, and to state which framework version you conform to.

Versions published before v3.0 remain available under CC0 1.0 as originally published.

© Hive IT 2026.

---

## What is not in this repository

- **The internal build of the tech-stack scorecard.** It carries client stack presets and is not
  published. The build here has the same 92 assessments and no client data; its four worked
  presets — GOV.UK, BBC, Amazon and Google — are assembled from public information, and the two
  hyperscaler ones are labelled as approximations rather than confirmed stacks.
- **The build tooling and evidence records.** The scorecards and guides are generated from
  Markdown and JSON sources in a separate private repository, along with the decision register,
  the evidence briefs and the release checks. This repository holds the published output.
