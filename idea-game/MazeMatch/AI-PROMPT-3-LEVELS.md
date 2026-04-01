# AI PROMPT: GENERATE 3 PLAYABLE LEVELS
# Maze Match Hero - Match-3 Pathfinding Puzzle Game

---

## 🎮 ROLE & OBJECTIVE

You are a **Game Level Designer** specializing in puzzle games for Voodoo-style hybrid casual mobile games.

**Your task:** Design and describe 3 complete, playable levels for "Maze Match Hero" - a Match-3 puzzle game where creating matches generates a path for the hero to reach the exit within limited moves.

**Target output:** Detailed level specifications that a developer can implement directly, including grid layouts, tile configurations, obstacle placements, path solutions, and visual descriptions.

---

## 📋 GAME CORE SPECIFICATION

### Basic Rules

**Player Action:**
1. Tap two adjacent tiles to swap them
2. If swap creates a match-3 or more of the same color:
   - Matched tiles disappear
   - Path tiles appear in their positions
   - Hero automatically moves along the generated path
3. Repeat until hero reaches the EXIT or runs out of moves

**Win Condition:** Hero reaches the EXIT tile before moves run out

**Lose Conditions:**
1. Move counter reaches 0 before hero reaches exit
2. Hero becomes blocked (no valid matches available)

**Valid Match Rules:**
- Standard Match-3 rules: 3+ same-colored tiles in a row or column
- Diagonal matches do NOT count
- L-shapes and T-shapes count as valid matches
- 4+ matches create power-ups (future feature, not in V1)

**Grid Size:**
- Tutorial/Onboarding (Level 1-5): 5x5 grid
- Standard (Level 6-30): 6x6 grid
- Advanced (Level 31-50): 7x7 or 8x8 grid

**Tile Colors:** 5 base colors
- Red (fire/warm)
- Blue (water/cool)
- Green (nature/earth)
- Yellow (light/energy)
- Purple (magic/mystery)

---

## 🎯 APS (ATTEMPT PER SUCCESS) TARGETS

**APS Definition:** Average attempts needed to pass one level

```
APS = Total Attempts / Total Successes
```

**Your Level Targets:**

| Level | Difficulty | APS Target | Player Success Rate | Purpose |
|-------|------------|------------|---------------------|---------|
| **LEVEL 1 (Easy)** | Tutorial | 1.1 - 1.2 | 83% - 91% | Teach basic mechanics, guarantee success |
| **LEVEL 2 (Medium)** | Core Introduction | 1.3 - 1.5 | 67% - 77% | Introduce strategic choices, fair challenge |
| **LEVEL 3 (Hard)** | Advanced | 1.6 - 1.8 | 56% - 63% | Multiple solutions, tight constraints, near-win moments |

**APS Implementation Guidelines:**

**For APS 1.1-1.2 (Easy):**
- Single obvious solution path
- Generous move count (can make 2-3 mistakes)
- No obstacles or very simple obstacles
- Clear hints (highlight suggested moves)
- All necessary tiles visible and accessible

**For APS 1.3-1.5 (Medium):**
- 2-3 valid solution paths
- Moderate move count (can make 1-2 mistakes)
- 1-2 obstacle types
- Some strategic choice required
- Multiple approaches possible

**For APS 1.6-1.8 (Hard):**
- 3+ valid solution paths (some optimal, some suboptimal)
- Tight move count (little room for error)
- 2-3 obstacle types combined
- Requires planning and optimization
- Near-win moments at 89-95% progress

---

## 🚧 OBSTACLE TYPES (Use in Your Designs)

### Obstacle 1: Locked Tiles 🔒
**Description:** Tiles with a chain/lock that can only be cleared by matching a specific color

**Rules:**
- Locked tiles cannot be swapped
- Locked tiles are cleared when adjacent match of required color is made
- Once cleared, they become normal empty tiles for path generation

**Visual:**
- Chain/lock icon overlay on tile
- Color indicator shows which match unlocks it

