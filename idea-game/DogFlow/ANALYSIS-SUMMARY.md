# DOGFLOW - ANALYSIS SUMMARY
## Idea Validation and APS Metrics Dashboard

> **Status:** READY FOR PROTOTYPE V1
> **Framework:** Voodoo March 2026
> **Date:** 2026-04-01

---

## Executive Summary

| Metric | Target | Status | Notes |
|--------|--------|--------|-------|
| **Concept** | Dog placement + flock redirection | PASS | Simpler to read, stronger fantasy |
| **APS (50 levels)** | > 1.4 | **1.48** | Balanced with visible difficulty knobs |
| **CPI** | < $2 | **Targeting ~$1.70-2.00** | Broad animal theme, clear ad readability |
| **D7 Retention** | > 20% | **Possible path** | Near-win loops and route mastery |
| **Prototype Scope** | 30-40 levels | **PASS** | Compact V1 with 4 obstacles |
| **VR01-VR06** | Strong pass | **53/60** | Better fit for hybrid casual |

---

## VR01-VR06 Validation Checklist

| VR | Criteria | Score | Notes |
|----|----------|-------|-------|
| **VR01** | Clear Puzzle Core | 9.5/10 | Place dogs, release flock, herd into safety |
| **VR02** | Newness and Twist | 8/10 | Clearer identity than draw-to-save |
| **VR03** | Fair Challenge and APS | 8.5/10 | Strong if turning rules stay deterministic |
| **VR04** | Game Feel | 9/10 | Dog sprint, flock bend, group flow payoff |
| **VR05** | Fast Prototype Scope | 8.5/10 | Tight V1, low feature risk |
| **VR06** | Publishability | 9/10 | Strong visual hook and clean fantasy |

**Overall Score:** 53/60 = 88 percent

Verdict: READY FOR PROTOTYPE V1

---

## Core Breakdown

```text
PLACE DOGS + TURN THE FLOCK + FILL SAFE PENS = HERDING PUZZLE
```

### What Makes It Different

| Element | Basic Rescue Puzzle | DogFlow |
|---------|--------------------|---------|
| **Player Goal** | Stop one bad event | Turn the whole flock into safety |
| **Decision Type** | Draw or shield | Place dogs and predict turn behavior |
| **Board Logic** | Single protection shape | Group movement redirection |
| **Progress** | Survive event | Fill pens safely and completely |
| **Payoff** | Threat avoided | Whole flock bends and lands perfectly |

### Why It Fits Voodoo Better Than a Simple Clone

- It uses a very readable fantasy.
- It adds one visible systemic twist.
- It stays in puzzle territory instead of simulation-heavy play.
- It avoids currently saturated red-ocean wrappers.

---

## APS Analysis

### APS Curve Design

| Level Block | APS Target | Difficulty Purpose |
|-------------|------------|-------------------|
| **1-10** | 1.10 - 1.20 | Teach draw, release, and pen entry |
| **11-20** | 1.25 - 1.40 | Introduce first dog turn decisions |
| **21-30** | 1.40 - 1.55 | Add capacities and chokepoints |
| **31-40** | 1.55 - 1.70 | Add two-dog setups and near-win states |
| **41-50** | 1.60 - 1.80 | Add tighter terrain logic and durability traps |

### APS Calculation

```text
APS = (1.15 x 10 + 1.35 x 10 + 1.475 x 10 + 1.65 x 10 + 1.75 x 10) / 50
APS = 73.75 / 50
APS = 1.475
```

Requirement: greater than 1.4

Result: PASS

### Main Difficulty Knobs

| Knob | Effect |
|------|--------|
| Number of sheep | Raises board pressure |
| Number of dogs | Raises setup complexity |
| Pen capacity | Forces split decisions |
| Dog placement spots | Controls freedom |
| Hazard placement | Raises tension visibly |
| Terrain funnels | Forces order |
| Breakable barriers | Creates late near-win failures |

---

## Obstacle Plan

| Obstacle | APS Impact | Purpose |
|----------|------------|---------|
| **Slot-Limited Pens** | Medium | Teach distribution |
| **One-Way Terrain** | Medium | Teach route order |
| **River Bridges** | Low-Medium | Visible danger and chokepoints |
| **Breakable Barriers** | Medium-High | Creates near-win tension |

### Progression

- Level 1-5: One flock, one dog, one obvious turn
- Level 6-15: Two pens, first slot-limited layouts
- Level 16-25: Add bridges and first terrain funnels
- Level 26-40: Add two-dog setups and combined route decisions

---

## Reference Direction

### Closest Mechanic Family

- `Save the Dog`: rescue readability
- `Flight Control`: pre-planned redirection
- sheepdog videos: emotional and visual fantasy reference

### Positioning Insight

The idea should be pitched as:

`A sheepdog placement puzzle with rescue stakes`

It should not be pitched as:

`Save the Dog with sheep`

---

## Risk Assessment

| Risk | Severity | Mitigation |
|------|----------|------------|
| Too close to rescue-clone framing | Medium | Make dog placement and flock turning central in every level |
| Sheep behavior feels chaotic | High | Deterministic movement, clear release phase |
| Too much visual noise | Medium | Small flock counts early, clean ranch layouts |
| Weak originality perception | Medium | Strong flock-turn moments and visible split-route moments |

---

## Prototype Roadmap

### Phase 1: Core Build

- Place dogs into valid setup positions
- Preview direction shift
- Release flock
- Check pen fill and fail states

### Phase 2: Level Set

- Build 10 onboarding levels
- Build 10 core split-route levels
- Build 10 pressure levels with first near-win patterns

### Phase 3: Test

- Internal playtest with APS tracking
- Check fail readability
- Validate ad-readable moments
- Use the `banana 2.0` block in `AI-PROMPT-3-LEVELS.md` for 3 level visual mockups
- Use the `aistudio.google.com` block in `AI-PROMPT-3-LEVELS.md` for the mechanic demo

---

## Final Recommendation

DogFlow is stronger in this version because:
- the core is clearer
- the dog fantasy is central
- the twist is easier to understand
- the scope is still disciplined

The critical production rule is simple:

`Keep the game puzzle-first and dog-turn-first.`

---

*Dashboard created: 2026-04-01*
