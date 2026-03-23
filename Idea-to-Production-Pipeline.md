# 🚀 Quy Trình Từ Idea Đến Sản Xuất (Idea-to-Production Pipeline)

> **Mục tiêu**: Biến một idea thô sơ thành một game concept hoàn chỉnh, sẵn sàng cho sản xuất
> **Khách hàng mục tiêu**: Voodoo (Hybrid-Casual / Puzzle)
> **Cập nhật**: Tháng 3/2026

---

## 📋 TỔNG QUAN QUY TRÌNH

```
┌─────────────────────────────────────────────────────────────────────────────┐
│                    IDEA TO PRODUCTION PIPELINE                               │
├─────────────────────────────────────────────────────────────────────────────┤
│                                                                              │
│  PHASE 1          PHASE 2          PHASE 3          PHASE 4                 │
│  ────────         ────────         ────────         ────────                │
│  DISCOVERY   →    CONCEPT    →     VALIDATION  →    PRODUCTION              │
│  (Khám phá)       (Ý tưởng)        (Kiểm chứng)      (Sản xuất)             │
│                                                                              │
│  Week 1           Week 2            Week 3-4          Week 5+               │
│                                                                              │
└─────────────────────────────────────────────────────────────────────────────┘
```

---

## 🔷 PHASE 1: DISCOVERY (Khám phá)

### Mục tiêu
Tìm ra các ý tưởng tiềm năng dựa trên dữ liệu thị trường và xu hướng.

---

### Bước 1.1: Nghiên cứu Market References

#### 📌 Options để tham khảo:

| Option | Mô tả | Độ ưu tiên |
|--------|-------|------------|
| **A. Game Hyper-casual cũ (2018-2021)** | Đã chứng minh CPI thấp, marketability cao | ⭐⭐⭐⭐⭐ |
| **B. Game Hybrid-casual đang hot** | Có core puzzle + meta progression | ⭐⭐⭐⭐ |
| **C. Game Indie / PC / Console** | Cơ chế độc đáo, có thể đơn giản hóa | ⭐⭐⭐ |
| **D. Trend TikTok / Social Media** | Viral potential cao | ⭐⭐⭐ |

#### 💡 Tại sao chọn Game Hyper-casual cũ?

> **Lý do từ Voodoo**: Các game hyper-casual cũ (Hole.io, Paper.io, Stack Ball...) đã được chứng minh về khả năng thu hút người dùng với CPI cực thấp. Lấy "vỏ bọc" này và đắp thêm core puzzle là chiến lược hiệu quả nhất.

**Ví dụ thành công:**
- **Hole in Home** = Trải nghiệm "hố đen" từ Hole.io + Core Match-3 từ Match Factory
- **Color Box Jam** = Core từ Closkiy Sluzle + Trải nghiệm "nghiền nát" đã mắt
- **Scudom** = Logic Sort Game + Trải nghiệm đồ chơi 3D vật lý

#### ✅ Checklist Bước 1.1:

- [ ] Liệt kê 5-10 game hyper-casual cũ có CPI thấp (download cao)
- [ ] Liệt kê 5-10 game hybrid-casual đang thành công
- [ ] Phân tích core mechanic của từng game
- [ ] Ghi chú trải nghiệm/visual style đặc biệt
- [ ] Tìm các cơ chế có thể kết hợp được

---

### Bước 1.2: Phân tích Core Mechanics

#### 📌 Framework phân tích:

```
Mỗi game reference cần trả lời:
├── INPUT: Người chơi làm gì? (Tap, Swipe, Drag, Hold)
├── GOAL: Mục tiêu là gì? (Clear, Collect, Build, Survive)
├── WIN: Khi nào thắng?
├── LOSE: Khi nào thua?
├── FEEDBACK: Visual/Audio response?
└── HOOK: Điều gì khiến người chơi muốn tiếp tục?
```

---

#### 🧩 PUZZLE CATEGORIES (Danh sách đầy đủ)

> **Yêu cầu từ Voodoo**: Game PHẢI có yếu tố Puzzle (Level-based, Lose condition, Revive)

##### 📊 Puzzle theo Core Mechanic:

| Category | Sub-types | Mô tả | Ví dụ game |
|----------|-----------|-------|------------|
| **SORT** | Color Sort | Sắp xếp theo màu vào container | Water Sort, Fill Fridge |
| | Shape Sort | Sắp xếp theo hình dáng | Button Sort, Ball Sort |
| | Type Sort | Sắp xếp theo loại đối tượng | Goods Sort, Organize games |
| | Stack Sort | Xếp chồng theo quy tắc | Stack colors, Tower sort |
| **MATCH** | Match-3 | Đổi chỗ để tạo 3+ giống nhau | Candy Crush, Royal Match |
| | Match-3D | Tìm cặp giống nhau trong 3D | Match 3D, Triple Match |
| | Pair Match | Tìm cặp đôi | Mahjong, Memory match |
| | Merge | Gộp 2 giống nhau thành mới | Merge Dragons, 2048 |
| **DRAW** | Draw to Complete | Vẽ phần thiếu để hoàn thành | DOP, Draw One Part |
| | Draw Path | Vẽ đường đi cho object | Love Balls, Happy Glass |
| | Draw Shape | Vẽ hình theo yêu cầu | Draw Something |
| | Draw to Cut | Vẽ để cắt | Cut the Rope, Rope Cut |
| **PHYSICS** | Pin/Remove | Rút ghim/loại bỏ để physics hoạt động | Pull the Pin, Pin Pull |
| | Balance | Cân bằng objects | Balance games |
| | Gravity | Điều khiển trọng lực | Gravity puzzles |
| | Chain Reaction | Tạo phản ứng dây chuyền | Amazing Alex |
| **LOGIC** | Sequence | Tìm thứ tự đúng | Sequence games |
| | Pattern | Nhận diện pattern | Pattern Match |
| | Deduction | Suy luận logic | Brain Test, Logic puzzles |
| | Math/Number | Toán học, số học | 2048, Sudoku |
| **WORD** | Word Search | Tìm từ trong bảng | Word Search |
| | Crossword | Điền từ chéo | Crossword |
| | Word Connect | Nối chữ tạo từ | Wordscapes |
| | Anagram | Sắp xếp lại chữ | Anagram games |
| **SLIDING** | Tile Slide | Trượt các ô | 15 Puzzle, Sliding block |
| | Pipe/Road | Nối ống/đường | Pipe Mania |
| | Flow | Nối điểm cùng màu | Flow Free |
| **HIDDEN OBJECT** | Find Items | Tìm đồ vật ẩn | Hidden City |
| | Spot Difference | Tìm điểm khác biệt | Spot the Difference |
| | Shadow Match | Tìm hình khớp bóng | Shadow games |
| **SCREW/BOLT** | Unscrew | Tháo ốc/bu lông | Screw Pin Puzzle |
| | Bolt Sort | Sắp xếp ốc theo màu | Screw Sort |
| | Nuts & Bolts | Tháo lắp ốc vít | Wood Nuts & Bolts |

