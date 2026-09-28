# Life OS

A personal operating system built in **AppFlowy**, designed around a structured software development learning engine, planner, and habit/RPG progression system.

---

## What is Life OS?

Life OS is a self-contained productivity and learning workspace that answers:

> **What do I do now? Why? What does "done" mean? What comes next?**

The system is built to support becoming a full-stack software developer through a structured curriculum, milestone-indexed planner, quiz-based mastery gates, and a gamified XP/level progression layer.

---

## Architecture

```
                          LIFE OS
                             │
     ┌───────────────────────┼───────────────────────┐
     │                       │                       │
 EXECUTION               LEARNING               PROGRESSION
     │                       │                       │
 Goals / Projects    Curriculum Sources         XP / Levels
 Tasks / Planner     Learning Topics            Quests / Rewards
 Calendar            Learning Material          Streaks
 Habits / Logs       Videos / Resources         Challenges
                     Tests / Mastery
                             │
                         DASHBOARDS
                    TODAY | SOFTWARE DEV | LIFE
```

### System Layers

| Layer | Contents |
|---|---|
| **A — Foundation** | Life Areas, Goals, Projects, Milestones |
| **B — Execution** | Tasks, Planner, Calendar, Habits, Study Sessions |
| **C — Learning Engine** | Subjects, Modules, Topics, Learning Pages, Quizzes, Attempts, Practice Tasks, Resources |
| **D — Progression** | XP Events, Levels, Quests, Rewards, Streaks, Challenges |
| **E — Secondary** | Health, Finance, Journal |

---

## Primary Focus

### Software Development Learning Engine

The highest-priority module. Every learnable topic becomes a guided experience:

```
Choose Topic
    ↓
Read finished learning material
    ↓
Watch recommended video(s)
    ↓
Take quiz  (pass threshold: 80%)
    ↓
Pass → Practice / Demonstrate
    ↓
Mark mastery → Earn XP
    ↓
Unlock next topic
```

### Primary Project — High-Concurrency Distributed URL Shortener

Built from scratch as the practical spine of the 24-week curriculum:

- Spring Boot + PostgreSQL + JPA
- React + TypeScript
- JWT Authentication
- Testing + Testcontainers
- Docker / Docker Compose
- Redis + Rate Limiting
- Kafka (async analytics)
- AWS EC2 + Nginx + HTTPS
- Prometheus + Grafana
- Load Testing + System Design

---

## Learning State Machine

```
🔒 Locked  →  ⚪ Available  →  📖 Learning  →  🧠 Ready for Test
                                                        ↓
                                              📝 Testing
                                         ┌──────┴──────┐
                                     Fail              Pass
                                       ↓                ↓
                                  🔁 Needs          💻 Practice
                                   Review                ↓
                                       └──────→   ✅ Mastered
```

---

## Mastery ≠ Presence

| State | Meaning |
|---|---|
| Resource found | ≠ Learned |
| Lesson generated | ≠ Learned |
| Lesson read | ≠ Learned |
| Quiz passed | = Evidence of understanding |
| Practice completed | = Evidence of application |
| Demonstrated | = Evidence of usable mastery |

---

## XP System

| Action | XP |
|---|---|
| Micro task completed | +5 |
| Standard learning task | +15 |
| Deep / complex task | +30 |
| Quiz passed | +15 |
| Practical demonstration | +40 |
| Topic mastered (bonus) | +25 |
| Habit completion | +10 |
| Quest completion | +50 |
| Milestone completion | +100 |

---

## Build Protocol

```
Stage 0  →  Reconcile sources + decisions
Stage 1  →  AppFlowy capability verification
Stage 2  →  Curriculum ingestion (structure only)
Stage 3  →  Roadmap mapping
Stage 4  →  Learning Engine schema
Stage 5  →  Content enrichment (Week 1 first)
Stage 6  →  Seed / import package
Stage 7  →  AppFlowy construction
Stage 8  →  Dashboard build
Stage 9  →  End-to-end verification
Stage 10 →  Quality review
```

---

## Design Principles

- **One source of truth** — dashboards are views over canonical records, never duplicates.
- **ADHD-friendly** — short cards, one obvious next action, visible XP, constrained choices.
- **No fake progress** — XP, mastery, and streaks are derived from evidence only.
- **No hallucinated content** — no fabricated URLs, citations, quiz history, or completion states.
- **Timing is provisional** — schedule/timing kept out of the canonical data model.
- **Visual direction** — AFFiNE-inspired, implemented with AppFlowy-native capabilities.

---

## Platform

**AppFlowy** (desktop/cloud) — primary workspace.

---

## Status

`Stage 0 — Gate 0 complete. Stage 1 (AppFlowy capability verification) pending.`

---

## Repository

This repository contains the build-control package for the Life OS AppFlowy workspace.  
Curriculum content, personal data, and workspace exports are not committed here.
