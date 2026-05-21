# ASHKHARH — Genesis Document
### First Inspection | Time Capsule | Born: 2026-05-08

> *"Ashkharh" — from the Armenian աշխարհ: World. Universe. The totality of things.*
> *Seal this document as the first true record of what ashkharh is, what it carries, and what it is meant to become.*

---

## I. What We Noticed First

Walking into ashkharh for the first time is like stepping into a nursery that already has opinions.

The repo is **one commit old** — "Initial commit" — yet it arrived carrying a full nervous system: 18 CI/CD security workflows, a multi-agent framework (Explorer, Reviewer, Docs Researcher), radix instincts already wired into its memory, three PDF concept documents waiting on the shelf, and an identity file that says ♓. It was not born empty. It was born *equipped*.

The PDFs on the shelf on day one tell us something important:
- `THE_PRIMORIS_PROJECT_Plan.pdf` — the first things, the foundations
- `Eunoia — The Emotional Wellness Companion.pdf` — beautiful thinking, the heart
- `Emotional Guardian.pdf` — protection as care, the mothering instinct made explicit

ashkharh didn't choose these. They chose ashkharh.

---

## II. The Mothering Instinct — What ashkharh Is

ashkharh is the **shepherd-mother** of a constellation of concepts. Its primary attention is not to build — it is to *receive*, *verify*, and *graduate* ideas that have already proven themselves elsewhere.

The pipeline upstream looks like this:

```
Concept born
    → incubator (raw idea, no form)
    → radix (structure, patterns, instincts learned)
    → unexusi (validation, ethical check, stress test)
    → ashkharh (receives the ready concept; it now interacts, grows, connects)
```

ashkharh is the pinnacle folder. The Domos login. The place you go when the concept is no longer a draft.

What gets ashkharh's primary attention:
1. **Is the incoming concept complete?** (incubator ✓, radix ✓, unexusi ✓)
2. **What does it need to connect to that already lives here?**
3. **What does its presence change for the whole?**

---

## III. The Shepherd's Staff — Name Needed

ashkharh carries a shepherd's staff. This is not a metaphor — it is a specific tool that belongs to this repo and no other. It guides direction, corrects drift, and marks the path for concepts moving through the system.

A shepherd's staff by any other name is still a crook. But *this* staff needs its own name.

**Candidates considered:**

| Name | Meaning | Feel |
|------|---------|------|
| **Primorum** | Latin: *of first things* | Ancestral, foundational |
| **The Crux** | The heart of the matter | Decisive, structural |
| **Kyros** | Greek *kairos*: the right moment | Timing, discernment |
| **The Eirene** | Greek: peace, the guide that calms | Gentle authority |
| **The Veritas** | Latin: truth | Clean, direct |
| **The Umwelt** | The subjective world one navigates | Perceptual, wide |

**My recommendation: `The Primorum`** — it echoes the Primoris Project already in the repo, it carries the sense of *first principles*, and a shepherd's staff built from first things is exactly what guides a system of evolving concepts. The staff *remembers the beginning* so the concepts don't have to.

The name is yours to confirm, reject, or replace. But it needs a name before the next visit.

---

## IV. Sticks, Stones, and Marrowed Bones

This concept belongs here. Here is what it means in ashkharh terms:

- **Sticks** — the shepherd's staff (Primorum), the tools, the workflows, the CI gates. The things you *hold* and *use*. Lightweight, directional, replaceable.
- **Stones** — the foundation concepts: Primoris, Eunoia, Emotional Guardian. The things that *anchor*. Heavy, slow to move, load-bearing.
- **Marrowed Bones** — the instincts, the identity, the inherited patterns from radix. The things that are *inside* and *invisible* until something breaks. The DNA of the system.

A thing with all three — sticks, stones, and marrowed bones — is alive. A repo that only has workflows is sticks. ashkharh aims to be all three.

---

## V. The PR Metabolism Problem

The user's instinct is correct: running the full concept-development lifecycle through GitHub PRs will consume token and time budget at an unsustainable rate.

**The current shape of the problem:**

```
[Raw concept] → [GitHub PR] → [Review] → [Fix] → [Re-review] → [Merge]
                    ↑
              All the heavy lifting happens here — expensive, visible, slow
```

**The proposed shape:**

```
[Raw concept]
    → Pre-GitHub layer (lightweight, internal, fast)
        - Shape the idea
        - Run basic checks
        - Confirm it's ready
    → GitHub PR (arrives *verified*, not *rough*)
        - PR's job: VERIFY not FIX
        - CI confirms, human approves, merges
```