##### 📊 Puzzle theo Complexity Level:

| Level | Đặc điểm | Ví dụ |
|-------|----------|-------|
| **Simple** | 1-2 rules, dễ hiểu ngay | Water Sort, Match-3 |
| **Medium** | Nhiều rules, cần suy nghĩ | Pull the Pin, Sliding |
| **Complex** | Nhiều systems kết hợp | Royal Match (Match-3 + Meta) |
| **Hybrid** | Kết hợp nhiều puzzle types | Merge Mansion (Merge + Meta) |

##### 📊 Puzzle theo Session Length:

| Type | Thời gian/level | Phù hợp |
|------|-----------------|---------|
| **Bite-sized** | 10-30 giây | Hyper-casual,通勤 |
| **Short** | 30-90 giây | Casual, break time |
| **Medium** | 2-5 phút | Traditional puzzle |
| **Long** | 5-15 phút | Hardcore puzzle fans |

---

#### 💥 DESTRUCTION ELEMENTS (Yếu tố Phá hủy)

> **Yêu cầu từ Voodoo**: Game PHẢI có yếu tố Destruction (Cảm giác "đã mắt", vui nhộn, thu hút trong quảng cáo)

##### 📊 Destruction Categories:

| Category | Types | Mô tả | Feel |
|----------|-------|-------|------|
| **CRUSH/SMASH** | Impact smash | Đập vỡ bằng lực | Stack Ball |
| | Press crush | Ép nát | Hydraulic press games |
| | Hammer smash | Đập bằng búa | Smash games |
| | Weight crush | Nghiền bằng vật nặng | Crushing games |
| **CUT/SLICE** | Straight cut | Cắt đường thẳng | Fruit Ninja |
| | Slice through | Cắt xuyên qua | Soap Cutting |
| | Carve | Khắc/tạc | Wood Carving |
| | Shred | Xé nhỏ | Paper Shredder |
| **MELT/DISSOLVE** | Heat melt | Tan chảy bằng nhiệt | Melting games |
| | Acid dissolve | Tan trong axit | Dissolve puzzles |
| | Water erode | Erode bởi nước | Erosion games |
| **EXPLODE/BLAST** | Single explosion | Nổ đơn | Bomb puzzles |
| | Chain explosion | Nổ dây chuyền | Chain reaction |
| | Color blast | Nổ theo màu | Match-3 blast |
| **ABSORB/CONSUME** | Hole absorb | Hố đen hút | Hole.io |
| | Character eat | Nhân vật ăn | Hungry games |
| | Vacuum suck | Hút bằng máy hút | Vacuum games |
| **BREAK/DISASSEMBLE** | Structure break | Phá vỡ cấu trúc | Breaker games |
| | Unscrew/disassemble | Tháo gỡ | Screw puzzles |
| | Peel/strip | Bóc tách | Peeling games |
| **SHRED/GRIND** | Grinder | Xay/nghiền | Grinder games |
| | Shredder | Băm nhỏ | Shredder games |
| | Crush into pieces | Vỡ thành mảnh | Crushing games |
| **BURN/INCINERATE** | Fire burn | Đốt cháy | Burn puzzles |
| | Laser cut | Cắt bằng laser | Laser games |
| | Flame throw | Phun lửa | Fire games |

##### 📊 Destruction Intensity Levels:

| Level | Mô tả | Ví dụ | Appropriate for |
|-------|-------|-------|-----------------|
| **Subtle** | Nhẹ nhàng, thỏa mãn âm thầm | Pop bubbles | Relaxing games |
| **Moderate** | Rõ ràng, đã tay | Match-3 blast | Casual puzzle |
| **Intense** | Mạnh mẽ, kích thích | Stack Ball smash | Hyper-casual |
| **Extreme** | Bạo lực (hài hước), quá đã | Complete destruction | Stress relief games |

##### 📊 Destruction Feedback Elements:

| Element | Purpose | Implementation |
|---------|---------|----------------|
| **Particles** | Visual satisfaction | Debris, fragments, dust |
| **Screen Shake** | Impact feel | Camera shake on destruction |
| **Sound FX** | Audio satisfaction | Crunch, smash, snap sounds |
| **Slow-mo** | Emphasize moment | Slow down on big destruction |
| **Vibration** | Tactile feedback | Haptic on mobile |
| **Color Flash** | Visual pop | Flash white/bright on impact |
| **Debris Physics** | Realism | Physics-based fragments |

---

#### 🎮 Mechanics Library để kết hợp:

| Category | Mechanics | Ví dụ game |
|----------|-----------|------------|
| **Movement** | Swipe, Tap, Hold/Release, Auto-run | Helix Jump, Stack Ball |
| **Physics** | Ragdoll, Gravity, Bounce | Flappy Bird, Stack |
| **Collection** | Magnetic, Choice Gates, Multipliers | Crowd City, Tall Man Run |
| **Destruction** | Break/Smash, Cut/Slice, Clear | Stack Ball, Soap Cutting |
| **Growth** | Size, Number, Power | Agar.io, Crowd City |
| **Territory** | Trail Conquest, Absorb | Paper.io, Hole.io |
| **Timing** | Rhythm, Precision | Tiles Hop, Stack |
| **Puzzle** | Sort, Draw, Physics, Logic | Water Sort, DOP, Pull the Pin |

