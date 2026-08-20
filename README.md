# Backend Learning Journey

Self-directed study plan for becoming a backend developer (Java / Spring Boot), documented in public.

I am a Software Engineering student. This repository holds the roadmap I follow, the schedule I hold myself to, and the notes I take while learning. It is a working record, not a tutorial — everything here is written for my own use and published in case it is useful to someone in the same position.

**The documents are in Vietnamese.** This README is in English so you can decide whether they are worth translating.

---

## Why this repository exists

Most learning roadmaps you find online are lists of topics. They tell you *what* to learn but not *when*, and they assume you have unlimited time. Mine is built around a hard constraint: the next university term starts on a fixed date, and the two heaviest backend courses land in it. Everything is scheduled backwards from that deadline.

The second reason is accountability. A plan kept in a private file is easy to quietly abandon. A plan in a public repository is not.

---

## Contents

### Planning

| File | What it is |
|---|---|
| `roadmap-public.md` | **Full roadmap** through graduation — one section per term, mapped against the actual course list. Includes the mistakes made while building it |
| `lo-trinh-giai-doan-1.html` | **Phase 1 roadmap** (1 Aug – 6 Sep 2026) — goals, principles, day-by-day schedule, contingency plan |
| `subject-importance.html` | **Course prioritisation** — every course scored by relevance to backend work, to decide where extra self-study time goes |

### Study notes

| File | What it is |
|---|---|
| `nen-tang-backend-tuan-1.html` | **Week 1** — client/server, HTTP, REST, CRUD, database fundamentals |
| `spring-boot-ngay-8-8.html` | **Spring Initializr and project structure** — what each dependency does and why the package layout matters |
| `tong-hop-project-todo.html` | **Knowledge summary** for the first project — every concept learned, why it exists, and the traps I fell into |
| `tra-cuu.html` | **Searchable reference** — only things I got wrong or forgot mid-session. Ctrl+F by term |

The HTML files are self-contained — no build step, no dependencies. Clone and open in a browser.

---

## Approach

### Three tiers of AI usage

The core rule of this plan. AI is not banned, but its role is fixed per stage:

| Tier | When | What AI may do |
|---|---|---|
| **Tier 1** | Phase 1 (until 6 Sep 2026) | Explain concepts only. **Never writes code for my assignments.** |
| **Tier 2** | Terms 3–4 | Reviewer — critiques code I wrote. Still no generated code. |
| **Tier 3** | From term 5, or day one of any real job | AI-assisted with judgement — boilerplate for things I have already proven I can write by hand. I review every line. |

The reasoning: this is the only stretch before heavy coursework where I can build the reflex of typing everything myself. If I get used to delegating at the foundation stage, every later stage rests on ground that was never there.

### How concepts are learned

- Every concept starts with the question **"what problem was this invented to solve"** — not memorising annotations as vocabulary.
- Terminology is sorted into three tiers: must memorise / understand the idea / safe to forget.
- All concepts from one session get assembled into **a single diagram**, and I explain it back from the diagram alone.
- Each concept closes with self-test questions. An answer that restates the question instead of naming the cause does not count as passing.

### What gets written down

`tra-cuu.html` only contains things I actually got wrong, asked about twice, or forgot mid-session. Anything obvious on sight is deliberately left out — a reference full of things you already know is a reference you stop opening.

### Working language

Code, comments, commit messages, and READMEs are **English only**. Study notes and roadmap documents stay in Vietnamese — they are for me, and thinking in my first language is faster.

---

## Phase 1 at a glance

**1 Aug – 6 Sep 2026 · 37 days**

Starting point: understood HTTP/REST/CRUD as concepts, basic Git. Could not write a complete CRUD API. Had never written SQL by hand.

| Week | Focus |
|---|---|
| 1–7 Aug | Client/server, HTTP, REST, CRUD, database fundamentals, Git flow |
| 8–14 Aug | Spring Boot + JPA + PostgreSQL. Four layers, typed by hand |
| 15–20 Aug | Exception handling, `ResponseEntity`, DTOs, validation |
| 21–25 Aug | Status codes, JUnit, checkpoint |
| 26 Aug – 6 Sep | Project #2 — different domain, one-to-many relationship, **written without step-by-step guidance** |

Target state by 6 Sep: two working Spring Boot + PostgreSQL projects with proper layering, exception handling, DTOs and validation; a one-to-many relationship handled correctly on both create and delete; unit tests on the service layer; and the ability to write a new endpoint without looking at old code.

### Deliberately not in this phase

- **SQL by hand** — deferred to week one of term 3, so it is learned alongside the database course rather than twice.
- **Spring Security** — term 4, when there is a project with real users.
- **Docker / CI** — term 5, when the project is large enough to need it.

Each of these waits until it solves a problem I am actually having. Learning Docker with nothing to deploy is learning syntax and forgetting it.

---

## Stack

Java 21 · Spring Boot 4 · Spring Data JPA / Hibernate · PostgreSQL 18 · Maven · JUnit · Postman · IntelliJ IDEA

---

## Status

Phase 1 in progress. Updated as I go — including the parts that did not work.

If you are following a similar path and want to compare notes, open an issue.
