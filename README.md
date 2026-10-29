# 🎨 像素瓦片工坊 (Pixel Tile Studio) v2.0.0

> **一款免费、轻量的像素双网格瓦片地图绘制工具**
> **支持正方形与 2:1 等距双模式，画几张源图，直接测出整张地图。**
>
> *A free, lightweight pixel dual-grid tile map painting tool.*
> *Supports Square and Isometric modes.*

---

## 📑 目录 (Table of Contents)

- [🚀 V2.0 重点更新](#-v20-重点更新)
- [📥 下载与安装](#-下载与安装-download--installation)
- [📖 这是什么](#-这是什么)
- [✨ 核心功能](#-核心功能)
- [🎮 快捷键](#-快捷键)
- [❓ 常见问题](#-常见问题-v2-补充版)
- [🔄 V1 → V2 升级说明](#-v1--v2-升级说明)
- [📜 许可证](#-许可证)

---

## 🚀 V2.0 重点更新

- **新增 2:1 等距模式**：4 个三角源 + 4 个平行四边形源自动拼合大菱形，支持独立旋转与 V 形辅助线。
- **画布尺寸上限扩展至 128×128**：编辑器画布从原有的 64 上限提升至 128，满足更复杂的像素地图需求。
- **自动保存更安心**：1.5 秒防抖自动保存草稿，切场景、关闭软件、意外闪退都不容易丢进度。
- **左右独立撤销**：源画布和光照修改层各有一套撤销栈。鼠标在哪边，`Ctrl+Z` 就作用于哪边，绝不串台。
- **存档物理隔离**：正式存档、伴生草稿、无名草稿分目录存放，彻底杜绝误删覆盖的风险。
- **加密分享 `.pxtile`**：带签名防篡改，支持批量导入导出，导入时自动分配新 ID 防冲突。
- **底层渲染重写**：修复了缩放时像素网格线断开、发暗、发糊的问题。
- **防误触保护**：打开任何弹窗或面板时，底层画布快捷键与画笔输入自动失效。

---

## 📥 下载与安装 (Download & Installation)

- **国内蓝奏云 (极速推荐) / Lanzou Cloud (Recommended for China)**: [点击这里去蓝奏云下载（提取码：1vr9）](https://wwamt.lanzout.com/b00rp90vyd)
- **GitHub**: [点击这里去 Releases 页面下载](https://github.com/HuaJiangShan1314/PixelTileStudio/releases) *(Download from the Releases page)*

**安装方法 / Installation**:
1. 解压到**全英文路径**下 / *Extract to an English-only path.*
2. 双击 `PixelTileStudio.exe` 运行（免安装） / *Double-click to run (portable).*

**💻 系统要求 (System Requirements)**:
- Windows 10 / 11（64 位）。无需安装 .NET 或任何运行库，纯绿色版。
- 建议屏幕分辨率：1920×1080 及以上。

---

<details>
<summary>👇 <b>点击展开详细中文文档 (Click to expand Chinese documentation)</b></summary>

<br>

## 📖 这是什么

像素瓦片工坊是一款专为**像素双网格瓦片系统**设计的绘制与组合工具。

**它解决什么问题**：传统地形过渡要手绘 16 张（或更多）瓦片，还得到引擎里试才知道效果。用双网格 + 旋转归并，**极少的源图就能覆盖全部组合**，工具里直接切测试场景验证。

**适合谁**：像素游戏地图绘制、瓦片素材测试、等距原型设计、拼图逻辑验证。

**和其他瓦片工具的不同**：
- 别的工具帮你“拼”已经画好的瓦片；这个工具帮你**用最少的源图**生成所有需要的瓦片。
- 别的工具要来回切到引擎；这个工具**内置测试场景**，画完立刻看效果。

## ✨ 核心功能

### 🧩 一、双模式拼图
**左侧画源，右侧拼合。**

| 功能 | 说明 |
|---|---|
| **正方形模式** | 6 个独立源，右侧拼成 4×4 大图 |
| **等距模式** | 4 个三角源 + 4 个平四源，拼合成大菱形 |
| **V 形辅助线** | 等距模式专属，帮助对齐透视与几何位置 |
| **独立旋转** | 每个拼图块可独立旋转 0 / 90 / 180 / 270° |
| **实时预览** | 改一笔，右侧立刻变 |

> **💡 等距模式怎么画？**
> 左侧会显示 4 个三角形源和 4 个平行四边形源。先在三角源上画地面/墙面，再在平四源上画过渡面；右侧大菱形会实时拼合。

### 🖌️ 二、像素绘制与交互
| 工具 | 说明 |
|---|---|
| **画笔 / 橡皮 / 油漆桶** | 逐像素绘制，支持 1×1 ~ 8×8 |
| **直线辅助** | 按住 `Shift` + 拖动，动态拉直线 |
| **防误触取消** | 画错了？左键不松点一下右键，瞬间回退整笔 |
| **独立撤销栈** | 左侧源、右侧修改层各自拥有独立栈，随鼠标悬停自动切换焦点 |

**画布尺寸**：8×8 / 16×16 / 32×32 / 64×64 / 128×128

### 🖌️ 三、光照修改层
**在拼图上叠加一层独立画布，用于绘制阴影、高光、色调等整体效果。**
- **独立图层**：不污染原始源图，随时显隐。
- **随存档保存**：修改层内容随存档保留，导出时可选包含或不包含。

### 🎨 四、颜色与辅助
- **颜色系统**：32色预设调色板、Hex/RGB 输入、6 个快捷色槽（支持拖拽重排）。
- **快捷取色**：按住 `Alt` 键临时切换为吸管取色。
- **防误触保护**：打开弹窗或面板时，底层画布和快捷键自动锁定。
- **辅助线**：参考图层（带甲乙标记）、透明棋盘格、拼图分割线、像素网格。
- **视图控制**：滚轮缩放，空格+左键或中键拖动平移。

### 🧪 五、测试场景（双网格模拟）
**把拼图切分，用二态网格组合验证。**
- 格子只有"甲/乙"两种状态，可自由涂色。
- 每 2×2 格子自动显示对应切片（包含修改层）。
- 支持 8 / 16 / 32 / 64 / 128 多档网格尺寸。

### 💾 六、存档与分享
| 功能 | 说明 |
|---|---|
| **全自动保存** | 防抖 1.5 秒自动存草稿，切场景、意外闪退不丢失 |
| **多存档管理** | 保存 / 另存为 / 加载 / 重命名 / 删除 |
| **物理级隔离** | 自动区分“未命名草稿”与“正式存档伴生草稿”，杜绝误删 |
| **加密分享** | 一键导出 `.pxtile` 分享文件（自带签名防篡改），支持批量导入/导出 |
| **导入冲突处理** | 导入重复文件时，保留最新修改的那份，其余自动重命名，不会互相覆盖 |
| **导出 PNG** | 导出源图或拼图到桌面，文件名形如 `拼图_YYYYMMDD_N.png` |

## 🎮 快捷键

### 绘制场景
| 快捷键 | 功能 |
|---|---|
| **Q / W / E** | 切换 画笔 / 橡皮 / 油漆桶 |
| **F** | 显示 / 隐藏 调色盘面板 |
| **Shift + 左键拖动** | 画直线 |
| **左键拖动中 + 右键** | 瞬间取消当前笔画 |
| **Alt（按住）** | 临时切换为吸管取色 |
| **Tab（按住）** | 临时切回上一个使用过的工具 |
| **Z（按住）** | 强制显示像素网格 |
| **S / D** | 开关像素网格 / 复位视图 |
| **滚轮 / Ctrl + 滚轮** | 缩放画布 / 调整画笔大小 |
| **空格 + 左键 / 中键拖动** | 平移视图 |
| **Ctrl + Z / Ctrl + Y / Ctrl+Shift+Z** | 撤销 / 重做 |
| **Ctrl + S / Ctrl + O / Ctrl + E** | 保存 / 加载 / 导出 |
| **F11 / ESC** | 全屏 / 关闭当前面板 |

### 测试场景
| 快捷键 | 功能 |
|---|---|
| **鼠标左键拖动** | 绘制甲（深色） |
| **鼠标右键拖动** | 绘制乙（浅色） |
| **滚轮 / 中键拖动** | 缩放 / 平移 |
| **Ctrl + Z / Ctrl + Y** | 撤销 / 重做 |

## ❓ 常见问题 (V2 补充版)

**Q: 杀毒软件报毒 / 被拦截怎么办？**
A: 本工具为免费绿色版，且底层接入了代码混淆保护，部分杀软（如 Windows Defender / 360）可能会误报。请将安装目录加入信任区，或从 GitHub Releases 重新下载核对。**请不要从第三方站点下载。**

**Q: 双击 exe 没反应？**
A: 检查是否解压在**全英文路径**下。

**Q: 自动保存的草稿在哪恢复？**
A: 正常进入编辑器或打开加载面板时，如果有未保存的进度，系统会自动弹窗询问你是否恢复。

**Q: `.pxtile` 是什么？安全吗？**
A: 这是 V2 新增的专属分享格式。它经过压缩和 HMAC 签名防篡改，导入时会自动分配新 ID，不会覆盖你现有的存档。

**Q: V1 的老存档还能用吗？**
A: 完全可以。V2 在加载老存档时会自动无感升级格式，并保留原文件备份。

**Q: 存档存在哪？怎么彻底卸载？**
A: 游戏本体直接删除解压目录即可。如果你想把存档也删干净，请删除 `C:\Users\<用户名>\AppData\LocalLow\HuaJiangShan\PixelTileStudio` 文件夹。

## 🔄 V1 → V2 升级说明

- **完全兼容**：V1 版本的旧存档（`.json`）在 V2 中打开时，会自动进行安全升级并备份原文件。
- **目录变更**：存档体系进行了重构。正式存档在 `Saves/` 根目录，未保存的草稿被迁移至独立的 `Drafts` 文件夹中，互不干扰。

## 📧 反馈

遇到 Bug 或有建议，欢迎联系：**huajiangshan001@qq.com**
📌 **反馈模板**（复制填写即可，附上截图修复速度提升 100%）：
- 系统版本 / 分辨率：
- 操作步骤：
- 预期结果 / 实际结果：
- 截图或录屏：

## 📜 许可证

**Copyright (c) 2026 HuaJiangShan1314. All Rights Reserved.**

本软件为免费软件，仅供个人学习与使用。

- ✅ **免费使用**：个人学习、娱乐、非商业用途。
- ❌ **禁止商用**：严禁任何形式的倒卖、二次打包售卖或用于商业用途。
- ❌ **禁止篡改**：严禁删除或修改本软件内的版权声明与打赏链接。
- ❌ **免责声明**：本软件按“原样”提供，作者不对使用本软件造成的任何损失负责。

**本软件完全免费，严禁任何形式的倒卖。**

## 🙏 致谢

感谢所有反馈问题的用户，你们的每一条建议都让这个工具变得更好。
**⭐ 如果这个项目对你有帮助，欢迎给个 Star！**

</details>

<br>

<details>
<summary>👇 <b>点击展开 V2.0 详细更新日志 / 技术细节 (Click to expand Changelog)</b></summary>

<br>

### 🛠️ 底层架构重构 (Refactoring)
- **输入路由系统**：重构了全局输入分发，采用三层路由逻辑，解决按键冲突。
- **多栈撤销管理**：支持多源独立历史栈，引入悬停焦点防抖与右键强切逻辑，跨场景保留历史。
- **渲染层重写**：重写网格线渲染，引入抗锯齿与平滑淡出；大幅降低 GC 开销。
- **防误触机制**：改为面板自注册模式。所有弹窗和 UI 面板打开时，自动阻断底层画布输入。

### 💾 存档系统重构 (Save System)
- **目录物理隔离**：彻底废弃前缀猜测法，使用 `Saves/`、`Saves/Drafts/`、`Drafts/` 三个独立目录。
- **ID 冲突自愈**：导入 `.pxtile` 时立即分配新 GUID；启动索引时如遇副本冲突，按修改时间保留最新，其余分配新 ID 并写回。
- **索引双向验证**：弃用内存覆盖逻辑，永远以磁盘文件为主，写回采用原子写入。

### 🎨 体验与交互 (UX)
- **动态直线与取消**：新增 `Shift` 动态直线回溯绘制，支持左键拖动期间使用右键瞬间差分回滚当前笔触。
- **快捷色槽拖拽**：快捷色槽支持长按拖拽排序，悬停时支持滚轮无缝切色。
- **重命名交互**：双击列表名字触发重命名输入框，超长名字自动中间截断。
- **测试场景补齐**：等距测试场景补齐了撤销/重做栈功能。

### 🔒 构建与发布 (Build)
- **代码混淆**：接入 Obfuscar，并在构建流程中增加原始 DLL 备份与恢复钩子，防止污染开发环境。
- **构建加固**：版权声明强制打入 IL2CPP，防止程序集属性被剥离。

</details>

<br>

<details>
<summary>👇 <b>Click to expand English documentation (点击展开英文文档)</b></summary>

<br>

## 🚀 V2.0 Highlights

- **2:1 Isometric Mode**: Compose 4 triangles + 4 parallelograms into a large diamond, with V-shape guides.
- **Canvas expanded to 128×128**: Editor canvas now supports up to 128x128.
- **Auto-Save**: 1.5s debounce auto-saves drafts. Never lose progress.
- **Multi-stack Undo**: Independent undo stacks for left and right canvases, switching seamlessly by mouse hover.
- **Directory Isolation**: Saves, companion drafts, and unnamed drafts are strictly separated.
- **Encrypted Share `.pxtile`**: Export/import with HMAC signatures and automatic ID conflict resolution.
- **Rendering Overhaul**: Fixed pixel grid lines breaking, darkening, and blurring when zooming.
- **Global Input Blocker**: Shortcuts and painting are disabled when panels or dialogs are open.

## 📖 What is this

Pixel Tile Studio is a painting and composition tool designed specifically for the **Pixel Dual-Grid Tile System**.

**The problem it solves**: Traditional terrain transitions require hand-drawing 16 (or more) tiles, and you need to test them in an engine. With dual-grid + rotation merging, **minimal source tiles cover every combination** — and you can validate the result directly in the built-in test scene.

**Supports two modes in V2.0**:
- **Square Mode**: 6 rectangular sources composed into a 4×4 map.
- **Isometric Mode**: 8 sources (4 triangles + 4 parallelograms) composed into a large diamond and V-shapes.

## ✨ Core Features

### 🧩 1. Dual-Mode Composition
| Feature | Description |
|---|---|
| **Square Mode** | 6 sources, composed into a 4×4 image. |
| **Isometric Mode** | 4 triangles + 4 parallelograms, composed into a diamond. |
| **V-Shape Guides** | Isometric mode exclusive, helps align perspective. |
| **Independent Rotation** | Each tile can be rotated independently. |
| **Real-time** | Instantly updates as you paint. |

### 🎨 2. Pixel Painting
| Tool | Description |
|---|---|
| **Brush / Eraser / Bucket** | Standard pixel drawing tools. |
| **Shift + Drag** | Draw dynamic straight lines. |
| **Right-click during stroke** | Cancel the entire stroke instantly. |
| **Multi-stack Undo** | Independent undo stacks for left and right canvases. |

**Canvas sizes**: 8x8 to 128x128.

### 🖌️ 3. Lighting Modification Layer
- **Independent Layer**: Overlay for shadows and highlights without touching originals.
- **Saved**: Persists across sessions.

### 🎨 4. Color & Aids
- Preset palettes + custom colors.
- Hex / RGB input, Quick Slots.
- **Alt to pick color**.
- Reference Overlay, Checkerboard, Guides, Pixel grid.
- **Input Blocker**: Panels automatically disable underlying canvas input.

### 🧪 5. Test Scene
- Binary grid layout (A / B).
- Real-time visual slices.
- Grid sizes from 8 to 128.

### 💾 6. Save & Share (V2 Major Refactor)
| Feature | Description |
|---|---|
| **Auto-Save** | 1.5s debounce auto-saves drafts. |
| **Directory Isolation** | Saves and drafts are strictly separated. |
| **Encrypted Share** | Export `.pxtile` files with HMAC signatures. |
| **Export PNG** | Export sources or composition to Desktop. |

## 🎮 Shortcuts

### Painting Scene
| Shortcut | Function |
|---|---|
| **Q / W / E** | Brush / Eraser / Bucket |
| **F** | Toggle Palette Panel |
| **Shift + Left Drag** | Draw straight line |
| **Right-click during Left Drag** | Cancel current stroke |
| **Alt (Hold)** | Temporary color picker |
| **Tab (Hold)** | Switch to previous tool |
| **Z (Hold)** | Force pixel grid |
| **S / D** | Toggle pixel grid / Reset view |
| **Scroll / Ctrl + Scroll** | Zoom / Adjust brush size |
| **Space + Left Drag / Middle Drag** | Pan view |
| **Ctrl + Z / Y / Shift+Z** | Undo / Redo |
| **Ctrl + S / O / E** | Save / Load / Export |
| **F11 / ESC** | Fullscreen / Close Panel |

### Test Scene
| Shortcut | Function |
|---|---|
| **Left-click drag** | Paint A (dark) |
| **Right-click drag** | Paint B (light) |
| **Scroll / Middle Drag** | Zoom / Pan |
| **Ctrl + Z / Ctrl + Y** | Undo / Redo |

## ❓ FAQ

**Q: Antivirus flagged the exe as a threat?**
A: This is a false positive. The tool is obfuscated for code protection. Please add the folder to your whitelist or redownload from GitHub Releases.

**Q: What is `.pxtile`? Is it safe?**
A: It's V2's share format with GZip compression and HMAC signature. Importing always assigns a new ID, so it won't overwrite your existing saves.

**Q: How do I recover an auto-saved draft?**
A: When you open the editor or the load panel, the tool will prompt you to restore unsaved progress if a draft exists.

**Q: Where are the saves stored?**
A: `C:\Users\<Username>\AppData\LocalLow\HuaJiangShan\PixelTileStudio\Saves\`.
To completely uninstall, just delete the extracted folder and this AppData folder.

**Q: Are v1 saves compatible?**
A: Yes. V2 automatically upgrades and backs up older formats upon loading. Save directories have been restructured for better isolation.

**Q: What is the Modification Layer?**
A: An independent canvas overlaid on the composition for shadows and highlights.

## 📧 Feedback
Contact: **huajiangshan001@qq.com**

## 📜 License
**Copyright (c) 2026 HuaJiangShan1314. All Rights Reserved.**
This software is provided free of charge for personal, non-commercial use only.

- ✅ **Free to use**: For personal, educational, and non-commercial purposes.
- ❌ **No Commercial Use**: Any form of resale, repackaging for sale, or commercial use is strictly prohibited.
- ❌ **No Modification of Notices**: Removing or altering the copyright notice or donation link is strictly prohibited.
- ❌ **Disclaimer**: The software is provided "as is", without warranty of any kind.

**This software is completely free. Reselling is strictly prohibited.**

## 🙏 Acknowledgements
Thanks to all users who provided feedback. Every suggestion makes this tool better.
**⭐ If this project helps you, please give it a Star!**

</details>