#### ✅ Checklist Bước 1.2:

- [ ] Phân tích tối thiểu 10 game references theo framework
- [ ] Xác định mechanics có tính "marketability" cao
- [ ] Tìm các mechanics có thể kết hợp (Puzzle + Destruction)
- [ ] Loại bỏ các mechanics đã bão hòa (Screw Loop, Pixel Flow)

---

### 🔥 Bước 1.2.1: PUZZLE + DESTRUCTION FRAMEWORK (Yêu cầu cốt lõi từ Voodoo)

> ⚠️ **QUAN TRỌNG**: Đây là yêu cầu BẮT BUỘC từ Voodoo cho game Hybrid Puzzle
>
> **Nhiệm vụ**: Kết hợp giữa **PUZZLE** (Giải đố) và **DESTRUCTION** (Phá hủy)
>
> **Tiêu chuẩn bắt buộc**:
> | Yếu tố | Yêu cầu |
> |--------|---------|
> | **Puzzle** | Level-based, Lose condition, Revive |
> | **Destruction** | Cảm giác "đã mắt", vui nhộn, thu hút trong quảng cáo |
> | **Cấm** | ❌ Endless game |

#### 📌 Cách tư duy sáng tạo (theo Voodoo):

```
┌─────────────────────────────────────────────────────────────┐
│            PUZZLE + DESTRUCTION MINDSET                      │
├─────────────────────────────────────────────────────────────┤
│                                                              │
│  ❌ KHÔNG: Sáng tạo từ con số 0                              │
│  ✅ NÊN: Dựa trên game đã thành công trên thị trường        │
│  ✅ NÊN: Kết hợp và "xào nấu" lại                           │
│                                                              │
│  VÍ DỤ - Screw Loop:                                        │
│  ├── Sử dụng lại: Ma trận + Dock dưới đáy màn hình         │
│  ├── Thêm mới: Băng chuyền di chuyển                        │
│  └── Twist: Thay vì cuộn len → Phá hủy bức tranh           │
│                                                              │
└─────────────────────────────────────────────────────────────┘
```

#### 🎯 16 COMBINATION PATTERNS (Puzzle × Destruction):

| # | Puzzle Type | Destruction Type | Concept | Marketability |
|---|-------------|------------------|---------|---------------|
| 1 | **Sort** | Crush/Smash | Sắp xếp → Nghiền nát khi hoàn thành | ⭐⭐⭐⭐⭐ |
| 2 | **Sort** | Absorb | Sắp xếp → Hố đen hút sai màu | ⭐⭐⭐⭐ |
| 3 | **Match-3** | Blast/Explode | Match → Nổ tung | ⭐⭐⭐⭐⭐ |
| 4 | **Match-3** | Crush | Match → Ép nát | ⭐⭐⭐⭐ |
| 5 | **Draw** | Cut/Slice | Vẽ → Cắt theo đường vẽ | ⭐⭐⭐⭐⭐ |
| 6 | **Draw** | Burn | Vẽ → Đốt cháy | ⭐⭐⭐ |
| 7 | **Physics (Pin)** | Break/Smash | Rút ghim → Vỡ nát | ⭐⭐⭐⭐⭐ |
| 8 | **Physics (Pin)** | Melt | Rút ghim → Tan chảy | ⭐⭐⭐ |
| 9 | **Sliding** | Crush | Trượt → Ép nát khi va chạm | ⭐⭐⭐⭐ |
| 10 | **Sliding** | Explode | Trượt → Nổ khi kết hợp | ⭐⭐⭐ |
| 11 | **Screw/Bolt** | Disassemble | Tháo ốc → Vỡ ra từng mảnh | ⭐⭐⭐⭐⭐ |
| 12 | **Screw/Bolt** | Shred | Tháo ốc → Băm nhỏ | ⭐⭐⭐ |
| 13 | **Merge** | Absorb | Gộp → Hút vào nhau | ⭐⭐⭐⭐ |
| 14 | **Merge** | Explode | Gộp → Nổ lớn | ⭐⭐⭐⭐ |
| 15 | **Hidden Object** | Break | Tìm → Phá vỡ để lộ | ⭐⭐⭐ |
| 16 | **Logic** | Burn | Giải đúng → Đốt sai | ⭐⭐⭐ |

#### 🎬 Destruction Timing (Khi nào destruction xảy ra?):

| Timing | Mô tả | Feel | Ví dụ |
|--------|-------|------|-------|
| **On Success** | Khi hoàn thành puzzle | Celebration, reward | Match-3 blast |
| **On Action** | Trong mỗi action | Immediate satisfaction | Slice each object |
| **On Fail** | Khi thua | Punishment but satisfying | Crush character |
| **Continuous** | Liên tục | ASMR, relaxing | Sand Balls flowing |
| **Climax** | Cuối level/chunk | Big moment | Chain explosion |

#### 🎨 Destruction Scale (Quy mô phá hủy):

| Scale | Mô tả | Visual Impact | Use Case |
|-------|-------|---------------|----------|
| **Micro** | 1 small object | Subtle satisfaction | Each tap/move |
| **Small** | Few objects | Clear feedback | Combo moves |
| **Medium** | Chunk of level | Celebratory | Section complete |
| **Large** | Most of level | Climax moment | Level complete |
| **Massive** | Entire level | Epic, viral-worthy | Perfect clear |

#### 📋 Template thiết kế Puzzle + Destruction:

