# Workout Plan — PWA Spec

## Structure
- 3 sessions/week: **Tue (hard)**, **Thu (hard, → Fri fallback)**, **Sat (light)**
- Sun = badminton (external, not tracked as lift)
- Session length: ~60 min
- Every session logs: exercise, sets, reps, load, date
- Skill work is **never to failure** — stop 2s before form breaks
- Progress an exercise only when top of its rep range is clean for **2 sessions in a row**

---

## Session A — Tuesday (pull + squat)

**Core (8 min)**
- Dead bug — 3×12
- Hollow hold — 3×25s

**Skill first (12 min)**
- Tuck front lever — 5×8s
- Tuck L-sit — 5×12s

**Strength**
- Pull-ups — 5 sets (4×5 + 1×8)
- Barbell squat — 4 sets (3×5 @ 60kg + 1×10 @ 50kg)
- Aussie rows (feet elevated) — 4×12
- Standing calf raise — 3×20 @ 20kg (slow 3s down)

**Explosive (5 min)**
- Jump squat — 4×6

---

## Session B — Thursday (push + hinge)

**Core (8 min)**
- Plank — 3×40s
- Side plank — 3×25s each

**Skill first (12 min)**
- Pike push-up — 4×8
- Support hold (top of dip) — 4×15s

**Strength**
- Dips (fists/handles) — 5 sets (4×5 + 1×10)
- DB Romanian deadlift — 4×10 @ 17–20kg each
- Push-ups — 4×12
- Lateral raise — 3×15 @ 5–7kg
- Bulgarian split squat — 3×10 each @ 12–14kg each

**Explosive (5 min)**
- Split squat jump — 3×6 each

---

## Session C — Saturday (light, pre-badminton)

**Skill practice (no grind)**
- Tuck front lever — 4×8s
- Tuck L-sit — 4×12s
- Wall handstand — 3×20s *(gated: skip unless wrist 100%)*

**Light full body**
- Goblet squat (slow) — 3×12 @ 20kg
- Aussie rows — 3×12
- Push-ups — 3×12

**Agility (smash prep)**
- Lateral bounds — 3×8 each
- Box jumps (step down) — 3×5

---

## Exercise progressions
Each exercise advances one rung when its progress trigger is met.

| Exercise | Progression path | Progress trigger |
|---|---|---|
| Pull-ups | BW → +5kg → +10kg → archer → one-arm | 4×8 clean |
| Dips | BW → +5kg → +10kg → ring dips | 3×10 clean |
| Push-ups | standard → archer → pseudo planche | 3×15 clean |
| Aussie rows | feet flat → feet elevated → weighted → one-arm | 4×12 clean |
| Barbell squat | +5kg jumps: 60 → 65 → 70 → 75 → 80 | 5×5 solid |
| DB RDL | 17 → 20 → 22kg each hand | 4×10 easy |
| Bulgarian split squat | 12 → 14 → 16kg each | 3×10 clean |
| Standing calf raise | 20 → 24 → 28kg | 3×20 clean |
| Lateral raise | 5 → 7 → 9kg | 3×15 clean |
| Jump squat | BW → 5kg vest → 10kg vest | 4×6 controlled |
| Goblet squat | 20 → 24 → 28kg | 3×12 clean |

---

## Skill progressions (from zero)
8-week base build. Advance a rung when the hold/rep target is clean for 2 sessions.

### L-sit
| Rung | Target |
|---|---|
| 1. Foot-supported / tuck hold | 5×10s |
| 2. Tuck (longer) | 5×15s |
| 3. Advanced tuck (hips open) | 5×12s |
| 4. One-leg extended | 5×10s each |
| 5. Full L-sit | 5×10s |

### Front lever
| Rung | Target |
|---|---|
| 1. Scap pull-ups (prereq) | 4×8 |
| 2. Tuck FL hold | 5×8s |
| 3. Tuck FL (longer) | 5×12s |
| 4. Advanced tuck | 5×8s |
| 5. One-leg FL | 5×8s each |
| 6. Straddle FL | 5×5s |

### HSPU (pike path)
| Rung | Target |
|---|---|
| 1. Pike push-up, feet on floor | 4×8 |
| 2. Feet on low box | 4×6 |
| 3. Feet on high box | 4×6 |
| 4. Wall HSPU negatives | 4×3 |
| 5. Wall HSPU full | 4×5 |

### Handstand *(gated — start only when wrist 100%)*
| Rung | Target |
|---|---|
| 1. Wall walks | 3×3 |
| 2. Chest-to-wall hold | 3×20s |
| 3. Free balance kicks | 3×5 |
| 4. Free handstand | 3×10s |

---

## PWA feature notes
- Phase toggle already exists (Phase 1 / Phase 2) — this is the Phase 2 content
- Skill blocks need hold-timer support (seconds-based), separate from rep-based sets
- Each exercise + skill rung should track: current rung, sessions-at-target counter (for the 2-session progress rule), auto-suggest advance when trigger met
- Sat session flagged "light" — exclude from progressive-overload prompts
- Wrist-gated items (handstand) need a manual unlock toggle
