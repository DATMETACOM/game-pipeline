# AI PROMPT: LEVELS, MOCKUPS, AND GAMEPLAY DEMO
# DogFlow - Sheepdog Placement Herding Puzzle

---

## How To Use This File

This file has 3 parts:
- Part A: shared level-design source of truth
- Part B: `banana 2.0` prompt for 3 level mockups
- Part C: `aistudio.google.com` prompt for mechanic demo generation

Use Part A as the base.
Then copy only Part B or Part C into the tool you are using.

---

## Part A - Shared Source Of Truth

## Role and Objective

You are a game level designer specializing in Voodoo-style puzzle and hybrid-casual mobile games.

Your task is to design 3 complete, playable levels for `DogFlow`, a puzzle game where the player places sheepdogs so they redirect a running flock into the correct pens before the sheep fall into danger.

The output must be detailed enough that a developer can implement the levels directly.

---

## Game Core Specification

### Basic Rules

1. The board contains:
   - sheep spawn points
   - valid dog setup points
   - one or more pens
   - visible hazards such as river or cliff
2. Before release, the player sees faint arrows showing the current sheep direction.
3. The player places dogs at setup points.
4. Each dog creates a predictable blocking or pressure line that the sheep will not cross.
5. After setup, the player taps `Release`.
6. Dogs sprint into position and the flock changes direction.
7. The level is won when all sheep enter valid pens safely.

### Lose Conditions

1. A sheep falls into the river or off the cliff.
2. A sheep enters the wrong pen or misses a turn.
3. A required pen overfills.
4. The flock passes through an unprotected gap and escapes safety.

### Prototype Constraints

- No boosters
- No revive
- No meta systems
- Deterministic sheep movement
- Planning puzzle first, reaction second
- Dog behavior must be simple and consistent

---

## APS Targets

| Level | Difficulty | APS Target | Design Purpose |
|-------|------------|------------|----------------|
| **Level 1** | Easy | 1.1 - 1.2 | Teach place, release, and first turn |
| **Level 2** | Medium | 1.3 - 1.5 | Introduce split-turn planning and pen capacity |
| **Level 3** | Hard | 1.6 - 1.8 | Near-win tension, multiple valid setups, tight constraints |

### APS Design Guidance

For Easy:
- one obvious dog placement
- one pen type or very simple split
- generous setup points

For Medium:
- two pens
- slot-limited pen or chokepoint
- two possible dog setups

For Hard:
- three-way tension or two-stage redirection
- at least one near-win fail pattern
- more than one valid setup, but one is clearly optimal

---

## Allowed Obstacles

### 1. Slot-Limited Pens
- Each pen accepts a fixed number of sheep.
- Forces routing distribution.

### 2. One-Way Terrain
- Sheep can safely turn only from one side.
- Creates order-based planning.

### 3. River Bridges
- Narrow passage over hazard.
- Increases visible tension without hidden rules.

### 4. Breakable Barriers
- A temporary support opens after a set number of sheep pass.
- Creates route order decisions and near-win moments.

---

## Visual and Theme Direction

### Art Direction

- Pixar-polish ranch world
- cute but readable sheep silhouettes
- smart sheepdog presentation
- soft wood pens, dust puffs, grass motion

Note:
- This file is the shared level-design source.
- bright but clean colors

### Readability Rules

- Sheep type and pen target must be readable instantly
- Pen capacities must be shown before release
- Hazards must be impossible to miss
- Dog influence area must be readable before release

---

## Required Output Format

For each of the 3 levels, provide:

### 1. Snapshot
- Level name
- Difficulty
- APS target
- Number of sheep
- Number of pens
- Obstacles used

### 2. Board Setup
- Describe the board layout clearly
- List spawn points
- List dog setup points
- List pen positions and capacities
- List hazards

### 3. Intended Solutions
- Best dog setup
- At least one alternate valid setup for medium and hard
- What common mistake players will make

### 4. Fail Design
- What near-win state can happen
- Why the fail still feels fair

### 5. Game Feel Notes
- What should feel satisfying in this level
- What visual moment should sell the level in a short ad

---

## Quality Checklist

Make sure your output satisfies all of these:

- The core is understandable in one sentence.
- The level can be read in 3 seconds.
- There is no hidden information.
- Dog placement effect is readable before release.
- Failures come from planning mistakes, not random behavior.
- The hard level includes a near-win fail at roughly 89-95 percent progress.

---

## Final Instruction

Design levels that prove `DogFlow` is a sheepdog placement puzzle, not a simple draw-to-defend game.

---

## Part B - Banana 2.0 Prompt

Copy the block below directly into `banana 2.0`.

