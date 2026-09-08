<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Macpaul26/Macpaul26/main/assets/monogram-dark.svg">
  <img src="https://raw.githubusercontent.com/Macpaul26/Macpaul26/main/assets/monogram-light.svg" alt="Macpaul Appiah-Adu monogram" width="76" height="76">
</picture>

# Macpaul Noble Appiah-Adu

<samp>SOFTWARE&nbsp;ENGINEER</samp>

**I build software that holds up.**

Clear architecture, typed boundaries, tested behaviour,<br>
and interfaces that stay out of the way.

<a href="https://github.com/Macpaul26?tab=repositories"><img src="https://raw.githubusercontent.com/Macpaul26/Macpaul26/main/assets/icons/brackets.svg" width="15" alt=""> Repositories</a>
&nbsp;&nbsp;·&nbsp;&nbsp;
<a href="https://www.linkedin.com/in/macpaul-appiah-adu-9a73ab35a"><img src="https://raw.githubusercontent.com/Macpaul26/Macpaul26/main/assets/icons/linkedin.svg" width="15" alt=""> LinkedIn</a>
&nbsp;&nbsp;·&nbsp;&nbsp;
<a href="mailto:mappiahadu@gmail.com"><img src="https://raw.githubusercontent.com/Macpaul26/Macpaul26/main/assets/icons/mail.svg" width="15" alt=""> Email</a>

<br>

<img src="https://raw.githubusercontent.com/Macpaul26/Macpaul26/main/assets/icons/layers.svg" width="15" alt=""> Architecture
&nbsp;&nbsp;&nbsp;
<img src="https://raw.githubusercontent.com/Macpaul26/Macpaul26/main/assets/icons/shield.svg" width="15" alt=""> Reliability
&nbsp;&nbsp;&nbsp;
<img src="https://raw.githubusercontent.com/Macpaul26/Macpaul26/main/assets/icons/window.svg" width="15" alt=""> Interface
&nbsp;&nbsp;&nbsp;
<img src="https://raw.githubusercontent.com/Macpaul26/Macpaul26/main/assets/icons/flow.svg" width="15" alt=""> AI systems
&nbsp;&nbsp;&nbsp;
<img src="https://raw.githubusercontent.com/Macpaul26/Macpaul26/main/assets/icons/terminal.svg" width="15" alt=""> Tooling

<br>

<sub>Computer Science · University of Ghana, Legon</sub>

</div>

---

<div align="center">

<sub><b>FEATURED PROJECT</b></sub>

## dev-orchestrator

**An AI coding agent, put on rails — work planned, approved by a human, delegated,<br>then verified against what the repository actually shows.**

</div>

<table>
<tr>
<td align="center" width="33%">
<img src="https://raw.githubusercontent.com/Macpaul26/Macpaul26/main/assets/icons/lock.svg" width="22" alt="">
<br><br>
<sub><b>CONTROLLED EXECUTION</b></sub>
<br>
<sub>Four typed, grant-bound operations. Never a raw filesystem API.</sub>
</td>
<td align="center" width="33%">
<img src="https://raw.githubusercontent.com/Macpaul26/Macpaul26/main/assets/icons/verify.svg" width="22" alt="">
<br><br>
<sub><b>INDEPENDENT VERIFICATION</b></sub>
<br>
<sub>Git state read first-hand. Claims kept structurally apart from observations.</sub>
</td>
<td align="center" width="33%">
<img src="https://raw.githubusercontent.com/Macpaul26/Macpaul26/main/assets/icons/flow.svg" width="22" alt="">
<br><br>
<sub><b>DURABLE WORKFLOW</b></sub>
<br>
<sub>Runs suspend at an approval and resume from checkpointed state.</sub>
</td>
</tr>
</table>

A `dev-agent` CLI drives it: register a project, start a run, and the workflow
executes until it suspends for a human decision. Nothing consequential happens
without that decision.

The design rule the whole system is built around — *a coding agent's report is
never authoritative.* `ImplementationReport` carries `claimed` and `observed`
fields separately, and no code path can write one into the other.

<sub><b>Selected engineering</b></sub>

- A capability boundary the agent cannot talk its way past — the request protocol
  has no field for a grant, project, scope or budget
- Tamper-evident, project-isolated storage that refuses corrupt or misfiled records on read
- A write quota that holds under concurrent writers, via a cross-process lock

