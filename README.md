# CCA-F Mock Exam · Claude Certified Architect — Foundations

A free, full-length **practice exam** for Anthropic's **CCA-F (Claude Certified Architect – Foundations)** certification. It runs entirely in the browser — no signup, no install, nothing to configure — and draws a **different 60-question paper every time you open it**.

> ⚠️ **Unofficial.** This is community-built study material, **not affiliated with, authorized by, or endorsed by Anthropic.** "Claude," "CCA-F," and "Claude Certified Architect" are marks of Anthropic. Questions here are original practice items written against the publicly described exam blueprint — they are **not** real exam questions, and a passing score here is no guarantee of passing the actual exam.

![Static Site](https://img.shields.io/badge/type-static%20HTML-B8532E)
![No Dependencies](https://img.shields.io/badge/dependencies-none-4C7A48)
![No Tracking](https://img.shields.io/badge/tracking-none-3C5A78)
![Cost](https://img.shields.io/badge/cost-free-4C7A48)

**▶ Live demo:** <https://thisisrohitsoni.github.io/cca-f-mock-exam/>

---

## What's inside

- **Randomized every load.** Each sitting draws a fresh **60-question paper** from a bank of **153 distinct questions**, weighted to match the blueprint. Both question order and answer-option order are shuffled, so you can retake it indefinitely and effectively never see the same paper twice (on the order of 10⁴⁰ possible combinations). Reload, or hit **Retake**, to draw a new one.
- **120-minute timed mode** — no feedback until you submit, auto-submits at zero (the realistic run).
- **Untimed study mode** — locks each answer on selection and shows the explanation immediately.
- **Resume where you left off.** Your in-progress attempt (current question, answers, flags, time remaining) is saved in your browser; if you reload or come back later, it offers to resume. Nothing leaves your device.
- **Scenario-based questions** built around six recurring production scenarios — a fintech multi-agent platform, a healthcare triage agent, a Claude Code CI/CD setup, a legal contract-extraction pipeline, a logistics routing/dispatch agent, and an insurance claim-intake pipeline.
- **Single- and multi-select** items, with multi-select scored all-or-nothing as on the real exam.
- **Scaled scoring out of 1000** with a **720 pass line**; scenario and anti-pattern items carry higher weight.
- **Per-domain performance breakdown** on the results screen.
- **Answer review** showing only the questions you answered, each with the correct answer and a full explanation — filterable by correct / incorrect / flagged.
- **Keyboard shortcuts** during the exam: `1`–`6` select an option, `←`/`A` previous, `→`/`D` next, `M` flag for review.
- **Accessible & safe** — labelled question-navigator controls (ARIA), a sticky header with a live "Question X of 60" indicator and a Home button, and all question text rendered through an allow-list sanitizer.

## Domains covered

Weighted to match the published CCA-F blueprint. Each sitting draws the per-exam count below from a larger per-domain pool:

| # | Domain | Weight | Questions per exam | Pool size |
| --- | --- | --- | --- | --- |
| 1 | Agentic Architecture & Orchestration | 27% | 16 | 38 |
| 2 | Tool Design & MCP Integration | 18% | 11 | 30 |
| 3 | Claude Code Configuration & Workflows | 20% | 12 | 30 |
| 4 | Prompt Engineering & Structured Output | 20% | 12 | 30 |
| 5 | Context Management & Reliability | 15% | 9 | 25 |
| | **Total** | **100%** | **60** | **153** |

The answer key leans on the exam's core meta-principle throughout: **programmatic enforcement beats prompt-based guidance** (e.g. `stop_reason`-driven loops over text-parsing, schema + validation + retry over "always return JSON," and programmatic escalation triggers over sentiment or self-reported confidence).

## How to use it

Just open the live link and pick a mode. Each visitor runs an independent session, so any number of people can take it at the same time.

To run it locally, download `index.html` and open it in any browser — it works fully offline.

## Tech notes

- A **single self-contained HTML file** — markup, styles, and logic in one file, no build step.
- **No backend, no database, no external runtime dependencies.**
- **No analytics, cookies, or tracking.** The only thing stored is your own in-progress attempt, kept in your browser's local storage so you can resume; it never leaves your device, and it's cleared when you finish or start fresh.
- Because it's plain static HTML, it hosts free on essentially any static host and carries **zero vendor lock-in**.

## Deploy your own

**GitHub Pages (recommended)**

1. Fork or create a **public** repo containing the file.
2. Name the file **`index.html`** so it loads at the clean root URL.
3. **Settings → Pages →** Source: *Deploy from a branch*, branch `main`, folder `/ (root)`, then **Save**.
4. ~1 minute later your site is live at `https://<your-username>.github.io/<repo-name>/`.

If you want a nice link preview when sharing, also add an `og.png` (1200×630) to the repo root and update the `og:image` / `og:url` tags in the `<head>` of `index.html` to point at your own URL.

**Drag-and-drop, no Git** — Cloudflare Pages or Netlify: sign up free, choose direct upload, drop in the files, and you get a public URL. Cloudflare Pages has no bandwidth cap.

## Usage & license

The author retains ownership of this material. You're welcome to **use and share it for personal study**, and to fork it to host your own copy. If you publish a modified version, please keep the unofficial / not-affiliated-with-Anthropic notice intact.

*Optional:* add a `LICENSE` file if you want formal terms — **MIT** is a common choice for the code, or **CC BY-NC** if you want to permit sharing while reserving commercial use.

## Disclaimer

This project is for educational practice only. It is not legal, professional, or certification advice, and provides no guarantee of any exam outcome. The live CCA-F exam is currently gated behind Anthropic's Claude Partner Network; consult Anthropic's official resources for authoritative, current exam information.