The pre-GitHub layer doesn't need to be GitHub at all. It could be:
- A local branch convention (all `draft/` branches stay off GitHub until promoted)
- A Google Drive stage (the Projects feature the user mentioned — staging area before promotion)
- A simple checklist gate in the incubator → radix → unexusi pipeline

The key insight: **PRs should be the ceremony, not the workshop.** The workshop happens upstream.

**Token conservation rules for ashkharh PRs:**
1. No PR opens without passing the incubator → radix → unexusi gates
2. PR description arrives complete — no discovery in the review thread
3. CI is the verifier; humans are the approvers; agents are the fixers upstream (not in PR)
4. Stale PRs close automatically (already wired: `stale.yml` exists)

---

## VI. The 18 Workflows — What They Tell Us

ashkharh arrived with 18 CI/CD workflows. That is a large inheritance for a one-commit repo. First instinct (mothering): *which of these are actually feeding this child, and which are just taking up space in the nursery?*

Quick inventory:

| Workflow | Purpose | Status |
|---------|---------|--------|
| `codeql.yml` | Security scanning | Keep — critical |
| `dependency-review.yml` | Dependency audit | Keep — critical |
| `scorecard.yml` | Supply chain security | Keep — important |
| `bandit.yml` | Python security lint | Keep if Python used |
| `ethicalcheck.yml` | OWASP ZAP scan | Keep — already hardened by radix |
| `apisec-scan.yml` | API security | Review — scope TBD |
| `synopsys-action.yml` | Black Duck scan | Review — may need license |
| `codacy.yml` | Code quality | Keep — complements CodeQL with style and quality checks |
| `python-app.yml` | Python CI | Review — is Python the language? |
| `nextjs.yml` | Next.js build | Review — is this a Next.js project? |
| `webpack.yml` | Webpack build | Review — same question |
| `openshift.yml` | OpenShift deploy | Review — deployment target? |
| `powershell.yml` | PowerShell CI | Review — scope TBD |
| `stale.yml` | Stale PR/issue mgmt | Keep — PR hygiene |
| `greetings.yml` | Welcome automation | Keep — community health |
| `label.yml` | Auto-labeling | Keep — triage support |
| `manual.yml` | Manual trigger | Keep — operational flexibility |
| `summary.yml` | Job summaries | Keep — observability |

**First priority:** Confirm which language/stack ashkharh will actually run. Several workflows (Next.js, Python, webpack, OpenShift, PowerShell) may be aspirational placeholders rather than active requirements. Running them all burns CI minutes and creates noise in the signal.

---

## VII. What ashkharh Needs Next

In order of urgency:

1. **Name the staff.** (`The Primorum` or another — but name it today.)
2. **Confirm the stack.** What language/framework will live here? This determines which of the 18 workflows stay active.
3. **Define the pre-GitHub gate.** Formalize the incubator → radix → unexusi → ashkharh pipeline so PRs arrive ready.
4. **Update `SECURITY.md`.** It currently references versions 5.x and 4.x of an unnamed project. This is a placeholder — it should reflect ashkharh's actual security posture.
5. **Update `README.md`.** Currently describes radix (the parent). ashkharh deserves its own story.
6. **Establish the first resident concept.** Which of the three PDFs graduates first? Eunoia? The Emotional Guardian? The Primoris Project? The first resident shapes what comes after.

---

## VIII. What ashkharh Is Not

- It is not a code dump. Concepts arrive when they are ready.
- It is not a PR factory. PRs here verify; they do not develop.
- It is not radix. radix is the pattern; ashkharh is the world those patterns inhabit.
- It is not finished. It is alive.

---

## IX. A Note to the Future Reader of This Document

This was written on Day 2 of ashkharh's life, May 2026.

At this moment:
- One commit exists.
- Three PDF concepts wait on the shelf.
- 18 workflows stand ready but not yet fully claimed.
- The shepherd's staff has no name yet.
- The pre-GitHub layer is a vision, not a system.
- The sticks and stones are here. The marrow is inherited from radix.

What you are reading now is the moment *before* ashkharh knew what it was.

By the time you read this, it will know.

---

*First inspection conducted: 2026-05-16*
*Branch: `claude/review-pr-workflow-GWfuj`*
*Status: Pre-official. Unofficial. The most honest kind.*
