# AI PROMPT: 3 LEVEL GENERATION

> Use this prompt to generate 3 test levels for Block Blast City
> Can be used with: aistudio.google.com or any AI code/image generator
> Created: 2026-04-01

---

## 🎮 GAME SPECIFICATION

### Game Name: Block Blast City

**Core Concept:**
Connect-the-dots puzzle where drawing fuse lines through toy blocks triggers chain reaction explosions to demolish colorful block towers.

**Core Mechanics:**
1. **Action:** Draw fuse line from start point through toy blocks
2. **Trigger:** Fuse ignites → travels to endpoints
3. **Explosion:** Blocks at endpoints explode → chain reaction spreads
4. **Collapse:** Tower collapses due to physics
5. **Win:** All target blocks destroyed OR path to exit cleared

**Win Conditions:**
- Destroy all red-highlighted target blocks
- OR clear path to green exit zone

**Lose Conditions:**
- Run out of moves before destroying all targets
- OR explosives don't reach targets

**Visual Style:**
- Stylized toy blocks (colorful, rounded edges, 3D)
- Bright background (sky blue)
- Clean, minimal UI
- Explosive FX (particles, screen shake)

---

## 📋 LEVEL GENERATION REQUIREMENTS

### Level 1: TUTORIAL - "First Blast"
**Difficulty:** Easy
**APS Target:** 1.1-1.2
**Moves:** 3
**Goal:** Teach basic fuse drawing + single explosion

**Layout:**
```
Grid: 5x5
┌─────────────────┐
│  [Start] 🔵     │  ← Fuse start point (blue)
│     ↓           │
│  [Block] 🔴     │  ← Target block (red)
│     ↓           │
│  [Bomb] 💣      │  ← Explosive endpoint
└─────────────────┘
```

**Requirements:**
- Single obvious route
- Straight line only
- 1 target block
- Generous moves (3 needed, player has 5)
- Clear visual hint (dotted line showing route)

**Success Criteria:**
- 95%+ first-time completion
- User learns: Draw line → Block explodes
- Takes 5-10 seconds

---

### Level 2: CHAIN REACTION - "Double Trouble"
**Difficulty:** Easy-Medium
**APS Target:** 1.2-1.3
**Moves:** 5
**Goal:** Teach chain reaction mechanics

**Layout:**
```
Grid: 6x6
┌─────────────────────┐
│  [Start] 🔵         │
│     ↓               │
│  [Block A] 🔴       │  ← Target 1
│     ↓               │
│  [Bomb] 💣          │  ← Triggers chain
│     ↓               │
│  [Block B] 🔴       │  ← Target 2
└─────────────────────┘
```

**Requirements:**
- Linear chain (A explodes → B explodes)
- 2 target blocks
- Chain reaction essential
- 5 moves needed, player has 7
- Show chain preview (glowing line)

**Success Criteria:**
- 85%+ first-time completion
- User learns: Explosions spread to adjacent blocks
- Takes 10-15 seconds

---

### Level 3: STRATEGIC CHOICE - "Pick Your Path"
**Difficulty:** Medium
**APS Target:** 1.4-1.5
**Moves:** 8
**Goal:** Multiple solutions, strategic thinking

**Layout:**
```
Grid: 8x8
┌─────────────────────────────┐
│                             │
│   [Start] 🔵               │
│      ↙  ↘                  │
│   [Bomb A] [Bomb B]        │  ← Player choice
│     ↓        ↓             │
│  [Tower 1] [Tower 2]       │
│   (3🔴)    (2🔴)           │  ← Target counts
│                             │
│   [Exit] 🟢                 │  ← Exit zone
└─────────────────────────────┘
```

**Route Options:**

**Route A (Left):**
- Through Bomb A → Tower 1 collapses (3 targets)
- Moves: 4
- Leaves Tower 2 standing → Must also clear

**Route B (Right):**
- Through Bomb B → Tower 2 collapses (2 targets)
- Moves: 3
- Leaves Tower 1 standing → Must also clear

**Route C (Optimal):**
- Connect both bombs in one route
- Triggers both towers simultaneously
- Moves: 5
- Clears all targets in single chain

**Requirements:**
- 2-3 valid solutions
- No visual hints (player must figure out)
- 8 moves max (tight but doable)
- Strategic: Which bomb first?

**Success Criteria:**
- 60-70% first-time completion
- User learns: Planning matters, multiple solutions exist
- Takes 20-30 seconds
- Replay value (try different routes)

---

## 🎨 VISUAL SPECIFICATIONS

### Block Types:
| Block | Color | Size | Visual |
|-------|-------|------|--------|
| **Standard** | Blue/Orange | 64x64px | Rounded, 3D bevel |
| **Target** | Red + glow | 64x64px | Pulsing highlight |
| **Start** | Blue icon | 64x64px | Spark marker |
| **Bomb** | Black/Red | 64x64px | Fuse icon |
| **Exit** | Green zone | 128x64px | Open door/gate |

