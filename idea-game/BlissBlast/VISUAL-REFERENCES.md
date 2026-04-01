# VISUAL REFERENCES: CONNECT CHAIN

> Level designs, UI mockups, and gameplay scenarios
> Status: Concept Phase

---

## 🎮 GAMEPLAY SCENARIOS

### SCENARIO 1: Basic Tutorial (Level 1-3)

**Objective:** Teach connection + first chain reaction

```
Level 1: Single Connection
┌──────────────────────┐
│ 💧 START  →  END 💧  │
│                      │
│ [Empty Grid]         │
│                      │
│ Instruction:         │
│ "Draw a pipe to      │
│  connect start       │
│  to end"             │
└──────────────────────┘

User action: Draw straight line
Result: Water flows → Simple success
Reward: Gentle "ding" sound + sparkle
```

---

```
Level 2: First Bomb
┌──────────────────────┐
│ 💧 START             │
│   ↓                  │
│ [Pipe]               │
│   ↓                  │
│ [💣] ← "Tap to arm"  │
│   ↓                  │
│ [Pipe]               │
│   ↓                  │
│ END 💧               │
└──────────────────────┘

User action: Draw through bomb
Result: Water flows → Bomb pulses → POP!
Reward: "BOOM!" sound + screen shake + confetti
```

---

```
Level 3: First Obstacle Clear
┌──────────────────────┐
│ 💧 START             │
│   ↓                  │
│ [Pipe]               │
│   ↓                  │
│ [💣] ← Chain trigger │
│   ↓                  │
│ [🧱 Wall] ← Blocked  │
│                      │
│ 💧 END (unreachable) │
└──────────────────────┘

User action: Draw through bomb
Result: Explosion! Wall destroyed → Path opens
Reward: Big explosion + "PATH CLEARED!" text
```

---

### SCENARIO 2: Strategic Choice (Level 10-15)

**Objective:** Multiple paths, different bomb placements

```
Level 12: Which Bomb?
┌──────────────────────────┐
│ 💧 START                 │
│   ↓                      │
│  [Choice Point]          │
│   ↙  ↘                  │
│ [💣A] [💣B]              │
│  ↓     ↓                 │
│ [Small] [Big]           │
│ [Area] [Area]            │
│   ↓     ↓                │
│ 💧 END 💧 END            │
└──────────────────────────┘

Option A: Use Bomb A
- Clears small area
- Saves 1 move
- Risk: Might not be enough later

Option B: Use Bomb B
- Clears big area
- Uses same moves
- Better for future planning

TEACHING MOMENT: Strategy matters!
```

---

### SCENARIO 3: Near-Win Design (Level 20-30)

**Objective:** Create 89-95% fail moments for IAP optimization

```
Level 25: "Just One More Pipe"
┌────────────────────────────┐
│ 💧 START                   │
│   ↓                        │
│ [Pipe][Pipe][Pipe]         │
│   ↓                        │
│ [💣] ← Used!               │
│   ↓                        │
│ [🧱][🧱][🧱][🧱] ← Cleared │
│                            │
│ [💧] ← Almost there!       │
│   ↓                        │
│ [🚧] ← 1 block remaining   │
│   ↓                        │
│ 💧 END 💧                   │
└────────────────────────────┘

Moves remaining: 0
Progress: 95%

FAIL MESSAGE: "So close! You're 1 pipe away!"
REVIVE BUTTON: "Continue? (+5 moves)"
    💝 Watch Ad
    💰 Use Coins

Near-win emotion: FRUSTRATION + HOPE
```

---

```
Level 28: "Wrong Turn"
┌────────────────────────────┐
│ 💧 START                   │
│   ↓                        │
│ [Pipe]                     │
│   ↓                        │
│ [💣 Bomb A] ← Chose this   │
│   ↓                        │
│ [🧱] ← Cleared area A      │
│                            │
│ [💣 Bomb B] ← Should have! │
│   ↓                        │
│ [🧱][🧱][🧱] ← Would clear │
│                            │
│ 💧 💧 💧 END (blocked)     │
└────────────────────────────┘

FAIL MESSAGE: "Try a different path!"
HINT BUTTON: "Reveal better route?"
    💝 Watch Hint
    💰 Buy Hint (3 coins)

Teaching moment: Planning ahead
```

---

### SCENARIO 4: Combo Chain (Level 30-40)

**Objective:** Maximum satisfaction, chain reaction payoff

