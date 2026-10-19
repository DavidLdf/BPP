# BPP Batch Plot Plugin (for AutoCAD 2027)

[English](#bpp-batch-plot-plugin-for-autocad-2027) | [中文](#bpp-批量打印插件适用于-autocad-2027)

BPP is a batch plotting plugin for AutoCAD. It automatically detects drawing frames, plots all sheets in model space and every layout in order to PDF, image files, or directly to a printer in one run, and can batch-process multiple DWG files at once.

> This plugin is a third-party tool.

## Features

- **Frame detection**: supports block frames, TArch frames (polylines), rectangles on specified layers, and "All (smart recognition)" — frame library blocks + rectangles / four-line rectangles on any layer + layout viewports, with automatic sheet size detection (including extended sizes).
- **Job list**: generates a list after scanning; check/uncheck, reorder, preview, and zoom to frames; automatically reads drawing number, title, revision, date, and other fields.
- **Sort settings**: sort by drawing number / sheet position / title / project; 8 position directions + snake order; configurable sort base point, row/column tolerance, current UCS direction, and grouping by sheet size / block name / layer; optionally renumber drawings in the final order.
- **Multi-document batch plot (BPPM)**: processes multiple DWG/DXF files at once, building a single plot list and plotting file by file.
- **Output**: PDF, JPG/PNG (configurable DPI), DWF, and any printer; PDFs can be merged by all / same drawing number / same project / paper size; output can be saved in per-file folders as "source folder\PDF\document name".
- **File naming and drawing index**: generates file names from naming rules; can insert a drawing index table into the drawing.
- **Others**: plot stamp, extended sheets, automatic paper matching, rotate all to landscape/portrait (optionally keep A4 unrotated), Chinese/English UI switch (en/cn button in the title bar).

## Requirements

| Item | Requirement |
|---|---|
| AutoCAD | **AutoCAD 2027** (64-bit); vertical products built on the 2027 platform (Architecture, Mechanical, etc.) should work |
| Not supported | AutoCAD 2026 and earlier, ZWCAD and other CAD platforms |
| OS | Windows 10 / 11 64-bit |

## Installation

1. Download the latest `BPP-v*-AutoCAD2027.zip` from **Releases** on the right side of this page.
2. Extract it to a permanent folder, e.g. `D:\CADPlugins\BPP\` (do not move it afterwards or copy only a single DLL — keep all files in the folder).
3. Start AutoCAD 2027, type `NETLOAD`, and select `BPP.dll` in that folder.

> On the first NETLOAD, Windows may warn that the file came from the internet: right-click `BPP.dll` → Properties → check "Unblock", then load it again.

## License

The plugin stops working automatically when the trial license expires. Licenses are bound to the machine; after changing computers or reinstalling Windows, request a new license with the new machine ID.

## Commands

| Command | Description |
|---|---|
| `BPP` | Open the batch plot main dialog |
| `BPPMULTI` | Open multi-document batch plot |
| `BPPRESET` | Reset plugin settings to defaults |

## FAQ

**Flagged or blocked by antivirus?**
The plugin is protected against cracking, which some antivirus software may falsely flag. Download only from Releases on this page and verify the SHA256 checksum of the zip (listed in each Release's notes); once confirmed, add the plugin folder to your antivirus trusted list.


## License Agreement

By using this plugin you agree to the [License Agreement](使用协议.md) (bilingual; the English version follows the Chinese).

---

# BPP 批量打印插件（适用于 AutoCAD 2027）

BPP 是一款 AutoCAD 批量打印插件：自动识别图纸中的图框，一次性把模型空间和各布局里的全部图纸按顺序打印成 PDF、图片或直接送打印机，并支持多个 DWG 文件一起批量处理。

> 本插件为第三方工具。

---

## 主要功能

- **图框识别**：支持图块图框、天正图框(多段线)、指定图层矩形，以及"所有(智能识别)"——图框信息库块 + 任意图层矩形/四线矩形 + 布局视口，自动判定图幅(含加长图纸)。
- **任务清单**：扫描后生成清单，可勾选、调整顺序、预览、定位到图框；自动读取图号、图名、版次、日期等字段。
- **排序设置**：按图号 / 图纸位置 / 图名 / 项目排序，8 种位置方向 + 蛇形排序，可设排序基点、行列容差、按 UCS 方向、按图幅/块名/图层分组；可同时按最终顺序重排图号。
- **多文档批打(BPPM)**：一次处理多个 DWG/DXF，统一生成待打印清单后逐文件出图。
- **输出**：PDF、JPG/PNG(可设 DPI)、DWF 及各类打印机；PDF 可按全部/同图号/同项目/纸张大小合并；输出可按"源文件路径\PDF\文档名称"分目录存放。
- **文件命名与图纸目录**：按命名规则生成文件名；可在图中插入图纸目录表格。
- **其它**：打印戳记、加长图纸、自动匹配纸张、全转横向/竖向(可保持 A4 不旋转)、中英文界面切换(标题栏 en/cn 按钮)。

## 运行环境

| 项目 | 要求 |
|---|---|
| AutoCAD | **AutoCAD 2027**(64 位)；基于 2027 平台的专业版(Architecture、Mechanical 等)理论上可用 |
| 暂不支持 | AutoCAD 2026 及更早版本、中望 CAD 等其它 CAD 平台 |
| 系统 | Windows 10 / 11 64 位 |

## 安装

1. 从本页右侧 **Releases** 下载最新的 `BPP-v*-AutoCAD2027.zip`。
2. 解压到一个固定文件夹，例如 `D:\CADPlugins\BPP\`(解压后不要移动或只拷贝单个 DLL，文件夹里的全部文件都要保留)。
3. 打开 AutoCAD 2027，输入 `NETLOAD`，选择文件夹里的 `BPP.dll`。

> 首次 NETLOAD 时 Windows 可能提示"来自网络的文件"：在 `BPP.dll` 上右键 → 属性 → 勾选"解除锁定"后再加载。

## 授权

试用授权到期后插件会自动停止工作。授权与机器绑定，更换电脑或重装系统后需用新机器码重新申请。

## 命令

| 命令 | 说明 |
|---|---|
| `BPP` | 打开批量打印主对话框 |
| `BPPMULTI` | 打开多文档批量打印 |
| `BPPRESET` | 把插件设置恢复为默认值 |


## 常见问题

**杀毒软件报毒 / 拦截？**
插件为防止破解做了加密保护，部分杀毒软件可能误报。请从本页 Releases 下载，并核对压缩包的 SHA256 校验值(见每个 Release 的说明)；确认无误后可将插件文件夹加入杀毒软件信任列表。


## 使用协议

使用本插件即表示同意 [使用协议](使用协议.md)。
