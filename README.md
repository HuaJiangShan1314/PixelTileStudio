# 🎨 像素瓦片工坊 (Pixel Tile Studio)

> **一款免费、轻量的像素双网格瓦片地图绘制工具**
> *A free, lightweight pixel dual-grid tile map painting tool.*
>
> **版本 (Version)：v1.0.0 公开测试版 (Public Beta)**

---

## 📖 快速介绍 (Introduction)

**中文**：像素瓦片工坊是一款专为"像素双网格瓦片系统"设计的绘制与组合工具。支持 6 个独立画布、16 色 / Hex / RGB 调色、4×4 拼图实时预览、光照修改层以及切片测试场景。

**English**: Pixel Tile Studio is a painting and composition tool designed specifically for the "Pixel Dual-Grid Tile System". It supports 6 independent canvases, 16-color / Hex / RGB input, real-time 4×4 tile preview, a lighting modification layer, and a test scene.

## 📥 下载与安装 (Download & Installation)

* **国内蓝奏云 (极速推荐) / Lanzou Cloud (Recommended for China)**: [点击这里去蓝奏云下载（提取码：1vr9）](https://wwamt.lanzout.com/b00rp90vyd)
* **GitHub**: [点击这里去 Releases 页面下载](https://github.com/HuaJiangShan1314/PixelTileStudio/releases) *(Download from the Releases page)*

**安装方法 / Installation**:
1. 解压到**全英文路径**下 / *Extract to an English-only path.*
2. 双击 `PixelTileStudio.exe` 运行（免安装） / *Double-click to run (portable).*

## ❤️ 支持作者 (Support)

如果这个工具帮到了你，欢迎请我喝可乐。
*If this tool helps you, feel free to buy me a coke.*
👉 **[点击这里支持我（爱发电）](https://afdian.com/a/hjs0307)**

---

<details>
<summary>👇 <b>点击展开详细中文文档 (Click to expand Chinese documentation)</b></summary>

<br>

## 📖 这是什么

像素瓦片工坊是一款专为**像素双网格瓦片系统**设计的绘制与组合工具。

**双网格瓦片系统**是一种常见的像素地图绘制方式：
- 地图由格子组成，每个格子有两种状态（用"甲"和"乙"表示）。
- 每 2×2 个格子组合成一个"视觉瓦片"，显示一个具体的图像。
- 2×2 格子的状态决定显示哪个瓦片（共 16 种可能）。

**典型用途：**
- 🗺️ **像素游戏的地图绘制**：用二态网格快速设计地形、墙壁、道路。
- 🧱 **瓦片素材测试**：验证 16 种瓦片组合在实际地图中的效果。
- 🎨 **像素素材原型**：快速验证素材搭配和旋转效果。
- 🧩 **拼图设计**：探索同一组素材的不同排布方式。

## 🎯 用在哪里

### 场景 1：设计双网格瓦片地图
你画好 6 个基础瓦片（比如草地、道路、墙角等），工具帮你：
- 用这 6 个瓦片按 4×4 组合出大图。
- 实时预览不同旋转角度下的效果。
- 一键导出为 PNG，用于游戏引擎。

### 场景 2：测试二态地图布局
用测试场景的**二态网格**模拟地图：
- 格子只有"甲/乙"两种状态。
- 每 2×2 组合自动选择对应的瓦片。
- 直观看到地图在不同布局下的样子。

### 场景 3：像素素材的快速原型
不用打开 PS，直接在工具里：
- 画 6 个瓦片。
- 调整旋转、组合。
- 导出验证。

## ✨ 核心功能

### 🧩 一、6 个源 + 4×4 拼图
**左边画 6 个源，右边拼成 4×4 大图。**

| 功能 | 说明 |
|---|---|
| **6 个独立源** | 每个源可单独绘制，互不影响 |
| **4×4 拼图** | 右侧实时显示，改一笔立刻变 |
| **独立旋转** | 每个拼图块可旋转 0 / 90 / 180 / 270° |
| **旋转源** | 一键把当前源在拼图中顺时针转 90° |

### 🖌️ 二、光照修改层
**在 4×4 拼图上叠加一层独立画布，用于绘制阴影、高光、色调等整体效果。**

| 功能 | 说明 |
|---|---|
| **独立图层** | 不污染原始 6 个源，随时显隐 |
| **一键清空** | 清除修改层全部内容，可 Ctrl+Z 撤销 |
| **共享工具** | 画笔 / 橡皮 / 填充、笔刷大小、颜色、透明度与左侧共享 |
| **随存档保存** | 修改层内容随存档保留，导出时可选包含或不包含 |
| **跨场景传递** | 切到测试场景时一并带上，切片中显示光照效果 |

### 🎨 三、像素绘制
| 工具 | 说明 |
|---|---|
| **画笔** | 逐像素绘制，支持 1×1 ~ 8×8 |
| **橡皮** | 完全擦除像素 |
| **油漆桶** | 填充相邻同色或空白区域 |
| **透明度** | 0 ~ 255 可调，支持半透明 |
| **混合模式** | 可选，画笔颜色与已有像素混合 |
| **撤销 / 重做** | 最多 50 步 |

**画布尺寸**：8×8 / 16×16 / 32×32 / 64×64

### 🎨 四、颜色系统
- 16 色预设调色板
- Hex / RGB 精确输入
- 6 个快捷色槽（常用色一键切换）
- **实时取色**：鼠标悬停画布时预览像素颜色，点击拾取并同步到笔刷、Alpha、输入框、快捷色槽
- 点击颜色文本复制 Hex

### 🔍 五、绘制辅助
- **参考图层**：显示当前源"应该的样子"
- **透明棋盘格**：区分透明和白色（G 键）
- **拼图辅助线**：显示 4×4 分割和编号（H 键）
- **缩放 / 平移**：Alt + 滚轮 / 中键拖动
- **同步平移**：Shift + 中键拖动时两侧画布一起动

### 🧪 六、测试场景（双网格模拟）
**把拼图切 16 个切片，用二态网格组合。**

| 功能 | 说明 |
|---|---|
| **二态网格** | 甲（深色）/ 乙（浅色），可画 |
| **视觉层** | 每 2×2 格子自动显示对应切片 |
| **网格尺寸** | 8 / 16 / 32 / 64 / 128 五档 |
| **网格线开关** | 场景线（L）/ 视觉线（K）独立切换 |
| **切片来源** | 实时读取当前 4×4 拼图（含修改层） |
| **独立撤销** | Ctrl+Z / Ctrl+Y |

### 💾 七、存档与导出
| 功能 | 说明 |
|---|---|
| **保存 / 另存为 / 加载** | 多存档管理 |
| **导出拼图** | 4×4 拼图存为 PNG（可选包含修改层） |
| **导出源图** | 勾选要导出的源，批量导出 |
| **自动保存到桌面** | 真实桌面路径，不受 OneDrive 影响 |
| **状态持久化** | 画布尺寸、修改层显隐、测试网格尺寸跨会话保留 |

### 🔄 八、更新检查
启动时静默检测新版本。发现更新时在工具栏显示提示，不打扰使用。

## 📥 安装方法

1. 下载 `PixelTileStudio_v1.0.0.zip`
2. **解压到全英文路径下**（例如 `D:\PixelTileStudio`）
3. 双击 `PixelTileStudio.exe` 运行（免安装，绿色版）

**⚠️ 注意**：
- 不要解压到带中文的路径，可能导致程序异常。
- 不要直接双击 zip 内的 exe，必须解压后再运行。

## 🎮 快捷键

### 绘制场景
| 快捷键 | 功能 |
|---|---|
| 鼠标左键拖动 | 绘制像素（左侧画源 / 右侧画修改层） |
| Alt + 滚轮 | 缩放画布 |
| 中键拖动 | 平移视图 |
| Shift + 中键拖动 | 两侧画布同步平移 |
| 普通滚轮 | 调整画笔大小（鼠标在画布内时） |
| F | 复位视图（左右两侧同时复位） |
| Ctrl + Z / Ctrl + Y | 撤销 / 重做 |
| G | 显示 / 隐藏透明棋盘格 |
| H | 显示 / 隐藏拼图辅助线 |
| F11 | 切换全屏 / 窗口 |
| ESC | 关闭当前面板 / 退出取色模式 |

### 测试场景
| 快捷键 | 功能 |
|---|---|
| 鼠标左键拖动 | 绘制甲（深色） |
| 鼠标右键拖动 | 绘制乙（浅色） |
| 滚轮 | 缩放 |
| 中键拖动 | 平移 |
| Ctrl + Z / Ctrl + Y | 撤销 / 重做 |
| L | 显示 / 隐藏场景网格线 |
| K | 显示 / 隐藏视觉层网格线 |

## ❓ 常见问题

**Q: 双击 exe 没反应？**
A: 检查是否解压在**全英文路径**下。

**Q: 导出文件在哪？**
A: **桌面**。文件名形如 `拼图_20260914_1.png`。

**Q: 存档存在哪？**
A: `C:\Users\<用户名>\AppData\LocalLow\HuaJiangShan\PixelTileStudio\Saves\`

**Q: 加载存档会提示保存吗？**
A: 有未保存修改时会弹确认。

**Q: 修改层是什么？**
A: 右侧 4×4 拼图上叠加的独立画布，用来画阴影、高光、色调。不影响原始的 6 个源。

**Q: 支持英文界面吗？**
A: **暂不支持**。英文版会在后续更新中推出。

**Q: 有 Mac / Linux 版吗？**
A: **暂无**，目前仅 Windows 版。

## 📧 反馈

遇到 Bug 或有建议，欢迎联系：**huajiangshan001@qq.com**
📌 附上系统版本、分辨率、截图、复现步骤，修复速度提升 100%！

## 📜 许可证

本软件基于 **MIT** 协议开源。
- ✅ 免费使用、修改、分发
- ✅ 允许商业使用，但需保留原作者版权声明
- ❌ 作者不对使用本软件造成的任何损失负责

**本软件完全免费，严禁任何形式的倒卖。**

## 🙏 致谢

感谢所有反馈问题的用户，你们的每一条建议都让这个工具变得更好。

**⭐ 如果这个项目对你有帮助，欢迎给个 Star！**

</details>

<br>

<details>
<summary>👇 <b>Click to expand English documentation (点击展开英文文档)</b></summary>

<br>

## 📖 What is this

Pixel Tile Studio is a painting and composition tool designed specifically for the **Pixel Dual-Grid Tile System**.

**The Dual-Grid Tile System** is a common pixel map design method:
- The map consists of cells, each having two states ("A" and "B").
- Every 2×2 cells combine into a "visual tile", displaying a specific image.
- The 2×2 cell states determine which tile is displayed (16 possible combinations).

**Typical Uses:**
- 🗺️ **Pixel Game Mapping**: Quickly design terrain, walls, and roads using binary grids.
- 🧱 **Tile Asset Testing**: Verify the effects of 16 tile combinations in an actual map.
- 🎨 **Pixel Art Prototyping**: Quickly validate asset pairings and rotation effects.
- 🧩 **Jigsaw Design**: Explore different arrangements of the same asset set.

## 🎯 Where to use

### Scenario 1: Designing Dual-Grid Tile Maps
Draw 6 base tiles (e.g., grass, road, wall corner), and the tool helps you:
- Compose them into a large 4x4 image.
- Preview the effect of different rotation angles in real-time.
- Export as PNG for game engines.

### Scenario 2: Testing Binary Map Layouts
Use the binary grid in the test scene to simulate maps:
- Cells have only two states ("A" / "B").
- Every 2x2 combination automatically selects the corresponding tile.
- Visually see the map under different layouts.

### Scenario 3: Rapid Prototyping of Pixel Assets
Without opening PS, directly in the tool:
- Draw 6 tiles.
- Adjust rotation and composition.
- Export and verify.

## ✨ Core Features

### 🧩 1. 6 Sources + 4×4 Composition
**Draw 6 sources on the left, compose them into a 4x4 image on the right.**

| Feature | Description |
|---|---|
| **6 Independent Sources** | Each source can be drawn separately. |
| **4×4 Composition** | Real-time display on the right, updates instantly. |
| **Independent Rotation** | Each tile can be rotated 0/90/180/270°. |
| **Rotate Source** | Rotate the current source 90° clockwise in the composition. |

### 🖌️ 2. Lighting Modification Layer
**Overlay an independent canvas on the 4×4 composition for shadows, highlights, and tint.**

| Feature | Description |
|---|---|
| **Independent Layer** | Doesn't modify the 6 original sources; can be toggled anytime. |
| **One-click Clear** | Clears the layer; undoable with Ctrl+Z. |
| **Shared Tools** | Brush / Eraser / Bucket, brush size, color, alpha all shared with the left canvas. |
| **Saved with the Project** | Persists across sessions; optional inclusion on export. |
| **Cross-scene** | Carried over to the test scene and reflected in the slices. |

### 🎨 3. Pixel Painting
| Tool | Description |
|---|---|
| **Brush** | Per-pixel drawing, supports 1×1 to 8×8. |
| **Eraser** | Completely erases pixels. |
| **Paint Bucket** | Fills adjacent same-color or blank areas. |
| **Alpha** | 0 ~ 255 adjustable, supports semi-transparency. |
| **Blend Mode** | Optional, mixes brush color with existing pixels. |
| **Undo / Redo** | Up to 50 steps. |

**Canvas sizes**: 8×8 / 16×16 / 32×32 / 64×64

### 🎨 4. Color System
- 16-color preset palette
- Hex / RGB precise input
- 6 quick color slots (one-click switch for common colors)
- **Real-time Color Picker**: hover to preview pixel color; click to pick and sync to brush, alpha, input fields, and quick slots
- Click color text to copy Hex

### 🔍 5. Painting Aids
- **Reference Overlay**: Shows what the current source "should" look like.
- **Checkerboard**: Distinguishes transparency from white (G to toggle).
- **Composition Guides**: Displays 4×4 splits and numbers (H to toggle).
- **Zoom / Pan**: Alt + Scroll / Middle-click drag.
- **Synced Panning**: Shift + middle-click drag pans both canvases together.

### 🧪 6. Test Scene (Dual-Grid Simulation)
**Splits the composition into 16 slices, composed using a binary grid.**

| Feature | Description |
|---|---|
| **Binary Grid** | A (dark) / B (light), drawable. |
| **Visual Layer** | Every 2×2 cells automatically displays the corresponding slice. |
| **Grid Sizes** | 8 / 16 / 32 / 64 / 128. |
| **Grid Toggles** | Scene lines (L) / Visual lines (K) independently toggled. |
| **Slice Source** | Reads the current 4×4 composition in real-time (including modification layer). |
| **Independent Undo** | Ctrl+Z / Ctrl+Y. |

### 💾 7. Save & Export
| Feature | Description |
|---|---|
| **Save / Save As / Load** | Multi-save management. |
| **Export Composition** | Saves the 4×4 composition as PNG (optionally including the modification layer). |
| **Export Sources** | Check sources to export, batch export. |
| **Auto Save to Desktop** | Real desktop path, unaffected by OneDrive. |
| **State Persistence** | Canvas size, modification layer visibility, and test grid size persist across sessions. |

### 🔄 8. Update Checker
Silent check for new versions on startup. Shows a hint on the toolbar when an update is available; no interruption.

## 📥 Installation

1. Download `PixelTileStudio_v1.0.0.zip`
2. **Extract to an English-only path** (e.g., `D:\PixelTileStudio`)
3. Double-click `PixelTileStudio.exe` to run (portable).

**⚠️ Notes**:
- Do NOT extract to a path containing Chinese characters, as it may cause errors.
- Do NOT run the exe directly inside the zip; you must extract it first.

## 🎮 Shortcuts

### Painting Scene
| Shortcut | Function |
|---|---|
| Left-click drag | Paint pixels (left: source, right: modification layer) |
| Alt + Scroll | Zoom canvas |
| Middle-click drag | Pan view |
| Shift + Middle-click drag | Synced panning on both canvases |
| Normal Scroll | Adjust brush size (when mouse is on canvas) |
| F | Reset view (both canvases) |
| Ctrl + Z / Ctrl + Y | Undo / Redo |
| G | Toggle checkerboard background |
| H | Toggle composition guide lines |
| F11 | Toggle fullscreen / windowed |
| ESC | Close current panel / exit color picker |

### Test Scene
| Shortcut | Function |
|---|---|
| Left-click drag | Paint A (dark) |
| Right-click drag | Paint B (light) |
| Scroll | Zoom |
| Middle-click drag | Pan |
| Ctrl + Z / Ctrl + Y | Undo / Redo |
| L | Toggle scene grid lines |
| K | Toggle visual layer grid lines |

## ❓ FAQ

**Q: Nothing happens when I double-click the exe?**
A: Check if you extracted it to an **English-only path**.

**Q: Where are the exported files?**
A: **Desktop**. Filename format: `Composition_20260914_1.png`.

**Q: Where are the saves stored?**
A: `C:\Users\<Username>\AppData\LocalLow\HuaJiangShan\PixelTileStudio\Saves\`

**Q: Does loading a save prompt to save first?**
A: Yes, if there are unsaved changes.

**Q: What is the Modification Layer?**
A: An independent canvas overlaid on the 4×4 composition for shadows, highlights, and tint. It doesn't touch the 6 original sources.

**Q: Is there an English UI?**
A: **Not currently**. English localization is planned for future updates.

**Q: Mac / Linux version?**
A: **Not available yet**. Currently Windows only.

## 📧 Feedback

For bugs or suggestions, please contact: **huajiangshan001@qq.com**
📌 Attach your OS version, resolution, screenshot, and reproduction steps to speed up fixing by 100%!

## 📜 License

This software is open-sourced under the **MIT** License.
- ✅ Free to use, modify, and distribute.
- ✅ Commercial use allowed, but original copyright notice must be retained.
- ❌ The author is not liable for any damages caused by using this software.

**This software is completely free. Reselling is strictly prohibited.**

## 🙏 Acknowledgements

Thanks to all users who provided feedback. Every suggestion makes this tool better.

**⭐ If this project helps you, please give it a Star!**

</details>
