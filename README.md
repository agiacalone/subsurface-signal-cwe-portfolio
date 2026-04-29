# Subsurface Signal — Cyber Warfare & Engineering Portfolio
**Anthony Giacalone**
University Lecturer · Malware Analyst · Reverse Engineer · Systems Thinker

> *A curated payload of labs, malware archives, and cyber warfare intent — transmitted from below test depth.*

I'm a Computer Science lecturer at California State University, Long Beach, teaching the security and systems track (CECS 326 Operating Systems, CECS 327 Distributed Systems, CECS 378 Intro to Computer Security, CECS 478 Advanced Computer Security). My public work spans three threads:

- **Security pedagogy** — original lab platforms that teach modern attack and defense, not 1996-era walkthroughs.
- **Hacker-culture preservation** — historical artifacts (the Morris Worm, the Jargon File, BBS-era textfile archives) maintained as living references.
- **Agentic engineering** — Claude Code skills that close the loop from lecture material to autograded student feedback.

This repo is the entry point. Most of my 400+ repos are course infrastructure — the links below are the ones worth your time.

---

## Table of Contents

- [Current Work](#current-work)
- [Security Lab Platforms](#security-lab-platforms)
- [Operating Systems & Systems Programming](#operating-systems--systems-programming)
- [Distributed Systems](#distributed-systems)
- [Programming Languages, Compilers & Data Science](#programming-languages-compilers--data-science)
- [Malware Archives](#malware-archives)
- [Agentic Engineering — Claude Code Skills](#agentic-engineering--claude-code-skills)
- [Hacker Culture & Preservation](#hacker-culture--preservation)
- [Background & Credentials](#background--credentials)

---

## Current Work

**[cecs-378-lab-buffer-overflow](https://github.com/agiacalone/cecs-378-lab-buffer-overflow)** — *v2 release, April 2026.* A leak-then-pwn buffer-overflow lab that teaches three concepts where the 1996-era original taught two: stack overflow with shellcode injection (Phase Φ), ret2libc to defeat NX (Phase Ω), and setuid privilege drop with `setreuid` re-elevation (both phases — the modern reality any exploit ending in a shell against a setuid binary has to handle).

Survives ASLR-on by design. Themed mainframe environment, Codespaces-only delivery, autograded against a per-student seed corpus. Built from a private dev repo via an allowlist-based release-sync tool that publishes a clean public student template — reference exploits and harnesses stay private. Pattern is reusable for future labs.

**[cecs-378-lab-malware-pokemon](https://github.com/agiacalone/cecs-378-lab-malware-pokemon)** — *"Gotta Hack 'Em All", April 2026.* A malware-analysis lab framed as ROM hacking *Pokémon Yellow* on the franchise's 30th anniversary. Students crack open a Game Boy ROM with a hex editor, locate data structures by hand, decode the 2bpp tile format, patch bytes at known offsets, and produce an IPS diff. The lab makes the pedagogical mapping explicit: locating sprite data ↔ finding shellcode in a binary, decoding custom encodings ↔ parsing obfuscated payloads, producing an IPS diff ↔ writing a minimal PoC patch. *The difference between a malware analyst and a ROM hacker is mostly intent and a software license agreement.*

**[unix-conventions](https://github.com/agiacalone/unix-conventions)** — Agentic skill that documents and structures code in the Unix tradition, grounded in *The Art of Unix Programming*. Used to keep my own tooling honest about its own conventions.

---

## Security Lab Platforms

Custom lab assignments for CECS 378 (Intro) and CECS 478 (Advanced). Each is a standalone repo with autograded scaffolding and instructor-private reference solutions.

### CECS 378 — Introduction to Computer Security
- [Buffer Overflow Lab (v2)](https://github.com/agiacalone/cecs-378-lab-buffer-overflow) — see Current Work.
- [Symmetric Cryptography Lab](https://github.com/agiacalone/cecs-378-lab-symmetric-crypto)
- [Malware: Pokémon ROM Hack ("Gotta Hack 'Em All")](https://github.com/agiacalone/cecs-378-lab-malware-pokemon) — see Current Work.
- [Malware: Super Mario Bros. ROM Hack](https://github.com/agiacalone/cecs-378-lab-malware-smb1)
- [Malware: Metroid ROM Hack](https://github.com/agiacalone/cecs-378-lab-malware-metroid)
- [Malware: Ultima V ROM Hack](https://github.com/agiacalone/cecs-378-lab-malware-ultimav)

### CECS 478 — Advanced Computer Security
- [PGP Lab](https://github.com/agiacalone/cecs-478-lab-pgp-new)
- [Malware: Super Star Trek](https://github.com/agiacalone/cecs-478-lab-malware-sst)
- [Buffer Overflow (Advanced)](https://github.com/agiacalone/cecs-478-lab-buffer-overflow)
- [Text Processing with sed/awk](https://github.com/agiacalone/cecs-478-lab-sed-and-awk)

---

## Operating Systems & Systems Programming

### CECS 326 — Operating Systems
- [Multithreaded Programming Lab](https://github.com/agiacalone/cecs-326-lab-threads)
- [Semaphores — Revamped (*Diablo mobile? Bah! Why not loot* this *dungeon instead!*)](https://github.com/agiacalone/cecs-326-lab-semaphores-revamp) — semaphores taught through a dungeon-crawl simulation.

### Tooling
- [qemu-lab](https://github.com/agiacalone/qemu-lab) — disposable KVM-backed VM sandbox for safely executing untrusted or dangerous student code on Fedora Linux.
- [dotfiles](https://github.com/agiacalone/dotfiles) — system config across macOS and Linux: zsh + powerlevel10k, neovim, tmux, mutt, slrn, statusline templating.

---

## Distributed Systems

### CECS 327 — Distributed Systems
- [Peer-to-Peer File Sharing Lab](https://github.com/agiacalone/cecs-327-lab-peer-to-peer)
- [Analytical Essay Assignment](https://github.com/agiacalone/cecs-327-lab-analytical-essay)

---

## Programming Languages, Compilers & Data Science

### CECS 444 — Compiler Construction
- [Semester Project — Compiler Construction](https://github.com/agiacalone/cecs-444-semester-project)

### CECS 342 — Programming Languages
- [Inform 7 Game Lab](https://github.com/agiacalone/cecs-342-lab-inform7)
- [Ruby Scripting](https://github.com/agiacalone/cecs-342-lab-ruby)
- [Erlang Concurrency](https://github.com/agiacalone/cecs-342-lab-erlang)
- [Prolog Logic Programming](https://github.com/agiacalone/cecs-342-lab-prolog)
- [Fortran 77 Legacy Lab](https://github.com/agiacalone/cecs-342-lab-fortran77)
- [Fortran 77 Program (QROOT)](https://github.com/agiacalone/qroot)

### CECS 450/451 — Data Science and AI
- [R Programming Project](https://github.com/agiacalone/cecs-450-lab-semester-project)
- [R Reference Materials](https://github.com/agiacalone/cecs-450-r-examples-and-docs)
- [AI: Informed Search Lab](https://github.com/agiacalone/cecs-451-lab-informed-search)
- [AI: First-Order Logic](https://github.com/agiacalone/cecs-451-lab-first-order-logic)

---

## Malware Archives

Archival repositories of historic malware with annotations and educational commentary. Used in CECS 378 and CECS 478 to teach the lineage of computer security from the first PC viruses through modern ransomware.

- [Elk Cloner](https://github.com/agiacalone/elk-cloner-malware) — the first widely-spread microcomputer virus (1982, Apple II).
- [Brain Virus](https://github.com/agiacalone/brain-virus-malware) — first IBM PC virus (1986).
- [Stoned Virus](https://github.com/agiacalone/stoned-virus-malware) — boot-sector classic.
- [Michelangelo Virus](https://github.com/agiacalone/michelangelo-virus-malware) — the 1992 media panic.
- [Morris Worm](https://github.com/agiacalone/morris-worm-malware) — the canonical 1988 case study. ⭐
- [Cabir Mobile Worm](https://github.com/agiacalone/cabir-worm-malware) — the first mobile-phone worm (Symbian, 2004).
- [LoveLetter Worm](https://github.com/agiacalone/loveletter-malware) — the email worm that defined a decade of social-engineering.
- [SunOS Rootkit](https://github.com/agiacalone/sunos-rootkit-malware)
- [WannaCry Ransomware](https://github.com/agiacalone/wannacry-malware) — the EternalBlue-driven 2017 outbreak.
- [Ambulance Virus](https://github.com/agiacalone/ambulance-malware)
- [SpySheriff Rogue AV](https://github.com/agiacalone/spysheriff-malware) — early scareware.

---

## Agentic Engineering — Claude Code Skills

Tools I built (and use daily) to make teaching and personal-information work tractable. Open-source skills designed to compose, with strict input/output contracts and consistent style enforcement.

- [lecture-materials-assistant](https://github.com/agiacalone/lecture-materials-assistant) — generates lecture notes (PDF), Cornell handouts, study questions, pop quizzes, GitHub Classroom assignments, question banks, exams, and slide decks for CS courses. Enforces strict style consistency and Cornell ↔ slide alignment auditing.
- [ta-grading-rubric](https://github.com/agiacalone/ta-grading-rubric) — generates TA grading rubrics directly from lab assignment READMEs.
- [assignment-triage](https://github.com/agiacalone/assignment-triage) — git-based authenticity triage for student GitHub Classroom submissions.
- [unix-conventions](https://github.com/agiacalone/unix-conventions) — see Current Work.
- [mlb-game-report](https://github.com/agiacalone/mlb-game-report) + [mlb-announcer-1930s](https://github.com/agiacalone/mlb-announcer-1930s) — newspaper-style and 1930s-radio-broadcast game reports from the MLB Stats API. Personal-domain skills; included to show range.

---

## Hacker Culture & Preservation

- [The Jargon File (Community Edition)](https://github.com/agiacalone/jargonfile) — the legendary hacker lexicon, maintained as a living reference. Submissions welcome. ⭐
- [super-startrek](https://github.com/agiacalone/super-startrek) — the classic Super Star Trek game (Tom Almy's enhanced port), maintained. ⭐

> *Understanding how hackers think isn't just useful — it's vital. The Jargon File helped define the mindset that built Unix, cracked systems, and reshaped software. It's not just culture. It's context.*

---

## Background & Credentials

**M.S. Thesis** — [*Evaluation of Security Methods for the Prevention of Malware on Mobile Devices*](https://www.proquest.com/openview/cd06aab6e06951ba6cdc064f959e8cb9/1?cbl=18750). Forecasting bootloader-level mobile threats before mainstream recognition.

**FCC Amateur Radio License — Extra Class.** Callsign **[N6SH](https://www.qrz.com/db/N6SH)**. The highest class license issued by the FCC; demonstrates advanced knowledge of RF spectrum, propagation, digital/analog transmission, and secure communication. (License lookup also available via the [FCC ULS](https://www.fcc.gov/uls) — search by callsign N6SH.) Currently self-studying for the FCC GROL Element 3 commercial radiotelephone exam.

---

*Transmissions from* [obsidianbay.net](https://obsidianbay.net) · *blog at* [anthonyg.sdf.org](https://anthonyg.sdf.org) · *running silent, running deep.*