```markdown
## Puzzle + Destruction Concept

### Puzzle Layer
- **Puzzle Type**: [Sort/Match/Draw/Physics/Sliding/Screw/Merge/...]
- **Core Mechanic**: [Mô tả ngắn gọn]
- **Win Condition**: [Khi nào thắng]
- **Lose Condition**: [Khi nào thua]

### Destruction Layer
- **Destruction Type**: [Crush/Cut/Melt/Explode/Absorb/Break/Shred/Burn]
- **Destruction Timing**: [On Success/On Action/On Fail/Continuous/Climax]
- **Destruction Scale**: [Micro/Small/Medium/Large/Massive]
- **Visual Feedback**: [Particles, Screen shake, Slow-mo, ...]

### Integration
- **How they connect**: [Puzzle và Destruction liên kết như thế nào?]
- **Destruction purpose**: [Reward/Punishment/Progression/Visual hook]
- **Marketing potential**: [Destruction có thu hút trong quảng cáo không?]

### Example Flow
1. [Bước 1: Player action]
2. [Bước 2: Puzzle logic]
3. [Bước 3: Destruction trigger]
4. [Bước 4: Visual feedback]
5. [Bước 5: Next action/Level complete]
```

#### 🏆 Case Studies: Puzzle + Destruction thành công:

| Game | Puzzle | Destruction | Why It Works |
|------|--------|-------------|--------------|
| **Stack Ball** | Timing (canh thời điểm) | Smash platforms | Simple + Satisfying |
| **Hole.io** | Collection strategy | Absorb objects | Power fantasy |
| **Color Box Jam** | Sort colors | Crush boxes on complete | Reward for puzzle |
| **Screw Loop** | Unscrew sequence | Shred picture | Curiosity + Destruction |
| **Soap Cutting** | Slice path | Cut through soap | ASMR + Satisfaction |
| **Bucket Crusher** | Aim & destroy | Crush bricks | Destruction AS goal |
| **Hole in Home** | Match-3 | Absorb with hole | Proven core + Proven visual |

#### ✅ Checklist Puzzle + Destruction:

**Bắt buộc:**
- [ ] Có yếu tố Puzzle (Level-based, Lose condition, Revive)
- [ ] Có yếu tố Destruction (Cảm giác "đã mắt")
- [ ] Destruction thu hút trong quảng cáo (marketability)
- [ ] KHÔNG phải Endless game

**Nên có:**
- [ ] Puzzle và Destruction liên kết chặt chẽ (không tách rời)
- [ ] Destruction timing phù hợp với gameplay
- [ ] Destruction scale tăng theo level
- [ ] Visual feedback mạnh cho destruction (particles, shake, sounds)
- [ ] Destruction tạo cảm xúc (satisfaction, power, relief)

**Kiểm tra:**
- [ ] Nếu bỏ Destruction, game có còn fun không? (Nên là CÓ)
- [ ] Nếu bỏ Puzzle, game có còn sâu không? (Nên là KHÔNG)
- [ ] Destruction có làm người xem quảng cáo muốn tải không?

---

### Bước 1.3: Xác định Direction Strategy

#### 📌 2 Chiến lược làm mới (theo Voodoo):

| Chiến lược | Công thức | Độ khó | Rủi ro |
|------------|-----------|--------|--------|
| **Cách 1: Giữ Core cũ + Trải nghiệm mới** | Core proven + Visual/Destruction mới | Trung bình | Thấp |
| **Cách 2: Giữ Trải nghiệm cũ + Core mới** | Visual proven + Puzzle mechanics mới | Cao hơn | Trung bình |

#### 🎯 Chiến lược 1: Giữ Core cũ + Đắp Trải nghiệm mới

**Khi nào dùng:**
- Tìm được core puzzle đã proven (có game thành công)
- Muốn giảm rủi ro về gameplay
- Có ý tưởng visual/destruction độc đáo

**Ví dụ:**
```
Core: Sort Game (Water Sort)
      ↓
Trải nghiệm mới: Đồ chơi 3D vật lý + Nghiền nát
      ↓
Kết quả: Scudom (chỉ số tốt hơn game gốc)
```

#### 🎯 Chiến lược 2: Giữ Trải nghiệm cũ + Đắp Core mới

**Khi nào dùng:**
- Tìm được trải nghiệm visual có CPI cực thấp
- Muốn tăng chiều sâu gameplay
- Có khả năng thiết kế puzzle tốt

**Ví dụ:**
```
Trải nghiệm: Hố đen hút đồ (Hole.io) - CPI siêu thấp
      ↓
Core mới: Match-3 mechanics
      ↓
Kết quả: Hole in Home (siêu phẩm hybrid-casual)
```

#### ✅ Checklist Bước 1.3:

- [ ] Chọn 1 trong 2 chiến lược chính
- [ ] Xác định game "gốc" để lấy Core hoặc Trải nghiệm
- [ ] Liệt kê 3-5 hướng có thể làm mới
- [ ] Đánh giá độ khả thi của mỗi hướng

---

## 🔷 PHASE 2: CONCEPT (Ý tưởng)

### Mục tiêu
Xây dựng concept chi tiết với đầy đủ 3 yếu tố: Unique + Challenging + Engaging

---

### Bước 2.1: Thiết kế tính Độc đáo (Uniqueness)

#### 📌 Công thức Uniqueness:

```
┌─────────────────────────────────────────────────────────────┐
│                    UNIQUENESS FORMULA                        │
├─────────────────────────────────────────────────────────────┤
│                                                              │
│  UNIQUENESS = CORE PUZZLE + EXPERIENCE (TWIST)              │
│                                                              │
│  Core Puzzle:          Experience (Twist):                  │
│  ├── Luật chơi rõ      ├── Visual "đã mắt"                  │
│  ├── Win/Lose rõ       ├── Destruction thỏa mãn             │
│  └── Thao tác đơn      └── Cảm xúc đặc biệt                 │
│                                                              │
└─────────────────────────────────────────────────────────────┘
```

#### 🎮 Các cách tạo Twist:

