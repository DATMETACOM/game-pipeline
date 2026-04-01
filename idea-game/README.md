# 🎮 Idea Game Library

> Repository của các game ideas được phát triển và validate theo framework Voodoo
> Mỗi phiên làm việc = 1 game idea riêng biệt

---

## 📁 Cấu Trúc Folder

```
idea-game/
├── README.md                    (File này - Tổng quan)
├── maze-match/                  (Game idea #1)
│   ├── README.md               (Overview của game này)
│   ├── ANALYSIS-SUMMARY.md     (Dashboard tổng hợp)
│   ├── IDEA-MAZE-MATCH-FINAL.md (Complete idea document)
│   ├── AI-PROMPT-3-LEVELS.md   (Prompt cho AI)
│   └── IDEA-ANALYSIS-Maze-Match.md (Initial analysis)
│
├── [game-name-2]/              (Game idea #2 - Phiên làm việc sau)
│   └── ...
│
└── [game-name-3]/              (Game idea #3 - Phiên làm việc sau)
    └── ...
```

---

## 🎯 Mục Tiêu

Mỗi folder game chứa:
1. **Initial Analysis** - Phân tích ý tưởng ban đầu
2. **Final Idea Document** - Specification hoàn chỉnh (VR01-VR06 pass)
3. **Analysis Summary** - Dashboard với metrics, APS, validation
4. **AI Prompt** - Prompt chi tiết để generate levels/prototypes
5. **README** - Overview nhanh của game đó

---

## 📋 Game Ideas

### 1. Maze Match Hero ⭐ **[READY FOR PROTOTYPE]**
**Status:** ✅ Approved for Prototype V1
**Concept:** Match-3 + Pathfinding puzzle
**APS:** 1.45 (target > 1.4) ✅
**CPI:** ~$1.80-2.20
**Created:** 2026-03-31

**Folder:** `maze-match/`

**Quick Start:**
1. Read `maze-match/ANALYSIS-SUMMARY.md` for overview
2. Use `maze-match/AI-PROMPT-3-LEVELS.md` to generate levels
3. Reference `maze-match/IDEA-MAZE-MATCH-FINAL.md` for full spec

### 2. DogFlow ⭐ **[READY FOR PROTOTYPE]**
**Status:** ✅ Ready for Prototype V1
**Concept:** Sheepdog placement + flock redirection
**APS:** 1.48 (target > 1.4) ✅
**CPI:** ~$1.70-2.00
**Created:** 2026-04-01

**Folder:** `DogFlow/`

**Quick Start:**
1. Read `DogFlow/ANALYSIS-SUMMARY.md` for overview
2. Use `DogFlow/AI-PROMPT-3-LEVELS.md` to generate detailed levels
3. Reference `DogFlow/IDEA-DOGFLOW-FINAL.md` for full spec

---

## 🔄 Workflow Cho Mỗi Phiên Làm Việc

```
1. User đưa ra ý tưởng game
   ↓
2. Phân tích theo framework Voodoo
   ↓
3. Tạo folder mới: idea-game/[game-name]/
   ↓
4. Tạo documents:
   - Initial analysis (chỉ ra vấn đề)
   - Final idea document (VR01-VR06 pass)
   - Analysis summary (dashboard, APS, metrics)
   - AI prompt (để generate levels)
   - README (overview)
   ↓
5. Validate APS > 1.4 ✅
   ↓
6. Approved for Prototype V1 🚀
```

---

## 📊 Framework Sử Dụng

**Voodoo Framework (March 2026):**

| Component | File |
|-----------|------|
| Core Mechanics | `../framework-v2/00A-AI-Generation-Pack.md` |
| Idea Review Criteria | `../framework-v2/01-Idea-Review-Pack.md` |
| APS Validation | `../framework-v2/01A-APS-Metrics-Validation-Guide.md` |
| Voodoo Requirements | `../framework-v2/00-Voodoo-Livestream-Key-Points.md` |

---

## ✅ Validation Criteria

Mỗi game idea phải pass **VR01-VR06:**

| VR | Criteria | Weight |
|----|----------|--------|
| **VR01** | Clear Puzzle Core | ⭐⭐⭐ |
| **VR02** | Newness & Twist | ⭐⭐⭐ |
| **VR03** | Fair Challenge (APS > 1.4) | ⭐⭐⭐ |
| **VR04** | Strong Game Feel | ⭐⭐⭐ |
| **VR05** | Fast Prototype Scope | ⭐⭐⭐ |
| **VR06** | Publishability | ⭐⭐⭐ |

**Pass threshold:** 90%+ overall → Approved for Prototype

---

## 🚀 Next Steps

**Khi bắt đầu game idea mới:**
1. Tạo folder mới trong `idea-game/`
2. Follow workflow ở trên
3. Tạo 5 documents như Maze Match example
4. Validate VR01-VR06
5. Calculate APS (must be > 1.4)
6. Approve for prototype hoặc revise

---

## 📈 Metrics Dashboard

### All Game Ideas

| Game | Status | APS | CPI | VR Score | Prototype Ready |
|------|--------|-----|-----|----------|-----------------|
| Maze Match Hero | ✅ Complete | 1.45 | ~$2.00 | 96.7% | ✅ Yes |
| DogFlow | ✅ Complete | 1.48 | ~$1.70-2.00 | 88.0% | ✅ Yes |

---

## 🎓 Learning Repository

Mỗi folder game là một case study về:
- Idea refinement process
- APS calculation & balancing
- Fair challenge design
- Game feel specification
- Prototype scoping
- Publishability analysis

**Học từ quá trình, không chỉ kết quả.**

---

*Idea Game Library created: 2026-03-31*
*Framework: Voodoo March 2026*
*Purpose: Organize game ideas by session*
