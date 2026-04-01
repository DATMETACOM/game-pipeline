# IDEA ANALYSIS: Maze Match Hero

## 📊 PHÂN TÍCH THEO FRAMEWORK (VR01-VR06)

---

## VR01. Clear Puzzle Core

### ❌ VẤN ĐỀ HIỆN TẠI

**Ý tưởng có 3 mechanics chồng lên nhau:**

| Layer | Mechanic | Complexity |
|-------|----------|------------|
| Base | Match-3 core | Medium |
| Layer 2 | Pathfinding/maze | Medium |
| Layer 3 | Hero combat + progression | High |

**Vấn đề:**
- Core không thể giải thích bằng 1 câu
- Người mới không hiểu điều kiện thắng/thua trong vài giây
- Quá nhiều hệ thống cho prototype V1

---

## VR02. Newness

### ✅ ĐIỂM MẠNH

**Twist rõ ràng:**
```
"Match-3 tạo đường đi cho hero vượt qua mê cung"
```

**Phân tích:**
- Nếu bỏ twist đi → còn lại Match-3 thuần túy (Royal Match)
- Twist nằm ở: **Experience mới (hero journey) trên Core cũ (Match-3)**

**Voodoo approval:** Đây là direction an toàn (proven core + fresh experience)

---

## VR03. Fair Challenge & APS

### ⚠️ VẤN ĐỀ QUAN TRỌNG

**APS Risk Level: HIGH**

| Factor | Effect on APS | Explanation |
|--------|--------------|--------------|
| Dual maze (Level 3) | ↑↑↑ Very High | 2x complexity = APS 2.0+ |
| Combat system | ↑↑ High | Hidden info trong match color → power mapping |
| Limited moves | ↑ High | Không rõ bao nhiêu moves là "fair" |
| Pathfinding dependency | ↑↑ High | Sai 1 match → sai toàn bộ path |

**Dự đoán APS:**
- Level 1-10: 1.3-1.5 ✓ (có thể pass)
- Level 11-30: 1.7-2.0 ⚠️ (ngưỡng nguy hiểm)
- Level 31-50: 2.2-2.8 ❌ (quá cao, user sẽ quit)

**Voodoo Critical Requirement Violated:**
```
APS > 1.4 cho 50 level đầu ❌
→ Idea hiện tại KHÔNG PASS
```

---

## VR04. Game Feel

### ✅ POTENTIAL (cần design kỹ)

**Pixar-style aesthetic:**
- Royal Match đã proven visual appeal
- Animation có thể tạo payoff mạnh

**Nhưng cần clarify:**
- Payoff moment là gì? Match successful? Hero到达? Monster defeated?
- "No wrong notes": Match-3 có thể reject invalid moves ✓
- Continuous progress: Hero movement dọc theo path có thể tạo cảm giác tiến bộ ✓

---

## VR05. Fast Prototype Scope

### ❌ VẤN ĐỀ NẶNG NỀ

**Voodoo Prototype V1 Requirements:**
```
✓ 30-40 levels handcrafted
✓ 3-4 obstacle types
✗ KHÔNG cần: meta, booster, economy, shop, IAP
```

**Idea hiện tại có:**
- [ ] Hero stats progression → **META**
- [ ] Combat system → **QUÁ PHỨC TẠP**
- [ ] Treasure collection → **ECONOMY**
- [ ] Power mapping (match color → skill) → **HIDDEN INFO**

**Scope creep:** Đây là 1 game hoàn chỉnh, không phải prototype gọn

---

## VR06. Publishability

### ✅ ĐIỂM MẠNH

**CPI Thesis:**
- Pixar-like aesthetic → proven low CPI (Royal Match, Royal Kingdom)
- Hero journey → emotional hook
- Visual readable trong 3 giây → hero moving through maze

**BUT:**
- Complex mechanics có thể làm tăng CPI
- Ad creative khó giải thích hết mechanics trong 3 giây

---

## 🚨 TỔNG HỢP VẤN ĐỀ

| VR | Status | Issue | Severity |
|----|--------|-------|----------|
| VR01 | ❌ FAIL | Core không rõ, quá nhiều layers | CRITICAL |
| VR02 | ✅ PASS | Twist rõ ràng, direction an toàn | - |
| VR03 | ❌ FAIL | APS dự đoán > 2.0 | CRITICAL |
| VR04 | ⚠️ UNCLEAR | Cần design kỹ payoff | MEDIUM |
| VR05 | ❌ FAIL | Quá rộng, có meta layer | CRITICAL |
| VR06 | ⚠️ RISKY | Visual tốt nhưng mechanics phức tạp | MEDIUM |

**QUYẾT ĐỊNH: NEEDS MAJOR REVISION**

---

## 💡 ĐỀ XUẤT REVISION

### OPTION A: Simplify (RECOMMENDED)

**Focus vào CORE khác biệt nhất:**

```
Match-3 + Pathfinding (ONLY)
Drop: Combat, Progression, Stats, Treasure
```

**Revised Concept:**
- **Core:** Match-3 để tạo path cho hero
- **Goal:** Hero到达 exit trong limited moves
- **Win:** Hero reaches exit
- **Lose:** Hết moves hoặc hero blocked
- **Obstacles:**
  1. Locked tiles (cần specific color match để unlock)
  2. One-way paths (match theo direction)
  3. Moving obstacles (timing element)
  4. Split paths (quyết định strategic)

**APS Target:**
- Level 1-10: 1.1-1.2 (single obvious path)
- Level 11-30: 1.3-1.5 (2-3 path options)
- Level 31-50: 1.5-1.8 (multiple solutions, tight moves)

**Prototype Scope:**
- 30-40 levels
- 4 obstacles (liệt kê trên)
- NO combat, NO progression, NO economy

---

### OPTION B: Hybrid Approach

**Giữ combat nhưng làm META (post-prototype):**

**Prototype V1:**
```
Focus: Match-3 + Pathfinding ONLY
X Hero stats
X Monster combat
X Treasure collection
→ Để sau khi prototype pass
```

**Soft Launch (nếu prototype pass):**
```
Thêm: Combat layer vào existing pathfinding core
```

---

## ❓ CÂU HỎI CHO USER

1. **Bạn muốn focus vào experience nào?**
   - A. Strategic puzzle (pathfinding challenge)
   - B. Combat progression (hero growth)
   - C. Hybrid (cả hai)

2. **Combat có phải là điểm khác biệt chính không?**
   - Nếu CÓ → Cân nhắc làm combat core (không phải Match-3)
   - Nếu KHÔNG → Drop combat, focus vào pathfinding

3. **Bạn muốn tôi revision theo hướng nào?**
   - A. Simplify (Match-3 + Pathfinding only)
   - B. Keep combat but separate into core + meta
   - C. Explore different core mechanics

---

## 📋 NEXT STEPS

Sau khi user trả lời:
1. Refine concept theo lựa chọn
2. Thiết kế APS curve chi tiết (50 levels)
3. Design 3 obstacles đầu tiên
4. Write prompt chi tiết cho AI (Easy/Medium/Hard levels)
5. Final checklist VR01-VR06 pass

---

*Analysis created: 2026-03-31*
*Framework version: Voodoo March 2026*