| Cách | Mô tả | Ví dụ |
|------|-------|-------|
| **Visual Twist** | Làm mới visual style | 2D → 3D, Flat → Physics-based |
| **Destruction Twist** | Thêm yếu tố phá hủy thỏa mãn | Nghiền nát, Cắt xẻ, Nổ tung |
| **Perspective Twist** | Thay đổi góc nhìn | Top-down → First person |
| **Scale Twist** | Thay đổi quy mô | Nhỏ → To, Ít → Nhiều (swarm physics) |
| **Emotion Twist** | Thêm cảm xúc cho objects | Face trên objects (Happy Glass) |
| **Physics Twist** | Thêm physics system | Ragdoll, Gravity, Bounce |

#### 📋 Template mô tả Concept:

```markdown
## Concept: [Tên Game]

### Core Puzzle
- **Input**: [Tap/Swipe/Drag/Hold]
- **Goal**: [Mục tiêu chính]
- **Win Condition**: [Khi nào thắng]
- **Lose Condition**: [Khi nào thua]

### Experience (Twist)
- **Visual Style**: [Mô tả]
- **Destruction Element**: [Yếu tố phá hủy]
- **Emotional Hook**: [Cảm xúc đánh vào]

### USP (Unique Selling Point)
> [1 câu mô tả điểm độc đáo nhất]

### Reference Games
- Core từ: [Game A]
- Trải nghiệm từ: [Game B]
```

#### ✅ Checklist Bước 2.1:

- [ ] Mô tả Core Puzzle rõ ràng (Input, Goal, Win, Lose)
- [ ] Xác định Experience Twist (Visual, Destruction, Emotion)
- [ ] Viết USP trong 1 câu
- [ ] Liệt kê 2 game references (1 Core + 1 Experience)
- [ ] Kiểm tra: Có trùng với game đã có trên market không?

---

### Bước 2.2: Thiết kế tính Thử thách (Challenge)

#### 📌 3 Yếu tố của Challenge công bằng:

| Yếu tố | Mô tả | Checklist |
|--------|-------|-----------|
| **Mục tiêu rõ ràng** | Biết cần làm gì để thắng, tránh gì để không thua | [ ] |
| **Dễ lập chiến lược** | Nhìn màn hình → biết các bước tiếp theo | [ ] |
| **Tự do** | Có nhiều hơn 1 cách để thắng | [ ] |

#### 🎯 Nguyên tắc tạo độ khó:

```
┌─────────────────────────────────────────────────────────────┐
│                  CHALLENGE DESIGN PRINCIPLES                 │
├─────────────────────────────────────────────────────────────┤
│                                                              │
│  ❌ TRÁNH:                                                   │
│  ├── Ẩn quá nhiều thông tin (thua do may rủi)              │
│  ├── Chỉ có 1 lời giải duy nhất (giống bài tập)            │
│  ├── Game gian lận (thua không hiểu lý do)                 │
│  └── Độ khó ngẫu nhiên không predictable                    │
│                                                              │
│  ✅ NÊN:                                                     │
│  ├── Tạo cảm giác "suýt thắng" (Near Win)                   │
│  ├── Mỗi thất bại = bài học để lần sau tốt hơn             │
│  ├── Progress rõ ràng (biết mình đang tiến bộ)             │
│  └── Revive/Continue đúng lúc "suýt thua"                  │
│                                                              │
└─────────────────────────────────────────────────────────────┘
```

#### 💰 Kích thích IAP thông qua độ khó:

| Cơ chế | Cách implement | Mục đích |
|--------|----------------|----------|
| **Time pressure** | Hết thời gian → Revive bằng coin | Tạo urgency |
| **Move limit** | Hết lượt → Mua thêm lượt | Tạo scarcity |
| **Near-miss** | Thua khi gần thắng → Continue | Tạo FOMO |
| **Difficulty spike** | Level khó → Booster/IAP | Tạo value |

#### 📊 APS (Attempts Per Success) - Chỉ số quan trọng:

| APS Range | Độ khó | Action |
|-----------|--------|--------|
| < 1.2 | Quá dễ | Tăng độ khó |
| 1.2 - 1.5 | Lý tưởng | Giữ nguyên |
| 1.5 - 2.0 | Khá khó | Monitor kỹ |
| > 2.0 | Quá khó | Giảm độ khó |

> **Lưu ý từ Voodoo**: APS là chỉ số quan trọng để validate khả năng kiếm tiền từ độ khó. Nếu tăng độ khó mà user vẫn chơi → cơ hội IAP lớn.

#### ✅ Checklist Bước 2.2:

- [ ] Định nghĩa Win Condition rõ ràng
- [ ] Định nghĩa Lose Condition rõ ràng
- [ ] Đảm bảo có nhiều cách để thắng (không phải 1 đường duy nhất)
- [ ] Thiết kế cảm giác "suýt thắng" (Near Win)
- [ ] Lên kế hoạch cho Revive/Continue mechanic
- [ ] Thiết kế độ khó tăng dần (Easy → Medium → Hard)

---

### Bước 2.3: Thiết kế tính Cuốn hút (Engaging / Game Feel)

#### 📌 3 Yếu tố của Game Feel (như bài hát hay):

| Yếu tố | Mô tả | Ví dụ |
|--------|-------|-------|
| **Không có nốt sai** | Tự động chặn water đi sai quy luật | Water Sort không cho đổ màu đỏ lên vàng |
| **Tiến triển liên tục** | Mỗi bước đi = tiến gần đích | Clear 1 row → thấy progress |
| **Khoảnh khắc cao trào** | Gỡ được nút thắt → vỡ òa | Combo chain reaction |

#### 🎨 Checklist Game Feel chi tiết:

| Category | Element | Must Have | Nice to Have |
|----------|---------|-----------|--------------|
| **Visual** | Particle effects | [ ] | |
| | Screen shake | [ ] | |
| | Color transitions | | [ ] |
| | Speed lines | | [ ] |
| | Glow/Bloom | | [ ] |
| **Audio** | Tap sound | [ ] | |
| | Success sound | [ ] | |
| | Fail sound | | [ ] |
| | Background music | | [ ] |
| | ASMR elements | | [ ] |
| **Haptic** | Vibration on action | | [ ] |
| | Vibration intensity vary | | [ ] |
| **Animation** | Smooth transitions | [ ] | |
| | Bounce/ease effects | [ ] | |
| | Idle animations | | [ ] |
| **Physics** | Weight feel | [ ] | |
| | Collision response | [ ] | |
| | Gravity/bounce | | [ ] |