```
Level 35: "Domino Effect"
┌──────────────────────────────┐
│ 💧 START                     │
│   ↓                          │
│ [💣 Bomb 1]                  │
│   ↓                          │
│ [💣 Bomb 2] ← Triggers 1&2   │
│   ↓                          │
│ [💣 Bomb 3] ← Triggers all!  │
│   ↓                          │
│ [🧱][🧱][🧱][🧱][🧱]          │
│ [🧱][🧱][🧱][🧱][🧱] ← Huge   │
│ [🧱][🧱][🧱][🧱][🧱]          │
│   ↓                          │
│ 💧 END 💧                     │
└──────────────────────────────┘

Sequence:
1. Water flows to Bomb 3
2. BOOM! Triggers 1, 2, 3 simultaneously
3. MASSIVE EXPLOSION (0.5s slow-mo)
4. Everything clears
5. Liquid reaches exit
6. Screen: "COMBO x3! PERFECT!"

Sound design:
- BOOM-BOOM-BOOM! (stereo effect)
- Chiming rewards
- "UNBELIEVABLE!" voice

Visual payoff:
- Screen shake
- Confetti explosion
- Rainbow path
- Hero character dances
```

---

## 🎨 UI/UX DESIGN

### Main Game Screen:
```
┌─────────────────────────────┐
│  🔙  Pipe Chain  ⚙️  💰    │ ← Top bar
├─────────────────────────────┤
│                             │
│  Level 15        Moves: 8   │ ← Status bar
│                             │
│  ┌─────────────────────┐   │
│  │                     │   │
│  │   💧 START          │   │
│  │     ↓               │   │
│  │   [Pipe Grid]       │   │ ← Game area
│  │     ↓               │   │
│  │    [💣]             │   │
│  │     ↓               │   │
│  │   💧 END            │   │
│  │                     │   │
│  └─────────────────────┘   │
│                             │
│  ┌───┐ ┌───┐ ┌───┐        │
│  │↩️ │ │💡 │ │🔄 │        │ ← Action bar
│  │Undo│ │Hint│ │Reset│    │
│  └───┘ └───┘ └───┘        │
└─────────────────────────────┘
```

### Level Complete Screen:
```
┌─────────────────────────────┐
│                             │
│      ⭐⭐⭐                 │
│   LEVEL COMPLETE!           │
│                             │
│   🎉 Great job! 🎉          │
│                             │
│   Moves: 5/8                │
│   Bonus: +150 coins         │
│                             │
│  ┌─────────────────────┐   │
│  │    ▶️ NEXT LEVEL     │   │
│  └─────────────────────┘   │
│                             │
│  [📺 Watch Ad for 2x bonus] │
└─────────────────────────────┘
```

### Fail / Revive Screen:
```
┌─────────────────────────────┐
│                             │
│      😢 Almost there!       │
│                             │
│   You're 1 pipe away!       │
│                             │
│  ┌─────────────────────┐   │
│  │   📺 CONTINUE       │   │
│  │   (Watch Ad)        │   │
│  └─────────────────────┘   │
│                             │
│  ┌─────────────────────┐   │
│  │   💰 +5 MOVES       │   │
│  │   (3 coins)         │   │
│  └─────────────────────┘   │
│                             │
│  [ 🔄 Restart Level ]       │
└─────────────────────────────┘
```

---

## 🎬 ANIMATION TIMELINE

### Standard Connection Success:
```
0.0s - User lifts finger (connection complete)
0.1s - Pipes glow blue (validation)
0.2s - Water starts flowing (animated sprite)
0.3s - Flow sound begins (water whoosh)
0.5s - Water reaches end
0.6s - End point flashes
0.7s - "SUCCESS!" stamp appears
0.8s - Coins fly to counter (if bonus)
1.0s - Level complete modal slides up
1.5s - Transition to next level
```

### Chain Reaction Explosion:
```
0.0s - Water reaches bomb
0.1s - Bomb pulses red (warning)
0.2s - Screen zooms in slightly
0.3s - BOOM! (screen shake)
0.3s - Explosion particles (30 particles)
0.4s - Debris flies outward
0.5s - Obstacles fade out
0.6s - New path glows gold
0.7s - "CHAIN REACTION!" text
0.8s - Water continues flowing
1.0s - Combo counter: x2, x3
1.5s - Normal completion sequence
```

### Fail Sequence:
```
0.0s - Moves counter reaches 0
0.1s - Grid shakes (warning)
0.2s - "OUT OF MOVES" text
0.3s - Camera pans to exit (shows how close)
0.5s - Sad trombone sound
0.6s - Fail modal slides up
0.8s - Revive options appear
```