### Grid Specifications:
- Cell size: 64x64 pixels
- Grid lines: Subtle gray
- Background: Sky blue (#87CEEB)
- Spacing: 4 pixels between blocks

### UI Elements:
```
Top Bar:
┌─────────────────────────────┐
│ Level 3        Moves: 6/8   │
└─────────────────────────────┘

Bottom Bar:
┌─────────────────────────────┐
│ [↩️ Undo] [💡 Hint] [🔄 Restart] │
└─────────────────────────────┘
```

---

## 🎯 SUCCESS CRITERIA FOR ALL LEVELS

### Gameplay:
- [ ] Clear win condition (targets destroyed or exit reached)
- [ ] Clear lose condition (moves exhausted)
- [ ] No ambiguous states
- [ ] Predictable physics (same result each time)

### Visual:
- [ ] 3-second readability (user understands goal immediately)
- [ ] Clear contrast between targets and normal blocks
- [ ] Smooth animations (fuse draw, explosion, collapse)
- [ ] Satisfying payoff (visual + audio)

### Difficulty:
- [ ] Level 1: APS ~1.1 (95%+ success)
- [ ] Level 2: APS ~1.2 (85%+ success)
- [ ] Level 3: APS ~1.4 (60-70% success)

### User Experience:
- [ ] "One more try" feeling on fail
- [ ] "Aha!" moment on solution discovery
- [ ] Satisfying completion (dopamine hit)
- [ ] Clear progression (learning happens)

---

## 🤖 AI GENERATION PROMPT

### For Text-Based AI (ChatGPT, Claude):

```
You are a level designer for a mobile puzzle game called "Block Blast City".

GAME CONCEPT:
- Players draw fuse lines through toy blocks
- Fuses ignite and cause chain reaction explosions
- Goal: Destroy all red target blocks or reach exit
- Constraint: Limited moves per level

GENERATE 3 LEVELS:

LEVEL 1 (Tutorial):
- Grid: 5x5
- Goal: Teach basic fuse drawing
- Targets: 1 red block
- Moves: 5 available, 3 needed
- Layout: Simple linear path

LEVEL 2 (Chain Reaction):
- Grid: 6x6
- Goal: Teach chain mechanics
- Targets: 2 red blocks
- Moves: 7 available, 5 needed
- Layout: Linear chain reaction

LEVEL 3 (Strategic Choice):
- Grid: 8x8
- Goal: Multiple solutions
- Targets: 5 red blocks in 2 towers
- Moves: 8 available
- Layout: 2 bomb options, optimal route connects both

For each level, provide:
1. ASCII grid layout showing block positions
2. Move count (available/needed)
3. Step-by-step solution
4. Why this teaches the intended mechanic
5. Expected success rate

Make levels fun, fair, and satisfying!
```

---

### For Image/Visual AI (Midjourney, DALL-E):

```
PROMPT FOR LEVEL 1:
"Isometric toy block puzzle level, 5x5 grid, one red target block, blue start point, black bomb, simple linear path, bright colorful blocks, rounded edges, sky blue background, clean minimal UI, mobile game screenshot style"

PROMPT FOR LEVEL 2:
"Isometric toy block puzzle level, 6x6 grid, two red target blocks in chain formation, blue start point, bomb in middle, chain reaction path, colorful blocks, explosions, sparks, mobile game UI, clean and cheerful"

PROMPT FOR LEVEL 3:
"Isometric toy block puzzle level, 8x8 grid, two toy towers with red targets, multiple bomb options, strategic layout, complex paths, green exit zone, colorful blocks, mobile game interface, decision moment"
```

---

### For Code Generation (AI coding assistant):

```
Generate Unity C# code for Block Blast City level system:

REQUIREMENTS:
1. Grid-based level system (5x5, 6x6, 8x8 grids)
2. Block types: Standard, Target (Red), Start (Blue), Bomb, Exit (Green)
3. Fuse drawing system (touch/drag input)
4. Explosion chain reaction logic
5. Win/lose condition checking
6. Move counter system
7. Level data structure (serializable)

Include:
- Block class with properties (type, position, color)
- LevelManager class with level loading
- Fuse drawing handler
- Explosion chain logic
- Win/lose state management
- Sample level data for 3 levels

Make it clean, modular, and ready for prototyping!
```

---

## 📊 EXPECTED OUTPUTS

### From Text AI:
- Detailed ASCII layouts for each level
- Step-by-step solution walkthroughs
- Balance analysis (APS calculations)
- Teaching moment explanations

### From Image AI:
- Visual mockups showing block placement
- Colorful, stylized toy aesthetic
- Clear UI overlays (moves, targets)
- Isometric or top-down view

### From Code AI:
- Functional prototype code
- Ready to import into Unity/Godot
- 3 levels implemented and playable
- Basic game loop working

---

## ✅ VALIDATION CHECKLIST

After generating levels, verify:

**Level 1 (Tutorial):**
- [ ] Can be solved in one obvious way
- [ ] Takes < 10 seconds
- [ ] Teaches draw mechanic
- [ ] 95%+ expected success rate

**Level 2 (Chain):**
- [ ] Chain reaction clear
- [ ] Both targets destroyable
- [ ] Takes 10-15 seconds
- [ ] 85%+ expected success rate

**Level 3 (Strategy):**
- [ ] Multiple valid solutions exist
- [ ] Optimal route is discoverable
- [ ] Takes 20-30 seconds
- [ ] 60-70% expected success rate
- [ ] Creates "aha!" moment

**All Levels:**
- [ ] 3-second readability ✅
- [ ] Clear win/lose ✅
- [ ] Satisfying completion ✅
- [ ] Fair challenge ✅
- [ ] No hidden info ✅

---

## 🚀 NEXT STEPS AFTER GENERATION

1. **Review generated levels** - Check if they meet criteria
2. **Playtest manually** - Draw solutions, verify APS
3. **Adjust difficulty** - Tweak move counts if needed
4. **Create gray-box prototype** - Test in Unity
5. **User test** - 5-10 people try the levels
6. **Iterate** - Improve based on feedback

---

*AI prompt ready for use*
*Can generate levels within minutes*
*Framework: Block Blast City concept*