#### 🎯 Nguyên tắc "No Wrong Notes":

```
┌─────────────────────────────────────────────────────────────┐
│                   "NO WRONG NOTES" PRINCIPLE                 │
├─────────────────────────────────────────────────────────────┤
│                                                              │
│  Mục tiêu: Mọi thao tác đều mang lại cảm giác tích cực      │
│                                                              │
│  Cách thực hiện:                                             │
│  1. Tự động chặn các nước đi sai quy luật                   │
│     → Không cho user thực hiện nước đi không hợp lệ        │
│     → Thay vì punish, hãy prevent                           │
│                                                              │
│  2. Mỗi action = feedback tức thì                           │
│     → Visual: Particle, flash, animation                    │
│     → Audio: Sound effect                                   │
│     → Haptic: Vibration                                     │
│                                                              │
│  3. Luôn có cảm giác tiến bộ                                │
│     → Show progress bar                                     │
│     → Celebration trên mỗi milestone                        │
│     → Không bao giờ làm user cảm giác "lùi"                 │
│                                                              │
└─────────────────────────────────────────────────────────────┘
```

#### ✅ Checklist Bước 2.3:

- [ ] Implement "No Wrong Notes" - chặn nước đi sai
- [ ] Thêm visual feedback cho mọi action
- [ ] Thêm audio feedback (tối thiểu tap + success)
- [ ] Thiết kế "Climax Moment" - khoảnh khắc cao trào
- [ ] Đảm bảo constant progression feel
- [ ] Test: Thao tác có "đã" không? (juice check)

---

### Bước 2.4: Thiết kế Creative/Marketing Hook

#### 📌 Công thức Creative 3 giây:

```
┌─────────────────────────────────────────────────────────────┐
│                    3-SECOND HOOK FORMULA                     │
├─────────────────────────────────────────────────────────────┤
│                                                              │
│  GIÂY 1: HOOK thị giác                                      │
│  ├── Màu sắc tương phản cao                                 │
│  ├── Action đang diễn ra                                    │
│  └── Bàn tay ảo đang tương tác                              │
│                                                              │
│  GIÂY 2: GIẢI THÍCH luật chơi                               │
│  ├── Show goal rõ ràng                                      │
│  ├── Show win/lose condition                                │
│  └── Không text, chỉ visual                                 │
│                                                              │
│  GIÂY 3: KÍCH THÍCH cảm xúc                                 │
│  ├── Near-miss / Fail scenario                              │
│  ├── "I can do better!" feeling                            │
│  └── Call to action (implicit)                              │
│                                                              │
└─────────────────────────────────────────────────────────────┘
```

#### 🎨 Visual Guidelines cho Creative:

| Element | Best Practice |
|---------|---------------|
| **Background** | Màu trung tính, xám, nhạt |
| **Main objects** | Màu rực rỡ, neon, tương phản cao |
| **Hand animation** | Luôn có để hướng dẫn thao tác |
| **Fail scenario** | Hiển thị thất bại ngớ ngẩn |
| **Text** | Tối thiểu hoặc không có |

#### 🎯 Chiến lược thao túng cảm xúc:

| Cảm xúc | Cách kích hoạt | Mục đích |
|---------|----------------|----------|
| **Tò mò** | Show kết quả bất ngờ | Muốn thử |
| **Ức chế** | Show fail ngớ ngẩn | "Tôi làm tốt hơn" |
| **Phấn khích** | Show near-win căng thẳng | Muốn trải nghiệm |
| **Đồng cảm** | Character với biểu cảm | Quan tâm kết quả |

#### ✅ Checklist Bước 2.4:

- [ ] Mô tả 3 giây đầu của video creative
- [ ] Xác định "Fail Scenario" để kích thích tải về
- [ ] Thiết kế color palette với độ tương phản cao
- [ ] Lên kịch bản bàn tay ảo hướng dẫn
- [ ] Test: Creative có hiểu trong 3 giây không?

---

## 🔷 PHASE 3: VALIDATION (Kiểm chứng)

### Mục tiêu
Kiểm chứng concept qua prototype và metrics

---

### Bước 3.1: Prototype V1 Specifications

#### 📌 Scope cho Prototype V1:

| Element | Required | Not Required |
|---------|----------|--------------|
| **Levels** | 30-40 levels (hand-crafted) | 100+ levels |
| **Core mechanic** | ✅ Hoàn chỉnh | - |
| **Win/Lose** | ✅ Hoàn chỉnh | - |
| **Basic UI** | ✅ | Complex UI |
| **Game Feel** | ✅ Polish | - |
| **Booster** | - | ❌ Chưa cần |
| **Meta progression** | - | ❌ Chưa cần |
| **IAP** | - | ❌ Chưa cần |
| **Ops/Live events** | - | ❌ Chưa cần |

#### 🎯 Nội dung 30-40 levels:

| Level Range | Mục đích | Độ khó |
|-------------|----------|--------|
| 1-5 | Tutorial ngầm, easy wins | Rất dễ |
| 6-15 | Introduce mechanics | Dễ |
| 16-25 | Combine mechanics | Trung bình |
| 26-40 | Challenge | Khó |

#### 💻 Technical Stack (khuyến nghị Voodoo):

| Category | Tool | Ghi chú |
|----------|------|---------|
| **Engine** | Unity 6 (LTS) | Bắt buộc |
| **Render Pipeline** | URP | Tiêu chuẩn |
| **Tweening** | DOTween | Essential cho juice |
| **Camera** | Cinemachine | Smooth transitions |
| **VFX** | VFX Graph / Shader Graph | Reactive elements |

#### ✅ Checklist Bước 3.1:

