## ⚽ Split-Screen Soccer Game

**`Blueprints`** • **`UE5 Chaos Physics`** • **`Local Multiplayer`**


**🔑 What Makes This Special:**

### 🎮 **Proper Split-Screen Implementation**
Split-screen in UE5 is **notoriously tricky** - and most tutorials don't cover the quirks. This project implements:
- ✅ **Independent Player Inputs** - Each controller has isolated input handling
- ✅ **Shared Game State** - Ball, score, and goals synchronized across viewports
- ✅ **Viewport Management** - Camera splitting, UI positioning, and render target handling
- ✅ **Edge Case Handling** - Goal celebrations, respawns, and pause menus in split-screen context

**Why This Matters:** Most UE5 developers struggle with split-screen because it requires deep understanding of player controllers, game state replication (even locally), and viewport systems.

---

### ⚽ **Smart Ball Ownership System**
Traditional sports games use simple "touch = own" logic. This system is **proximity-based and physics-aware**:

**The Algorithm:**
```cpp
