# Money is too effective in campaigns

**A Frame Creation problem situation — mapped, not solved. Open for pod formation.**

> Voters in competitive races need their choice to turn on something other than
> which message was repeated at them most, because what reaches them is selected
> by spending power rather than accuracy — and the open, financially unrestricted
> marketplace of speech that democracy depends on is exactly what lets
> concentrated capital buy that dominance.

### ▸ [Open the pitch](https://theupskillinglabs.github.io/jeremy/) · [Read the full web map](https://theupskillinglabs.github.io/jeremy/report.html)

*If you have two minutes, open the pitch. If you're deciding how to vote, read the map.*

---

## Why this is open, not bounded

Four forces hold it in place, and each one re-arms the others.

| Force | What it does |
| --- | --- |
| **Legal & structural** | Citizens United anchors campaign spending in constitutional First Amendment protection. Reform keeps hitting the same wall. |
| **Cognitive & social** | Voters aren't passive blank slates. They actively seek partisan narratives that confirm their identity — motivated reasoning, not gullibility. |
| **Systemic feedback** | When fact-checkers intervene, partisan actors brand the fact-checkers as biased. The intervention is neutralised and civic distrust deepens. |
| **Economic incentive** | Platform algorithms and media companies profit directly from high-conflict political ad spend. Nobody in the loop is paid to close it. |

## Where the evidence is strong — and where it isn't

Mapped from **6 cards across 7 signals** out of the Labs civics survey. Every
claim is traceable: the extracts and the themes narrative ship in this repo.

We stress-tested our own coverage across the seven dimensions of a problem
situation. Three came back empty.

| Dimension | Coverage | |
| --- | --- | --- |
| Problem | `██████████` | Strong — win rates, ad persuasion, media distrust |
| Value | `███████░░░` | Moderate — democratic integrity vs. free expression |
| Player | `████░░░░░░` | Thin — names AIPAC, crypto, AI; lacks roles and incentives |
| History | `███░░░░░░░` | Thin — cites Citizens United, misses historical trends |
| **Boundary** | `░░░░░░░░░░` | **Absent** — no distinction by race type, geography, district |
| **Flux** | `░░░░░░░░░░` | **Absent** — misses how AI/ad-tech shift persuasion costs |
| **Counter** | `░░░░░░░░░░` | **Absent** — no cases where heavy spend lost |

**Two blind spots follow from that.** We have no data on *where money stops
working* — presidential versus municipal, statewide versus ballot initiative —
and none on how generative AI is changing the unit cost of persuasion. And we
have analysed **no races where the outspent candidate won**, which means we're
currently assuming money's power is total rather than conditional. It's probably
conditional.

We also scored our own paradox **0/3 on sharpness**. That isn't a footnote; it's
the reason the pod exists.

## What the pod does first

No warm-up phase. The gaps are already named, scoped and matched to a method.

| # | Question | Method |
| --- | --- | --- |
| 01 | In which electoral contexts does high spend *fail* to deliver wins — and what neutralises it? | Secondary literature review and electoral dataset analysis — Perplexity, OpenSecrets |
| 02 | How do media buyers and strategists actually evaluate ad-spend ROI against voter scepticism and fact-checkers? | 3–5 expert qualitative interviews with campaign consultants, across parties |
| 03 | Are generative AI and automated ad generation lowering the marginal cost per persuaded voter — for insurgents, or for incumbents? | Deep-research sweep on political ad-tech and regulatory filings — NotebookLM |

**What we can't reach alone:** campaign media strategists who allocate real
digital budgets, late-deciding voters in competitive districts, and fact-checkers
who can say whether their work changes anything.

**Candidate problem owners** — ad-tech platform integrity, and fact-checkers —
are hypotheses, not commitments. Neither has been approached.

## What could break this framing

The *voter as passive object* fallacy. The cards currently assume voters are
dupes who are easily persuaded by ads. That ignores identity-driven choice —
voters often **want** low-veracity partisan messaging because it validates their
social group. If that's the stronger explanation, the whole frame moves. We'd
rather find that out in a pod than defend it on a ballot.

## Vote

Pods form at quorum. If this one reaches it, what follows is Frame Creation's
next steps, not a solution sprint: map the field, identify a client who could own
the paradox, choose a delivery context, deepen the archaeology, and only then
create frames.

### ▸ [Open the pitch and vote](https://theupskillinglabs.github.io/jeremy/)

---

<details>
<summary><b>What's in this repo</b></summary>

A static, self-contained export from The Labs Sensemaking Engine. No build step,
no dependencies.

| Path | What it is |
| --- | --- |
| `index.html` | The pod-ballot landing page — self-contained, no external assets |
| `report.html` | The report shell; hydrates the full narrative and spatial web map |
| `slides.html` | "Meet the Pod" slide deck |
| `assets/` | `style.css` and `viewer.js` — render the report and the map |
| `content/` | `situation.md` and `themes.md` — the human-readable narrative |
| `data/` | `project.jsonld` (semantic graph + coordinates), `extracts.csv` (extracted signals), `site-data.js` (fallback so `report.html` also renders over `file://`) |

Start with [`content/situation.md`](content/situation.md) for the narrative as
plain text, or [`data/extracts.csv`](data/extracts.csv) for the raw source
signals.

</details>

<details>
<summary><b>Running and publishing it</b></summary>

**Locally.** Serve over HTTP so `report.html` can fetch the content files:

```
python3 -m http.server
```

Then open <http://localhost:8000/>. Double-clicking `report.html` also works —
it falls back to `data/site-data.js` — but serving it is higher fidelity.
`index.html` is fully self-contained and works either way.

**On GitHub Pages.** Settings → Pages → deploy from branch `main`, folder `/`.
Published at <https://theupskillinglabs.github.io/jeremy/>.

</details>

---

<sub>The Upskilling Labs · Sensemaking Engine · Frame Creation (Kees Dorst) · exported 26 Jul 2026</sub>