- [ ] Core mechanic hoạt động mượt mà
- [ ] Win/Lose condition hoàn chỉnh
- [ ] 30-40 levels hand-crafted
- [ ] Basic UI (Menu, Game, Win, Lose)
- [ ] Game Feel polish (particles, sounds, animations)
- [ ] Quick restart functionality
- [ ] Level progression system

---

### Bước 3.2: Metrics Targets cho V1

#### 📊 Targets cho Prototype V1:

| Metric | Minimum | Good | Great | Excellent |
|--------|---------|------|-------|-----------|
| **D1 Retention** | 25% | 30-35% | 40% | 45%+ |
| **D7 Retention** | 8% | 10% | 15% | 20%+ |
| **CPI** | <$3 | <$2 | <$1 | <$0.50 |
| **Playtime** | 10 min | 20-30 min | 30+ min | - |
| **APS** | 1.0 | 1.2-1.4 | 1.5 | - |

> **Lưu ý từ Voodoo**: Không cần đạt ngay con số excellent! V1 chỉ cần D1 ~30-35%, Playtime 20-30 phút, CPI ~$2, D7 ~10% là đã có tín hiệu tiềm năng để iterate.

#### 📈 Metrics để theo dõi:

| Metric | Cách đo | Mục đích |
|--------|---------|----------|
| **Level completion rate** | % người qua mỗi level | Detect difficulty spikes |
| **Drop-off point** | Level nào user bỏ nhiều nhất | Optimize funnel |
| **APS** | Attempts / Success | Validate difficulty/IAP potential |
| **Session length** | Thời gian chơi trung bình | Engagement |
| **Sessions per day** | Số lần mở app/ngày | Addiction level |

#### ✅ Checklist Bước 3.2:

- [ ] Tích hợp analytics (GameAnalytics, Firebase)
- [ ] Setup tracking cho các events quan trọng
- [ ] Chuẩn bị budget test ($100-200/ngày, 4-5 ngày)
- [ ] Tạo video creative cho CPI test
- [ ] Setup tracking dashboard

---

### Bước 3.3: Playtesting & Feedback

#### 📋 Playtest Questions:

| Category | Question |
|----------|----------|
| **Understandability** | Bạn hiểu phải làm gì không? |
| **Control** | Điều khiển có dễ dùng không? |
| **Difficulty** | Level có quá khó/dễ không? |
| **Engagement** | Bạn có muốn chơi tiếp không? |
| **Fun** | Điểm gì thú vị nhất? |
| **Frustration** | Có lúc nào thấy ức chế không? Tại sao? |

#### 🎯 Success Criteria cho Playtest:

| Metric | Target |
|--------|--------|
| Hiểu trong 5 giây đầu | 90%+ |
| Level 1 completion | 80%+ |
| Muốn chơi tiếp | 70%+ |
| No major frustration | 90%+ |

#### ✅ Checklist Bước 3.3:

- [ ] Internal playtest (team members)
- [ ] External playtest (5-10 người ngoài)
- [ ] Thu thập feedback theo questionnaire
- [ ] Ghi lại các điểm drop-off
- [ ] Phân tích và prioritize fixes

---

### Bước 3.4: Go/No-Go Decision

#### 📊 Decision Matrix:

| Scenario | D1 | D7 | CPI | Decision |
|----------|-----|-----|-----|----------|
| 🟢 Excellent | >40% | >15% | <$1 | **GO** - Scale ngay |
| 🟢 Good | 35-40% | 10-15% | $1-2 | **GO** - Iterate nhẹ |
| 🟡 Potential | 30-35% | 8-10% | $2-3 | **ITERATE** - Cần cải thiện |
| 🔴 Poor | <30% | <8% | >$3 | **NO-GO** - Pivot hoặc kill |

#### 🔄 Nếu cần Iterate:

| Vấn đề | Nguyên nhân có thể | Action |
|--------|-------------------|--------|
| CPI cao | Creative không hấp dẫn | Tối ưu creative, test hook mới |
| D1 thấp | Core không fun | Review game feel, add juice |
| D7 thấp | Không có chiều sâu | Add progression, meta |
| Drop-off sớm | Tutorial kém | Improve FTUE |
| Drop-off muộn | Quá khó | Balance difficulty |

#### ✅ Checklist Bước 3.4:

- [ ] Thu thập đủ metrics sau 4-5 ngày test
- [ ] Phân tích theo decision matrix
- [ ] Nếu GO: Lên kế hoạch scale
- [ ] Nếu ITERATE: Xác định vấn đề và solution
- [ ] Nếu NO-GO: Pivot sang concept mới hoặc kill project

---

## 🔷 PHASE 4: PRODUCTION (Sản xuất)

### Mục tiêu
Mở rộng prototype thành product hoàn chỉnh sẵn sàng soft launch

---

### Bước 4.1: Soft Launch Requirements

#### 📌 Scope cho Soft Launch:

| Element | Requirement |
|---------|-------------|
| **Content** | Đủ chơi 14 ngày (đo D14, D30) |
| **Levels** | 100+ levels |
| **Booster** | 2-3 boosters cơ bản |
| **Blocker/Obstacle** | 4-5 loại |
| **Economy** | Virtual currency, reward system |
| **IAP** | 3-5 packages cơ bản |
| **Ads** | Interstitial + Rewarded |
| **Meta** | Basic progression |

#### 📊 Soft Launch Targets:

| Metric | Target |
|--------|--------|
| **CPI** | <$2 |
| **D7 Retention** | >20% |
| **D14 Retention** | >15% |
| **Playtime** | >30 phút |
| **APS** | >1.4 |

#### ✅ Checklist Bước 4.1:

- [ ] 100+ levels hand-crafted
- [ ] 2-3 Boosters implemented
- [ ] 4-5 Blocker types
- [ ] Virtual currency system
- [ ] 3-5 IAP packages
- [ ] Interstitial + Rewarded ads
- [ ] Basic meta progression
- [ ] Analytics đầy đủ

---

### Bước 4.2: Scale Preparation

#### 📌 Checklist trước khi Scale:

