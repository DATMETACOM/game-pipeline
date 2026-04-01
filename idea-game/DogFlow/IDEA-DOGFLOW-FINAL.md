# DOGFLOW - FINAL IDEA DOCUMENT

> Voodoo Idea Review Pack
> Created: 2026-04-01

---

## Executive Summary

**One-line Concept:**
Place sheepdogs to turn a running flock into the correct pens before any sheep falls into the river or off the cliff.

**Core Philosophy:**
Use a familiar rescue setup, then make the actual puzzle about placing sheepdogs that visibly turn flock movement in clean, readable ways.

**Voodoo Pass Status:** READY FOR PROTOTYPE V1

---

## 1. Core Mechanic (VR01)

### Player Action

```text
Place sheepdogs at valid setup points
Press release
Dogs sprint into blocking position
Sheep turn away from the dog line and run into safe pens
```

### Goal and Conditions

| Condition | Description |
|-----------|-------------|
| **Goal** | Herd the flock into the correct pens |
| **Win** | All sheep enter safe pens |
| **Lose** | A sheep falls into danger, passes the wrong route, or misses the safe setup |

### Core One-liner

Place sheepdogs so they turn the flock safely into the correct pens.

### 3-Second Readability

The player sees:
1. Sheep running toward danger
2. Dogs placed ahead of the flock
3. Faint arrows showing current running direction
4. Safe pens waiting beyond the turning points

The logic reads almost instantly.

---

## 2. Newness and Twist (VR02)

### Twist Definition

`Pre-place sheepdogs to redirect flock flow`

### What Remains Without the Twist

Without the dog-placement redirection system, it becomes a generic rescue game.

### Why the Twist Matters

- Multiple sheep react to the same setup
- The player predicts group movement instead of drawing a shield
- Dog placement creates a visible turning event
- Pens and terrain convert the fantasy into a puzzle

### Direction Safety

This is a safe Voodoo direction:
- familiar input
- new puzzle structure
- broad visual fantasy
- no dependence on a hot saturated puzzle wrapper

---

## 3. Fair Challenge and APS (VR03)

### Design Rules

- The whole board is visible before release.
- Sheep have faint direction arrows before release.
- Dogs always create the same kind of blocking pressure.
- Sheep turning rules are deterministic.
- Pen targets and hazards are always visible.
- No hidden spawn changes in onboarding.

### Multiple Solution Logic

From level 11 onward, levels should support at least two workable setup plans:
- direct aggressive redirection with tighter margin
- safer placement that bends the flock earlier

### APS Target Curve

| Level Block | APS Target | Purpose |
|-------------|------------|---------|
| **1-10** | 1.1 - 1.2 | Teach drawing, release, and safe entry |
| **11-20** | 1.25 - 1.4 | Introduce first split turns and wrong-route risk |
| **21-30** | 1.4 - 1.55 | Add pen capacities and terrain chokepoints |
| **31-40** | 1.55 - 1.7 | Add two-dog setups and near-win traps |
| **41-50** | 1.6 - 1.8 | Add one-way terrain and collapsing route supports |

### Overall APS Estimate

```text
APS = (1.15 x 10 + 1.35 x 10 + 1.475 x 10 + 1.65 x 10 + 1.75 x 10) / 50
APS = 1.475
```

Result: passes the Voodoo requirement of APS greater than 1.4.

### Near-Win Fail Patterns

1. One sheep slips around the final dog pressure line and misses the pen.
2. The flock turns correctly at first, but one late split goes toward the river.
3. The final dog setup is slightly too deep, leaving a small escape gap.

These fails should happen at 89-95 percent of progress whenever possible.

---

## 4. Game Feel (VR04)

### Main Action

Placing the dogs should feel direct and intentional, while the flock response should feel smooth and believable.

### Feedback Loop

1. Touch and drag places a dog into a valid setup point.
2. The game previews the dog's blocking line or pressure zone.
3. On release, the dog sprints into place.
4. The flock bends as a group and changes direction.
5. Each pen fills slot by slot with a satisfying count-up.
6. Final success closes the gate and triggers a clean ranch celebration.

