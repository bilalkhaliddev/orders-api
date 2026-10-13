# Orders & Integrations API — Roadmap Progress

Source plan: `Bilal_Laravel_Backend_Roadmap_26_Weeks.docx` (Claude project "Laravel Roadmap").
This file is the single status ledger. Bilal updates the Status block and ticks checkpoints; Claude verifies at each Saturday review and returns the updated block to commit.

---

## Status

| Field | Value |
|---|---|
| Current week | 0 (Setup) — in progress |
| Phase | 0 — Setup |
| Week started | 2026-10-13 (Tue) — actual start; planned 2026-10-12 |
| Week 1 starts | 2026-10-14 (Wed) — one day behind plan; Saturday absorbs the slip |
| Planned end of Phase 5 (Week 26) | 2027-04-10 (Sat) — unchanged |
| Hours this week | 2 / 12 |
| Last review | 2026-10-13 — Week 0 day 1 verified by Claude (repo, README, devlog #1) |
| Next session goal | Finish Week 0 (intro video + AI assistant), then "Week 1 start" in the project |

---

## Calendar (6 days/week, Sunday off; Weeks 6, 12, 22 are buffer weeks)

| Phase | Weeks | Dates |
|---|---|---|
| 0 — Setup | 0 | 2026-10-10 → 2026-10-11 |
| 1 — Modern PHP & Laravel foundations | 1–6 | 2026-10-12 → 2026-11-21 |
| 2 — Testing, database engineering & integrations | 7–12 | 2026-11-23 → 2027-01-02 |
| 3 — Ship it: Docker, Git/CI, Linux, AWS, observability, security | 13–17 | 2027-01-04 → 2027-02-06 |
| 4 — Architecture, performance & AI-era engineering | 18–22 | 2027-02-08 → 2027-03-13 |
| 5 — Interview readiness & proof | 23–26 | 2027-03-15 → 2027-04-10 |
| 6 — Frontend (optional) | 27–32 | 2027-04-12 → 2027-05-22 |

If the plan slips by two weeks or more, re-plan with Claude and move the dates. Changing the date is fine; lowering the bar is not.

---

## Weekly checkpoints

Tick `[x]` when you believe it is done. Claude writes `verified YYYY-MM-DD` after the review. A week is complete only when verified.

### Phase 0
- [ ] W0 — Environment works (php -v, composer -V, laravel new); public GitHub; orders-api repo with README; DEVLOG entry #1; 60-second intro video recorded

### Phase 1 — Modern PHP & Laravel foundations
- [ ] W1 — money-calc package runs; interface vs abstract, enum, strict_types explained on camera
- [ ] W2 — SOLID with own examples; PHPStan level 6; 8 PHPUnit tests green
- [ ] W3 — Request lifecycle from memory; register vs boot; OrderNumberGenerator swapped via config
- [ ] W4 — 7 relationship types from memory; N+1 before/after shown; Query Builder vs Eloquent explained
- [ ] W5 — Every endpoint validated + authorized; one error JSON shape for 401/403/404/422/429; Sanctum vs Passport, Gate vs Policy on camera
- [ ] W6 — W3–W5 all green; 10 Collection methods from memory; mail renders; scheduler runs; topics 1–6 recorded

### Phase 2 — Testing, database engineering & integrations
- [ ] W7 — 40+ tests green; coverage report; feature vs unit explained
- [ ] W8 — One TDD feature with commit history; every fake used; 70+ tests
- [ ] W9 — Read an EXPLAIN and fix it; isolation levels explained; lockForUpdate test proves no overselling
- [ ] W10 — Worker-dies-mid-job explained; failed job retried from Horizon; cache invalidation strategy explained
- [ ] W11 — Webhook replayed twice → processed once; idempotency both directions; third-party outage handling
- [ ] W12 — Coverage ≥ 70%; v0.2 tagged; 5 ADRs; topics 7–14 recorded; mock interview #1 done

### Phase 3 — Ship it
- [ ] W13 — Fresh clone → running app in < 5 min via README; image vs container vs volume explained
- [ ] W14 — CI green (tests + Pint + PHPStan); rebase vs merge explained; PR a stranger could test from
- [ ] W15 — PR → production in one merge; Supervisor and queue:restart explained; Nginx → PHP-FPM flow
- [ ] W16 — IAM role vs user vs policy; S3 vs EBS vs RDS; presigned URL working; billing alarm set
- [ ] W17 — Error visible in Sentry with request id; 5 OWASP items + Laravel defence each; topics 15–20 recorded

### Phase 4 — Architecture, performance & AI-era engineering
- [ ] W18 — Business-logic placement explained; module boundary diagram; actions/DTOs/events refactor with tests green
- [ ] W19 — 2x improvement on one endpoint with k6 evidence; slow-endpoint debugging explained; Octane pitfalls
- [ ] W20 — "Scale to 10x" whiteboard in 10 min on camera; 2 min on each awareness topic; topics 21–25 recorded
- [ ] W21 — AI workflow explained; LLM feature live with tests; 3 bugs caught in AI code named
- [ ] W22 — Swagger UI live; v1.0 tagged; coverage ≥ 75%; mock interview #2 done

### Phase 5 — Interview readiness & proof
- [ ] W23 — Any of the 25 topics on camera without notes; 10 random → 8 confident; 5 STAR stories
- [ ] W24 — Two take-homes within time, tested, documented; live drill recorded and watchable
- [ ] W25 — 2 easy problems in 30 min consistently; video answers without restarts; MCQ self-test ≥ 80%; mock #3
- [ ] W26 — README a stranger can run from; CV checked against 5 real JDs; intro video clearly better than W0

### Phase 6 — Frontend (optional)
- [ ] W27 — Vanilla-JS page works against the API
- [ ] W28 — Vue component from spec in 30 min
- [ ] W29 — Sanctum SPA auth end to end
- [ ] W30 — Admin looks professional on mobile and desktop
- [ ] W31 — Inertia vs SPA vs Livewire explained
- [ ] W32 — One E2E test green in CI; admin live

---

## Open items

- W0: Record 60-second intro video (English)
- W0: Install one AI assistant (Copilot / Claude Code / Cursor)
- Fill or remove the empty 2026-10-10 devlog entry

## Blockers

- (none — git push hang on 2026-10-13 was the credential manager; resolved)

## Plan decisions (schedule and scope only — technical decisions go in docs/decisions.md)

| Date | Decision | Why |
|---|---|---|
| 2026-10-10 | Start Week 0 on Sat 10 Oct; Week 1 on Mon 12 Oct | Roadmap delivered today |
| 2026-10-13 | Actual start slipped to Tue 13 Oct (one day); Week 1 starts Wed 14 Oct; calendar dates unchanged, Saturday is the catch-up day | Monday was missed; buffer rules in roadmap §5.3 |

## Review log (filled by Claude at each Saturday review)

| Date | Week | Result | Top fixes |
|---|---|---|---|
| | | | |