<sub><b>Built with</b></sub>&nbsp;&nbsp;TypeScript (strict) · Node 22 · LangGraph · Anthropic SDK · Zod · Vitest · SQLite

<sub>31 test suites · 16 source modules · 13 phase documents</sub>

<a href="https://github.com/Macpaul26/dev-orchestrator"><img src="https://raw.githubusercontent.com/Macpaul26/Macpaul26/main/assets/icons/arrow.svg" width="16" alt=""> <b>View repository</b></a>

---

## <img src="https://raw.githubusercontent.com/Macpaul26/Macpaul26/main/assets/icons/cube.svg" width="20" alt=""> Engineering

<img src="https://raw.githubusercontent.com/Macpaul26/Macpaul26/main/assets/icons/brackets.svg" width="15" alt=""> &nbsp;**Languages** &nbsp;·&nbsp; <sub>TypeScript &nbsp;·&nbsp; JavaScript &nbsp;·&nbsp; Java &nbsp;·&nbsp; Python</sub>

<img src="https://raw.githubusercontent.com/Macpaul26/Macpaul26/main/assets/icons/flow.svg" width="15" alt=""> &nbsp;**AI systems** &nbsp;·&nbsp; <sub>LLM agents &nbsp;·&nbsp; Anthropic SDK &nbsp;·&nbsp; LangGraph &nbsp;·&nbsp; tool &amp; capability design</sub>

<img src="https://raw.githubusercontent.com/Macpaul26/Macpaul26/main/assets/icons/window.svg" width="15" alt=""> &nbsp;**Frontend** &nbsp;·&nbsp; <sub>React &nbsp;·&nbsp; Vite &nbsp;·&nbsp; Tailwind CSS &nbsp;·&nbsp; Radix UI</sub>

<img src="https://raw.githubusercontent.com/Macpaul26/Macpaul26/main/assets/icons/database.svg" width="15" alt=""> &nbsp;**Backend & data** &nbsp;·&nbsp; <sub>Node.js &nbsp;·&nbsp; SQLite &nbsp;·&nbsp; PostgreSQL</sub>

<img src="https://raw.githubusercontent.com/Macpaul26/Macpaul26/main/assets/icons/shield.svg" width="15" alt=""> &nbsp;**Practice** &nbsp;·&nbsp; <sub>Vitest &nbsp;·&nbsp; Playwright &nbsp;·&nbsp; ESLint &nbsp;·&nbsp; Git &nbsp;·&nbsp; strict TypeScript</sub>

---

## <img src="https://raw.githubusercontent.com/Macpaul26/Macpaul26/main/assets/icons/compass.svg" width="20" alt=""> Currently building

Extending **dev-orchestrator** so it can learn from outcomes it verified itself.
The store is built and deliberately unwired — a test asserts no production module
imports it yet.

Alongside it: full-stack TypeScript, and getting better at the interface layer.

---

## <img src="https://raw.githubusercontent.com/Macpaul26/Macpaul26/main/assets/icons/compass2.svg" width="20" alt=""> How I work

**Boundaries before features.** If a limit matters, there is a test that fails when it moves.

**Evidence over assertion.** Something reporting success is a claim, not a result.

**Review my own merged work.** The quota above was rewritten after a second pass
found two failures a single-threaded test could never have caught.

---

<div align="center">

<br>

<a href="mailto:mappiahadu@gmail.com"><img src="https://raw.githubusercontent.com/Macpaul26/Macpaul26/main/assets/icons/mail.svg" width="17" alt=""> <b>Email</b></a>
&nbsp;&nbsp;&nbsp;·&nbsp;&nbsp;&nbsp;
<a href="https://www.linkedin.com/in/macpaul-appiah-adu-9a73ab35a"><img src="https://raw.githubusercontent.com/Macpaul26/Macpaul26/main/assets/icons/linkedin.svg" width="17" alt=""> <b>LinkedIn</b></a>
&nbsp;&nbsp;&nbsp;·&nbsp;&nbsp;&nbsp;
<a href="https://github.com/Macpaul26?tab=repositories"><img src="https://raw.githubusercontent.com/Macpaul26/Macpaul26/main/assets/icons/brackets.svg" width="17" alt=""> <b>Repositories</b></a>

<br>

<sub>Ghana · Open to a conversation about system design, TypeScript, or good interfaces.</sub>

</div>