### Pixar-Polish Layer

- Sheep: fluffy, expressive, slightly silly
- Dog: fast, smart, playful, sells the fantasy
- World: clean ranch, cliffs, bridges, river edges
- Materials: soft fur, wood, dust, grass motion, safe pen glow

Art production note:
- This package defines visual direction only.
- Use the `banana 2.0` block in `AI-PROMPT-3-LEVELS.md` for mockup generation.
- Use the `aistudio.google.com` block in `AI-PROMPT-3-LEVELS.md` for mechanic demo generation.

### Payoff

The highest dopamine moment is when the final dog turn works perfectly and the whole flock pours into the pen in one clean motion.

---

## 5. Prototype V1 Scope (VR05)

### Prototype Targets

| Metric | Target V1 |
|--------|-----------|
| **APS** | > 1.4 |
| **CPI** | Around $2 |
| **D1** | Around 35% |
| **D7** | Around 10% |
| **Playtime** | 20-30 minutes |

### Content Scope

- 30-40 handcrafted levels
- Around 1 hour of content
- One ranch biome
- One flock type
- One dog type
- No procedural generation in V1

### First 4 Obstacles

#### 1. Slot-Limited Pens
- Pens only accept a fixed number of sheep
- Forces distribution planning

#### 2. One-Way Terrain
- Terrain funnels the flock from only one side
- Creates placement order planning

#### 3. River Bridges
- Narrow safe passage across danger
- Makes turn precision matter

#### 4. Breakable Barriers
- A temporary terrain support opens after part of the flock passes
- Creates near-win route pressure

### Not Included in V1

- No farm meta
- No dog progression
- No economy or shop
- No booster system
- No revive system
- No wolves or enemy AI

---

## 6. Publishability (VR06)

### 3-Second Ad Readability

Frame 1 should show:
- sheep running toward cliff or river
- dogs placed in the path
- the flock visibly changing direction

The player should understand the challenge without text.

### Creative Hooks

**Hook 1: One Sheep Left**
- The route works for almost the whole flock.
- One sheep misses the final slot and falls.
- Viewer thinks: I can fix that.

**Hook 2: Bad Route vs Smart Route**
- First dog placement leaves a gap and fails.
- Second dog placement bends the flock cleanly and wins.

### CPI Thesis

- Animal rescue is broad-audience.
- The board reads cleanly in video.
- The dog-herding fantasy is emotionally sticky and easy to remember.
- Theme is not sitting inside the hottest saturated puzzle wrappers.

### Retention Thesis

- Near-win loops are easy to build.
- Placement and turn prediction add depth.
- Multiple workable setups make the game feel smarter than a simple rescue puzzle.

### Monetization Path

After prototype validation:
- hint ads
- revive at final sheep fail
- cosmetic dog, ranch, and sheep skins

### Execution Note

- Use `BANANA-MOCKUP-PROMPT.md` for static or staged visual mockups.
- Use `AISTUDIO-GAMEPLAY-PROMPT.md` for playable mechanic validation.

---

## 7. Reference Direction

### Input and Fantasy References

- `Save the Dog`: fast rescue readability
- `Flight Control` / `Harbor Master`: pre-planned redirection intuition
- real sheepdog videos: fantasy reference for flock turning payoff

### Positioning Rule

Do not present the game as a line-drawing clone.
Present it as a sheepdog placement puzzle with rescue stakes.

---

## 8. Final Evaluation

| VR | Result | Notes |
|----|--------|-------|
| **VR01** | PASS | Core is clear in one sentence |
| **VR02** | PASS | Dog placement is a clearer identity than line-drawing |
| **VR03** | PASS | APS 1.475, fair challenge improves with deterministic turning |
| **VR04** | PASS | Stronger cinematic payoff and character fantasy |
| **VR05** | PASS | Tight prototype scope |
| **VR06** | PASS | Good ad readability and broad theme |

### Score

53/60 = 88 percent

### Verdict

READY FOR PROTOTYPE V1

This version is stronger because it is easier to understand, more emotionally coherent, and still compact enough to test inside Voodoo's prototype framework.

---

*Final document created: 2026-04-01*
