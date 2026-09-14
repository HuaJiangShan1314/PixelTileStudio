# 🎨 像素瓦片工坊 (Pixel Tile Studio)

> 一款免费、轻量的**像素双网格瓦片地图绘制工具**
> **版本 (Version)：v1.0 公开测试版 (Public Beta)**

---

## 📖 这是什么

像素瓦片工坊是一款专为**像素双网格瓦片系统**设计的绘制与组合工具。

**双网格瓦片系统**是一种常见的像素地图绘制方式：
- 地图由格子组成，每个格子有两种状态（用“甲”和“乙”表示）。
- 每 2×2 个格子组合成一个“视觉瓦片”，显示一个具体的图像。
- 2×2 格子的状态决定显示哪个瓦片（共 16 种可能）。

**典型用途：**
- 🗺️ **像素游戏的地图绘制**：用二态网格快速设计地形、墙壁、道路。
- 🧱 **瓦片素材测试**：验证 16 种瓦片组合在实际地图中的效果。
- 🎨 **像素素材原型**：快速验证素材搭配和旋转效果。
- 🧩 **拼图设计**：探索同一组素材的不同排布方式。

---

## ✨ 核心功能

* **🧩 6个源 + 4×4拼图**：左侧绘制6个独立源，右侧实时拼成4×4大图预览。每个拼图块支持独立配置 0/90/180/270° 旋转。
* **🎨 像素绘制**：提供画笔、橡皮、油漆桶；支持 1×1 ~ 8×8 画笔大小；透明度可调，支持混合模式；支持多达 50 步的撤销/重做。
* **🌈 颜色系统**：16色预设调色板，支持 Hex / RGB 精确输入，提供 6 个快捷色槽，点击颜色文本可复制 Hex。
* **🔍 绘制辅助**：参考图层临摹、透明棋盘格背景（G键切换）、拼图辅助线 + 编号（H键切换）、Alt+滚轮缩放、中键平移。
* **🧪 测试场景（双网格模拟）**：将拼图切为 16 个切片并用二态网格组合。网格尺寸提供 8/16/32/64/128 五档。支持场景网格线（L）和视觉层网格线（K）独立切换。
* **💾 存档与导出**：支持多存档管理（保存/另存为/加载）；导出拼图或单/多个源为独立PNG。文件自动保存到桌面，重名自动加编号。

---

## 📥 安装方法

1. 下载 `PixelTileStudio_v1.0.zip`
2. **解压到全英文路径下**（例如 `D:\PixelTileStudio`）
3. 双击 `PixelTileStudio.exe` 运行（免安装，绿色版）

**⚠️ 注意**：
- 不要解压到带中文的路径，可能导致程序异常。
- 不要直接双击 zip 内的 exe，必须解压后再运行。

---

## 🎮 快捷键

### 绘制场景
| 快捷键 | 功能 |
|---|---|
| 鼠标左键拖动 | 绘制像素 |
| Alt + 滚轮 | 缩放画布 |
| 中键拖动 | 平移视图 |
| 普通滚轮 | 调整画笔大小（鼠标在画布内时） |
| F | 复位视图 |
| Ctrl + Z / Ctrl + Y | 撤销 / 重做 |
| G | 显示 / 隐藏透明棋盘格 |
| H | 显示 / 隐藏拼图辅助线 |
| ESC | 关闭当前面板 |

### 测试场景
| 快捷键 | 功能 |
|---|---|
| 鼠标左键拖动 | 绘制格子 |
| 滚轮 | 缩放 |
| 右键拖动 | 平移 |
| L | 显示 / 隐藏场景网格线 |
| K | 显示 / 隐藏视觉层网格线 |

---

## ❓ 常见问题

**Q: 双击 exe 没反应？**
A: 检查是否解压在**全英文路径**下。

**Q: 导出文件在哪？**
A: **桌面**。文件名形如 `拼图_20260914_1.png`。