**APS Impact:** ↑ Low (adds planning, requires color matching)

**Use in levels:** 2 (Medium) and 3 (Hard)

---

### Obstacle 2: One-Way Paths ➡️
**Description:** Path tiles with arrows showing movement direction

**Rules:**
- Hero can only move in the direction of the arrow
- Cannot reverse direction on one-way path tiles
- Creates timing and sequence constraints

**Visual:**
- Arrow indicators on path tiles
- Glowing directional trail

**APS Impact:** ↑ Medium (requires reading ahead, planning sequence)

**Use in levels:** 3 (Hard)

---

### Obstacle 3: Dead Ends 🚫
**Description:** Tiles that, if matched, create a path leading nowhere

**Rules:**
- Not a direct obstacle, but a strategic trap
- Player must avoid creating paths to dead ends
- Forces strategic thinking about path direction

**Visual:**
- Subtle visual hint (slightly darker tiles)
- Only revealed upon inspection

**APS Impact:** ↑ Low-Medium (teaches strategic planning)

**Use in levels:** 2 (Medium) and 3 (Hard)

---

### Obstacle 4: Limited Color Palette 🎨
**Description:** Level has fewer tile colors available

**Rules:**
- Grid only contains 2-3 colors instead of 5
- Makes matches easier but requires more strategic planning
- Can create unintended matches (accidental path generation)

**Visual:**
- Grid shows only available colors
- Missing colors appear grayed out in UI

**APS Impact:** Variable (easier matches, but less control)

**Use in levels:** 1 (Easy) - 3 colors only

---

## 🎨 VISUAL STYLE & THEME

### Art Direction: Pixar-like Polish

**Overall Aesthetic:**
- Bright, saturated colors (Royal Match style)
- Smooth, high-quality animations
- Expressive characters with personality
- Clean, readable UI with depth and polish
- Magical glow effects for paths

**Character Design:**
- **Hero:** Small, adorable adventurer (think: Minion + Woody)
  - Expressive face (excited, determined, confused on fail)
  - Smooth walk/run animations
  - Celebration dance on victory
  - Sad pose with "try again" expression on defeat
  - Size: About 1/3 of tile size, sits on path tiles

**Environment:**
- **Background:** Magical forest/castle theme (soft focus, not distracting)
- **Tiles:** 3D or high-quality 2.5D with depth
  - Rounded corners, soft shadows
  - Gem-like appearance with inner glow
  - Color-coded with subtle symbols inside
- **Path:** Glowing magical trail (gold/white light)
  - Sparks/particles along the path
  - Pulsing glow effect
- **Exit:**
  - Easy levels: Wooden door or treasure chest
  - Medium: Stone archway or portal
  - Hard: Glowing portal with particle effects

**UI Elements:**
- **Moves Counter:** Large, visible, countdown animation
- **Score/Progress:** Not needed for V1 (focus on moves)
- **Hints:** Subtle sparkle on suggested tiles (Easy levels only)

---

## 🎮 GAME FEEL SPECIFICATIONS

### Feedback Sequence (Per Match)

**Step 1: Tile Selection (0.1s)**
- Visual: Tile scales up slightly, glow effect
- Audio: Soft "pop" sound

**Step 2: Swap Animation (0.2s)**
- Visual: Smooth tile swap animation
- Audio: "Whoosh" sound

**Step 3: Match Detection (0.3s)**
- Visual:
  - Matched tiles scale up then burst
  - Particle explosion (color-coordinated)
  - Screen shake (subtle)
- Audio: Satisfying "crunch" or "pop" sound

**Step 4: Path Generation (0.4s)**
- Visual:
  - Empty tiles fill with path tiles
  - Glowing path appears from hero position
  - Path pulses from start to end
- Audio: Magical "chime" or "ding" sound

**Step 5: Hero Movement (0.5s per tile)**
- Visual:
  - Hero walks along path (smooth animation)
  - Path lights up as hero travels
  - Hero shows determined/excited expression