```text
Create 3 readable mobile-game mockups for a hybrid casual puzzle game called DogFlow.

DogFlow is a sheepdog placement puzzle.
The player places sheepdogs before the flock runs.
When the level starts, the dogs sprint into blocking position and the flock changes direction.
The objective is to herd every sheep safely into the correct pens before any sheep falls into the river or off the cliff.

Visual direction:
- mobile hybrid-casual readability
- premium cartoon finish
- soft, cinematic, family-friendly ranch world
- cute but readable sheep silhouettes
- smart, playful sheepdogs
- clean terrain and obvious hazards
- strong depth separation between flock, dogs, pens, and danger
- bright but clean colors

Create 3 mockups:
1. Tutorial level
- one flock
- one dog
- one obvious safe pen
- one visible hazard
- clear faint arrow showing sheep running direction

2. Mid-core level
- one flock
- two pens
- one dog or two dogs
- first real redirection choice
- slot-limited pen visible

3. High-tension level
- larger flock
- two dogs
- river bridge or cliff edge
- near-win composition with one risky escape gap

Composition rules:
- vertical mobile framing
- top-down or slightly angled top-down camera
- sheep path readability is more important than background beauty
- dogs must be visually distinct from sheep and terrain
- pens must read as safe targets immediately
- hazards must read as fail states immediately
- faint direction arrows should be visible before release
- if a rope or influence line is shown, it should be subtle and supportive, not the visual headline

UI guidance:
- light gameplay UI only
- release button
- pen capacity indicators when relevant
- minimal top HUD
- no economy, store, or booster UI

Emotional goal:
- I understand what is happening immediately
- that flock turn looks satisfying
- I want to fix the route so every sheep gets into safety

Generate:
- 3 separate level mockups
- 1 optional collage sheet showing them side by side

Label them:
- Level 1 Tutorial
- Level 12 Core Split
- Level 32 Near-Win Pressure

Important:
Do not redesign the mechanic into line drawing, tower defense, or full simulation.
Keep the concept as:
place sheepdogs -> release flock -> redirect into safe pens
```

---

## Part C - Aistudio Gameplay Prompt

Copy the block below directly into `aistudio.google.com`.

```text
Build a small playable gameplay demo for a hybrid casual puzzle game called DogFlow.

The demo should prove one thing clearly:
placing sheepdogs before release can reliably redirect a flock into safe pens.

This is a mechanic-validation prototype only.
Do not build meta systems, economy, cosmetics, or complex AI.

Core concept:
The player sees a flock of sheep running toward danger.
Before the run starts, the player places one or more sheepdogs at valid setup positions.
When the player presses Release, the dogs sprint into blocking position.
The flock reacts by turning away from the dog pressure line and moving toward safe paths.
The level is won when all sheep enter the safe pens.

Required game loop:
1. Load level
2. Show sheep spawn points, pens, hazards, and valid dog setup positions
3. Show faint direction arrows for the sheep before release
4. Let player place dogs
5. Player presses Release
6. Dogs move into active blocking position
7. Sheep move forward and redirect according to dog placement
8. Check win or lose
9. Allow retry

Win condition:
- all sheep enter safe pens

Lose conditions:
- any sheep falls into a hazard
- any sheep misses the intended route and escapes safety
- any pen overfills, if capacity is used

System rules:
- sheep move at deterministic speed
- sheep follow their current forward direction until redirected
- sheep cannot cross active dog pressure lines
- when blocked, sheep turn toward the nearest valid open route according to a simple deterministic rule
- sheep should move as a readable group, not as chaotic physics bodies
- dogs are placed only at valid setup positions
- on release, each dog performs one consistent move into blocking position
- dogs act as player-controlled routing tools, not AI companions

Readability requirements:
- show faint arrows for sheep direction before release
- show dog influence line or pressure zone clearly enough that the player understands the turn logic
- hazards and pens must be obvious
- keep the board uncluttered

Prototype scope:
- 3 playable levels
- 1 sheep type
- 1 dog type
- 1 ranch biome
- retry flow only

Do not build:
- shop
- boosters
- skins
- revive economy
- procedural generation
- enemies
- narrative systems

Level targets:
Level 1
- one flock
- one dog
- one pen
- one visible hazard
- one obvious successful placement
- APS target: 1.1 - 1.2

Level 2
- one flock
- two pens or one pen plus chokepoint
- one meaningful turn decision
- APS target: 1.3 - 1.5

Level 3
- larger flock
- two dogs
- one near-win fail pattern
- APS target: 1.6 - 1.8

Feel targets:
- dog sprint should feel quick and decisive
- flock bend should feel smooth and satisfying
- pen entry should feel safe and rewarding
- final success should feel like the whole puzzle clicks into place

Technical goal:
- prioritize clarity
- prioritize determinism
- prioritize fast iteration
- prioritize visible cause and effect

Do not prioritize:
- advanced rendering
- realistic flock simulation
- elaborate camera behavior

Final instruction:
Generate the demo around this exact fantasy:
place sheepdogs -> release flock -> turn the group -> herd into safety
If the output drifts toward line drawing, tower defense, or uncontrolled simulation, simplify it back into a readable puzzle prototype.
```