**Q: 存档存在哪？**
A: `C:\Users\<用户名>\AppData\LocalLow\HuaJiangShan\PixelTileStudio\Saves\`

**Q: 支持英文界面吗？**
A: **暂不支持**。英文版会在后续更新中推出。

**Q: 有 Mac / Linux 版吗？**
A: **暂无**，目前仅 Windows 版。

---

## 📧 反馈

遇到 Bug 或有建议，欢迎联系：**huajiangshan001@qq.com**
📌 附上系统版本、分辨率、截图、复现步骤，修复速度提升 100%！

---

## ❤️ 支持作者

如果这个工具帮到了你，欢迎支持我继续开发。
👉 **[点击这里支持我（爱发电）](https://afdian.com/a/hjs0307)**

---

## 📥 下载

* **GitHub**: 从本仓库的 [Releases](https://github.com/HuaJiangShan1314/PixelTileStudio/releases) 页面下载。
* **国内下载（蓝奏云）**: 👉 **[点击这里去蓝奏云下载（提取码：1vr9）](https://wwamt.lanzout.com/b00rp90vyd)**

---

## 📜 许可证

本软件基于 **MIT** 协议开源。
- ✅ 免费使用、修改、分发
- ✅ 允许商业使用，但需保留原作者版权声明
- ❌ 作者不对使用本软件造成的任何损失负责

**本软件完全免费，严禁任何形式的倒卖。**
详见 [LICENSE](LICENSE) 文件。

---

## 🙏 致谢

感谢所有反馈问题的用户，你们的每一条建议都让这个工具变得更好。

**⭐ 如果这个项目对你有帮助，欢迎给个 Star！**

<details>
<summary>👇 <b>Click here to expand English documentation (点击展开英文文档)</b></summary>

<br>

# 🎨 Pixel Tile Studio

> A free, lightweight **pixel dual-grid tile map painting tool**.
>
> **Version: v1.0 Public Beta**

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

## ✨ Core Features

* **🧩 6 Sources + 4×4 Composition**: Draw 6 independent sources on the left, preview the 4×4 composition in real-time on the right. Each tile supports independent rotation (0/90/180/270°).
* **🎨 Pixel Painting**: Brush, Eraser, Paint Bucket; brush sizes from 1×1 to 8×8; adjustable alpha for semi-transparent pixels; optional blend mode; Undo/Redo up to 50 steps.
* **🌈 Color System**: 16-color preset palette; Hex/RGB precise input; 6 quick color slots; click color text to copy Hex.
* **🔍 Painting Aids**: Reference overlay, checkerboard background (G to toggle), composition guide lines + numbers (H to toggle), Zoom (Alt + scroll) / Pan (middle mouse).
* **🧪 Test Scene (Dual-Grid Simulation)**: Splits the composition into 16 slices on a binary grid. Grid sizes: 8/16/32/64/128. Independent toggles for scene grid lines (L) and visual layer lines (K).
* **💾 Save & Export**: Multi-save management (Save/Save As/Load); Export composition or single/multiple sources as PNGs. Files are saved to the Desktop with auto-numbering.

## 📥 Installation

1. Download `PixelTileStudio_v1.0.zip`
2. **Extract to an English-only path** (e.g., `D:\PixelTileStudio`)
3. Double-click `PixelTileStudio.exe` to run (portable, no installation needed).

**⚠️ Notes:**
- Do NOT extract to a path containing Chinese characters, as it may cause errors.
- Do NOT run the exe directly inside the zip; you must extract it first.

## 🎮 Shortcuts

### Painting Scene
| Shortcut | Function |
|---|---|
| Left-click drag | Paint pixels |
| Alt + Scroll | Zoom canvas |
| Middle-click drag | Pan view |
| Normal Scroll | Adjust brush size (when mouse is on canvas) |
| F | Reset view |
| Ctrl + Z / Ctrl + Y | Undo / Redo |
| G | Toggle checkerboard background |
| H | Toggle composition guide lines |
| ESC | Close current panel |

### Test Scene
| Shortcut | Function |
|---|---|
| Left-click drag | Paint cells |
| Scroll | Zoom |
| Right-click drag | Pan |
| L | Toggle scene grid lines |
| K | Toggle visual layer grid lines |

## ❓ FAQ

**Q: Nothing happens when I double-click the exe?**
A: Check if you extracted it to an **English-only path**.

**Q: Where are the exported files?**
A: **Desktop**. Filename format: `Composition_20260914_1.png`.

**Q: Where are the saves stored?**
A: `C:\Users\<Username>\AppData\LocalLow\HuaJiangShan\PixelTileStudio\Saves\`

**Q: Is there an English UI?**
A: **Not currently**. English localization is planned for future updates.

**Q: Mac / Linux version?**
A: **Not available yet**. Currently Windows only.

## 📧 Feedback

For bugs or suggestions, please contact: **huajiangshan001@qq.com**
📌 Attach your OS version, resolution, screenshot, and reproduction steps to speed up fixing by 100%!

## ❤️ Support the Author

If this tool helps you, feel free to support my development.
👉 **[Click here to support me (Afdian)](https://afdian.com/a/hjs0307)**

## 📥 Download

* **GitHub**: Download from the [Releases](https://github.com/HuaJiangShan1314/PixelTileStudio/releases) page of this repository.
* **Domestic (China)**: 👉 **[Download from Lanzou Cloud (Password: 1vr9)](https://wwamt.lanzout.com/b00rp90vyd)**

## 📜 License

This software is open-sourced under the **MIT** License.
- ✅ Free to use, modify, and distribute.
- ✅ Commercial use allowed, but original copyright notice must be retained.
- ❌ The author is not liable for any damages caused by using this software.

**This software is completely free. Reselling is strictly prohibited.**
See the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgements

Thanks to all users who provided feedback. Every suggestion makes this tool better.

**⭐ If this project helps you, please give it a Star!**

</details>