---

## 🎵 SOUND DESIGN

### Core Sounds:
| Action | Sound | Duration | Feeling |
|--------|-------|----------|---------|
| **Pipe connect** | Click + snap | 0.1s | Satisfying |
| **Water flows** | Whoosh | 0.3s | Relief |
| **Bomb arm** | Tick-tock | 0.2s | Tension |
| **Explosion** | BOOM | 0.4s | Power |
| **Chain x2** | Ding-ding | 0.3s | Excitement |
| **Chain x3+** | Fanfare | 0.5s | Triumph |
| **Level complete** | Victory chord | 0.6s | Achievement |
| **Fail** | Sad trombone | 0.4s | Near-win |

### Music Layers:
- **Menu:** Upbeat, catchy (90 BPM)
- **Gameplay:** Calm focus (60 BPM)
- **Chain reaction:** Music swells + accelerates
- **Level complete:** Triumphant crescendo

---

## 📱 AD CREATIVE REFERENCES

### Ad Format 1: "Perfect Route" (15 seconds)
```
[0-3s] Failed attempt showing messy route
[3-6s] "Try this instead!" (hand draws clean route)
[6-9s] Bomb explodes, everything clears
[9-12s] "So satisfying!" + Level complete
[12-15s] CTA: "Can you solve it?"
```

### Ad Format 2: "One Pipe Away" (15 seconds)
```
[0-5s] Perfect play, almost at exit
[5-7s] "OUT OF MOVES" (1 pipe from goal)
[7-10s] "I can do better!" (reverse shows solution)
[10-12s] Success with bombs
[12-15s] CTA: "Think before you connect"
```

### Ad Format 3: "Chain Reaction Master" (30 seconds)
```
[0-10s] Fast-forward: 3 levels solved perfectly
[10-15s] Level 4: Complex setup shown
[15-20s] User connects ONE bomb
[20-25s] Massive chain reaction clears everything
[25-27s] "INSANE COMBO!" + Character celebrates
[27-30s] CTA: "Download now"
```

---

## 🎯 OBSTACLE LIBRARY (For Prototype V1)

### Obstacle 1: Locked Pipes
**Unlocks at:** Level 5
**Visual:** Chain/lock icon on pipe
**Mechanic:** Can't use until adjacent pipe connects
**Strategic:** Forces planning sequence
**APS Impact:** ↑ Low (adds order, not luck)

```
🔒 Pipe → Connect neighbor first → Unlocks
```

---

### Obstacle 2: One-Way Valves
**Unlocks at:** Level 10
**Visual:** Arrow indicator on pipe
**Mechanic:** Water only flows one direction
**Strategic:** Path planning crucial
**APS Impact:** ↑ Medium (requires reading ahead)

```
Pipe → → → Must follow arrows
```

---

### Obstacle 3: Timed Flow
**Unlocks at:** Level 18
**Visual:** Countdown timer on start pipe
**Mechanic:** Water starts flowing after X seconds
**Strategic:** Speed + accuracy
**APS Impact:** ↑↑ Medium-High (time pressure)

```
💧 (3...2...1...) → Flow starts automatically
```

---

### Obstacle 4: Color-Matched Bombs
**Unlocks at:** Level 25
**Visual:** Colored bomb (red, blue, green)
**Mechanic:** Only matching-colored liquid triggers
**Strategic:** Color routing decisions
**APS Impact:** ↑ High (complex planning)

```
🔵 Pipe → 🔵 Bomb → 💥
🔴 Pipe → 🔵 Bomb → ❌ (nothing)
```

---

## 📊 LEVEL DESIGN PATTERNS

### Pattern A: Tutorial (1-5)
- Single obvious solution
- Generous moves
- Teach one mechanic per level
- Success rate: 95%+

### Pattern B: Core Introduction (6-15)
- 2-3 valid solutions
- Moderate moves
- Introduce obstacles gradually
- Success rate: 70-85%

### Pattern C: Challenge Zone (16-30)
- Multiple solutions (3-5)
- Tighter moves
- Combine obstacles
- Near-win design built-in
- Success rate: 40-60%

### Pattern D: Master Levels (31-40)
- Complex planning
- Multiple viable strategies
- High chain reaction potential
- Satisfying payoff
- Success rate: 25-45%

---

*Visual references complete for IDEA 1: Connect Chain*
*Ready for prototype development*