- Audio: Footstep sounds, soft "hum" while moving

**Step 6: Path Complete (0.3s)**
- Visual:
  - Full path glows brighter
  - Hero celebrates small (thumbs up, smile)
- Audio: Musical " flourish" or positive chord

**Step 7: Level Complete**
- Visual:
  - Hero jumps/dances at exit
  - Exit bursts with particles
  - "VICTORY" text appears with animation
  - Confetti or fireworks
- Audio: Triumphant fanfare, multi-layered music

**Step 8: Level Failed**
- Visual:
  - Hero shows confused/sad expression
  - "OUT OF MOVES" text appears
  - "Try Again?" button with hero giving hopeful look
- Audio: Sad but encouraging "womp-womp" sound

---

## 📐 LEVEL DESIGN TEMPLATE

For each level, provide:

### 1. Level Overview
- Level number & difficulty
- Grid size
- Total moves allowed
- Obstacles present
- APS target
- Estimated completion time

### 2. Visual Layout
```
Example format:
[S] [R] [G] [Y] [P]
[R] [B] [G] [Y] [P]
[R] [B] [G] [Y] [P]
[R] [B] [G] [Y] [P]
[R] [B] [G] [Y] [E]

Legend:
[S] = Start (Hero position)
[E] = Exit
[R] = Red tile
[G] = Green tile
[Y] = Yellow tile
[B] = Blue tile
[P] = Purple tile
[L] = Locked tile (with color)
[→] = One-way path
```

### 3. Tile Configuration
- Number of each color tile
- Total tiles vs. empty tiles
- Special tile placements

### 4. Solution Paths
Provide **minimum 2 solution paths** for Medium, **minimum 3** for Hard:

**Solution Path A (Optimal):**
- Step-by-step moves
- Total moves used
- Colors matched in sequence
- Path generated

**Solution Path B (Alternative):**
- Different approach
- May use more moves
- Shows multiple solutions exist

**Solution Path C (Suboptimal but valid - Hard only):**
- Works but wastes moves
- Creates near-win moment (89-95% progress)
- Good for teaching optimization

### 5. Strategic Choices
- What decisions must the player make?
- Where are the branching points?
- What makes this level interesting?

### 6. Fail Scenarios
- Common mistakes players might make
- How the level creates near-win moments
- What feedback player receives

### 7. Visual Description
- Overall theme/setting for this level
- Background elements
- Exit type
- Any special visual elements

---

## 🎯 YOUR TASK: DESIGN 3 LEVELS

### LEVEL 1: TUTORIAL - "FIRST STEPS"
**Difficulty:** Easy
**APS Target:** 1.1 - 1.2
**Grid:** 5x5
**Obstacles:** None
**Colors:** 3 only (Red, Green, Blue)
**Moves:** 15
**Purpose:** Teach core mechanics, guarantee success

**Requirements:**
- Single obvious solution
- Can make 2-3 mistakes and still win
- No obstacles
- Clear visual hints
- Hero visible at start, exit clearly marked
- First match should be obvious (3 same colors visible and adjacent)
- Path generation should be straightforward (linear, no branches)

---

### LEVEL 2: STRATEGIC CHOICE - "FORK IN THE ROAD"
**Difficulty:** Medium
**APS Target:** 1.3 - 1.5
**Grid:** 6x6
**Obstacles:** Locked Tiles (1-2), Dead Ends
**Colors:** 4 (Red, Green, Blue, Yellow)
**Moves:** 12
**Purpose:** Introduce strategic decisions, multiple solutions

**Requirements:**
- 2-3 valid solution paths
- 1-2 locked tiles that require specific color matches
- At least 1 dead end trap (teach planning)
- Can make 1-2 mistakes and still win
- Requires some planning ahead
- Not immediately obvious solution
- Player must choose between shorter/harder path or longer/easier path

---

