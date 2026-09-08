<div align="center">

# Macpaul Noble Appiah-Adu

<samp>SOFTWARE&nbsp;ENGINEER&nbsp;&nbsp;·&nbsp;&nbsp;AI&nbsp;SYSTEMS&nbsp;&nbsp;·&nbsp;&nbsp;INTERFACE&nbsp;DESIGN</samp>

<br>

**I build systems that verify their own work.**

Most of my time goes to an AI development orchestrator that plans, gates on human
approval, delegates the work — then inspects the repository itself rather than
trusting the report it was handed.

<br>

[**dev-orchestrator**](https://github.com/Macpaul26/dev-orchestrator) &nbsp;·&nbsp;
[**Repositories**](https://github.com/Macpaul26?tab=repositories) &nbsp;·&nbsp;
[**LinkedIn**](https://www.linkedin.com/in/macpaul-appiah-adu-9a73ab35a) &nbsp;·&nbsp;
[**Email**](mailto:mappiahadu@gmail.com)

<sub>Computer Science · University of Ghana, Legon</sub>

</div>

---

## 01 · What I build

I work where AI systems meet real software engineering. The interesting problem there
isn't getting a model to produce code — it's deciding what to trust once it has.

That question shapes how I build everything else: typed boundaries, narrow capabilities,
tests that describe guarantees rather than implementations, and interfaces quiet enough
that people actually use them.

Three things hold my attention — **agent architecture and verification**, **full-stack
TypeScript**, and **the design layer** that most engineers skip.

---

## 02 · Flagship

### dev-orchestrator

**A general-purpose AI development orchestrator that never takes an agent's word for it.**

> The coding agent's report is never authoritative.

It loads project context, plans, gates on human approval, delegates implementation to a
coding agent, and then establishes for itself what changed. An agent reporting success is
producing a *claim*, not evidence — so the two are kept structurally apart:
`ImplementationReport` carries `claimed*` and `observed*` fields, and there is no code
path that writes a claim into an observation.

**What I built**

- **A controlled tool bridge.** The coding agent touches a repository only through four
  typed, grant-bound operations — never a raw filesystem API. The request protocol has no
  field for a grant, project, session, scope or budget, so authority is not something the
  agent can name.
- **Read-only repository evidence.** Metadata, status, changed paths and bounded file
  excerpts, exposed through a closed set of operations rather than open access.
- **Tamper-evident experience storage.** Project-isolated records that survive a restart,
  are ordered and paged from filenames rather than by parsing the whole corpus, and are
  refused on read if corrupt or filed under the wrong project.
- **A quota that holds under concurrent writers.** Writes serialize through a
  cross-process lock and the count is derived from the records inside that lock — a
  directory too large to scan completely refuses the write instead of trusting a partial
  count.

**Stack** — TypeScript (strict) · Node 22 · LangGraph · Anthropic SDK · Zod · Vitest · SQLite checkpointing

<sub>31 test suites · 16 source modules · 13 phase documents · ships as a <code>dev-agent</code> CLI</sub>

[**View repository →**](https://github.com/Macpaul26/dev-orchestrator)

---

## 03 · Selected work

### Newbreed — campus ministry website

An editorial site for the ICGC campus ministry at the University of Ghana, built around a
content-integrity policy: the site is not allowed to claim something the church hasn't
said. Routed React app with a real design system rather than component defaults.

<sub>React · Vite · TypeScript · Tailwind · Radix UI · TanStack Query · Framer Motion · Playwright · Vitest &nbsp;—&nbsp; **private repository**</sub>

### God-man Classics — storefront and admin

A commerce project on TanStack Start with Supabase behind it — catalogue, cart, and an
admin surface for managing stock.

<sub>TanStack Start · Supabase · Tailwind v4 · Radix UI · TypeScript &nbsp;—&nbsp; **private repository**</sub>

### Ghana Smart Service Operations Optimizer

Campus maintenance triage over a real SQLite database — 56 locations, 140 roads, 320
service requests, 32 resources. **15 data structures and 8 algorithms implemented from
scratch**, with no `java.util` collections: priority scheduling, Dijkstra routing,
BFS/DFS reachability, Prim and Kruskal, and budget-constrained selection.

<sub>Java · SQLite &nbsp;—&nbsp; group project, TEAM ATLAS · DCIT 204/308</sub>

[**View repository →**](https://github.com/Macpaul26/TEAM-ATLAS-GROUP-25-)

---

## 04 · Technical focus

| Area | Working with |
| :--- | :--- |
| **Languages** | TypeScript, Java, Python |
| **AI systems** | Anthropic SDK, LangGraph, tool and capability design, Zod-typed boundaries |
| **Frontend** | React, Vite, Tailwind CSS, Radix UI, TanStack Query, Framer Motion |
| **Backend & data** | Node.js, SQLite, Supabase / PostgreSQL |
| **Testing & quality** | Vitest, Playwright, Testing Library, ESLint, strict TypeScript |

<sub>Every tool listed here appears in a repository I have actually shipped code into.</sub>

---

## 05 · Current direction

**Learning from verified experience.** Getting the orchestrator to improve its own
planning and verification from outcomes it confirmed itself — never from what an agent
claimed. The store is built and deliberately unwired; a test asserts that no production
module imports it yet.

**Holding the authority boundary.** Learning informs reasoning and never becomes
authority. A lesson drawn from a hundred verified runs still cannot approve a plan, grant
a capability, widen a scope, or disable a check.

**Design as engineering.** Pushing the interface layer of my product work toward
something closer to editorial design than to framework defaults.

---

## 06 · How I work

- **I review my own merged work.** The concurrency quota above was rewritten after a
  second pass found two ways it could fail under simultaneous writers — neither of them
  visible to a single-threaded test, which is exactly why the original suite passed.
- **Architecture gets written before it gets built.** Each milestone has a phase document
  that states plainly what is guaranteed today and what is deferred.
- **Tests describe guarantees, not implementations.** Where a boundary matters, there is a
  test asserting the boundary itself — including tests that fail if the wrong module ever
  imports another.

---

## 07 · Contact

<div align="center">

[**Email**](mailto:mappiahadu@gmail.com) &nbsp;·&nbsp;
[**LinkedIn**](https://www.linkedin.com/in/macpaul-appiah-adu-9a73ab35a) &nbsp;·&nbsp;
[**GitHub**](https://github.com/Macpaul26?tab=repositories)

<br>

<sub>Ghana · Always open to a conversation about AI systems, verification, or good interfaces.</sub>

</div>