| Category | Item | Status |
|----------|------|--------|
| **Technical** | Crash rate <1% | [ ] |
| | Load time <3s | [ ] |
| | No memory leaks | [ ] |
| **Content** | 200+ levels | [ ] |
| | Content pipeline ready | [ ] |
| **Monetization** | IAP tested | [ ] |
| | Ads placement optimized | [ ] |
| **Marketing** | Multiple creatives ready | [ ] |
| | ASO complete | [ ] |
| **Legal** | Privacy policy | [ ] |
| | GDPR/CCPA compliant | [ ] |

---

## 📋 MASTER CHECKLIST: IDEA TO PRODUCTION

### Phase 1: Discovery ✅

- [ ] **1.1** Nghiên cứu 5-10 game hyper-casual cũ có CPI thấp
- [ ] **1.1** Nghiên cứu 5-10 game hybrid-casual đang hot
- [ ] **1.2** Phân tích 10 game references theo framework (Input, Goal, Win, Lose, Feedback, Hook)
- [ ] **1.2** Xác định mechanics có marketability cao
- [ ] **1.2.1** 🔥 **Chọn Puzzle Type** (Sort/Match/Draw/Physics/Logic/Word/Sliding/Hidden Object/Screw)
- [ ] **1.2.1** 🔥 **Chọn Destruction Type** (Crush/Cut/Melt/Explode/Absorb/Break/Shred/Burn)
- [ ] **1.2.1** 🔥 **Xác định Combination Pattern** (Puzzle × Destruction)
- [ ] **1.2.1** 🔥 **Xác định Destruction Timing** (On Success/On Action/On Fail/Continuous/Climax)
- [ ] **1.2.1** 🔥 **Xác định Destruction Scale** (Micro/Small/Medium/Large/Massive)
- [ ] **1.2.1** Điền Template Puzzle + Destruction Concept
- [ ] **1.3** Chọn chiến lược: Core cũ + Experience mới HOẶC Experience cũ + Core mới
- [ ] **1.3** Xác định game "gốc" để phát triển

### Phase 2: Concept ✅

- [ ] **2.1** Mô tả Core Puzzle (Input, Goal, Win, Lose)
- [ ] **2.1** Xác định Experience Twist (Visual, Destruction, Emotion)
- [ ] **2.1** Viết USP trong 1 câu
- [ ] **2.1** Kiểm tra không trùng game trên market
- [ ] **2.2** Định nghĩa Win/Lose condition rõ ràng
- [ ] **2.2** Đảm bảo nhiều cách để thắng
- [ ] **2.2** Thiết kế Near-Win feeling
- [ ] **2.2** Lên kế hoạch Revive/Continue
- [ ] **2.3** Implement "No Wrong Notes"
- [ ] **2.3** Thêm visual/audio feedback
- [ ] **2.3** Thiết kế Climax Moment
- [ ] **2.4** Mô tả 3 giây đầu creative
- [ ] **2.4** Thiết kế Fail Scenario
- [ ] **2.4** Xác định color palette

### Phase 3: Validation ✅

- [ ] **3.1** Core mechanic hoạt động
- [ ] **3.1** 30-40 levels hand-crafted
- [ ] **3.1** Basic UI hoàn chỉnh
- [ ] **3.1** Game Feel polish
- [ ] **3.2** Analytics tích hợp
- [ ] **3.2** Creative cho CPI test
- [ ] **3.3** Internal playtest
- [ ] **3.3** External playtest
- [ ] **3.4** Thu thập metrics
- [ ] **3.4** Go/No-Go decision

### Phase 4: Production ✅

- [ ] **4.1** 100+ levels
- [ ] **4.1** Boosters implemented
- [ ] **4.1** Economy system
- [ ] **4.1** IAP packages
- [ ] **4.1** Ads integration
- [ ] **4.2** Technical stability
- [ ] **4.2** Marketing materials
- [ ] **4.2** Legal compliance

---

## 🎯 TÓM TẮT: KEY SUCCESS FACTORS

### Từ Voodoo:

| Factor | Mô tả |
|--------|-------|
| **Uniqueness** | Core + Experience twist |
| **Challenge** | Fair, Near-Win, Progression |
| **Engaging** | No Wrong Notes, Constant Progress, Climax |
| **Marketability** | 3-second hook, Fail scenario, High contrast |
| **Game Feel** | Juice trên mọi action |

### Công thức thành công:

```
┌─────────────────────────────────────────────────────────────┐
│                    SUCCESS FORMULA                           │
├─────────────────────────────────────────────────────────────┤
│                                                              │
│  HIT GAME = UNIQUE + CHALLENGING + ENGAGING                 │
│                                                              │
│  UNIQUE = Core proven + Twist mới                           │
│  CHALLENGING = Fair + Near-Win + Progression                │
│  ENGAGING = No Wrong Notes + Juice + Climax                 │
│                                                              │
│  MARKETABILITY = 3s Hook + Fail Scenario + High Contrast    │
│                                                              │
│  METRICS TARGETS (V1):                                       │
│  ├── D1: 30-35%+                                            │
│  ├── D7: 10%+                                               │
│  ├── CPI: <$2                                               │
│  ├── Playtime: 20-30 min+                                   │
│  └── APS: 1.2-1.4                                           │
│                                                              │
└─────────────────────────────────────────────────────────────┘
```

---

## 📚 RESOURCES

### Wiki Links
- [Voodoo Game Design Guidelines](Voodoo-Game-Design-Guidelines)
- [Voodoo Success Stories](Voodoo-Success)
- [Game Templates](Templates)
- [Mechanics Library](Mechanics-Library)
- [Puzzle Prototyping](Puzzle-Prototyping)
- [Case Studies](Case-Studies)

### External Links
- [Voodoo Academy](https://voodoo.io/academy)
- [Voodoo Publishing](https://voodoo.io/publishing)
- [Supersonic Case Studies](https://supersonic.com/learn/case-studies/)

---

*Last Updated: Tháng 3/2026*
*Maintained by Kien Tao So Community*