### LEVEL 3: MASTER PLANNER - "THE GAUNTLET"
**Difficulty:** Hard
**APS Target:** 1.6 - 1.8
**Grid:** 7x7
**Obstacles:** Locked Tiles (2-3), One-Way Paths, Dead Ends
**Colors:** All 5 (Red, Green, Blue, Yellow, Purple)
**Moves:** 10
**Purpose:** Tight constraints, multiple solutions, near-win moments

**Requirements:**
- 3+ valid solution paths (with different move efficiencies)
- 2-3 locked tiles with different color requirements
- 1-2 one-way path sections
- Multiple dead end traps
- Very tight move count (little room for error)
- Requires careful planning and optimization
- At least 1 near-win moment (89-95% progress)
- Optimal solution uses all or nearly all moves
- Suboptimal solutions create "just 1 more move" feeling

---

## ✅ SUCCESS CRITERIA

Your level designs will be evaluated on:

1. **APS Accuracy**
   - [ ] Easy level truly achievable in 1-2 attempts (APS 1.1-1.2)
   - [ ] Medium level requires some thought but solvable (APS 1.3-1.5)
   - [ ] Hard level challenging but fair (APS 1.6-1.8)

2. **Multiple Solutions**
   - [ ] Medium: 2-3 valid paths
   - [ ] Hard: 3+ valid paths

3. **Fair Challenge**
   - [ ] No hidden information
   - [ ] Clear goals
   - [ ] Readable strategy (board shows planning possibilities)
   - [ ] Fail feels fair (near-win, not random)

4. **Strategic Depth**
   - [ ] Meaningful choices (not just random matching)
   - [ ] Different approaches have different tradeoffs
   - [ ] Planning ahead is rewarded

5. **Visual Clarity**
   - [ ] Grid layout is easy to understand
   - [ ] Obstacles are clearly marked
   - [ ] Solution paths are traceable
   - [ ] Theme is consistent

6. **Game Feel**
   - [ ] Clear progression (see path building)
   - [ ] Satisfying payoff (complete path, reach exit)
   - [ ] Appropriate difficulty curve

---

## 📤 OUTPUT FORMAT

Please provide your response in this exact format:

```markdown
# LEVEL 1: FIRST STEPS (Tutorial - Easy)

## Level Overview
[Fill in overview details]

## Visual Layout
[Show grid using ASCII art]

## Tile Configuration
[Specify tile counts and placement]

## Solution Paths

### Solution Path A: The Obvious Route
[Step-by-step walkthrough]

### Solution Path B: The Learning Route
[Alternative approach, if applicable]

## Strategic Choices
[What decisions/learning happens]

## Fail Scenarios
[How player might fail, feedback]

## Visual Description
[Theme, setting, exit type]

---

# LEVEL 2: FORK IN THE ROAD (Medium)

[Same structure as above]

---

# LEVEL 3: THE GAUNTLET (Hard)

[Same structure as above]

---

## SUMMARY: APS VALIDATION

[Table showing all 3 levels with calculated APS]

## DESIGN NOTES
[Any additional insights about the level progression, difficulty curve, or design philosophy]
```

---

## 🎨 BONUS: VISUAL MOCKUP DESCRIPTIONS

For each level, also include a **"Visual Mockup"** section describing:
- What the player sees when level loads
- Key visual elements that draw attention
- How the path looks when generated
- What the victory/defeat moments look like
- Any special visual effects unique to this level

---

## 🚀 READY TO BEGIN

You now have all the specifications needed to design 3 complete, playable levels for "Maze Match Hero."

**Remember:**
- Focus on FAIR CHALLENGE (not luck-based)
- Ensure MULTIPLE SOLUTIONS (for Medium/Hard)
- Create NEAR-WIN moments (89-95% progress)
- Keep APS targets in mind (1.1-1.2, 1.3-1.5, 1.6-1.8)
- Make it satisfying to play (progress visible, payoff clear)

**Begin your level designs now!**

---

*Prompt version: 1.0*
*Game: Maze Match Hero*
*Framework: Voodoo March 2026*
*Created: 2026-03-31*
