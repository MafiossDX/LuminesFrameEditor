# Lumines Frame Editor

`Lumines Frame Editor` 是一个单文件工具，用于逐帧排列 Lumines 版面状态，以便按照你的节奏来回顾和分析。你可以手动重新绘制棋盘，添加或复制帧，并回放以直观地跟踪摆块顺序和版面变化。

为便于发布到 GitHub Pages，该工具用单个文件`lumines_frame_editor.html`实现。

URL: [https://mafiossdx.github.io/LuminesFrameEditor/lumines_frame_editor.html](https://mafiossdx.github.io/LuminesFrameEditor/lumines_frame_editor.html)

## 功能

- 编辑 `16 x 10` 的固定版面
- 摆放方格，有 6 种颜色和一种垃圾格
- 添加、复制、删除和清空帧
- 在时间轴上移动帧并按序播放
- 给每一帧添加备注
- 只为当前帧中最大的一个 `3x3` 及以上 BURST 形状显示边框
- 将当前帧导出为 PNG
- 使用 `Ctrl+V` 粘贴游戏截图，选择版面所处的范围，将其导入当前帧
- 显示当前版面中正方形的数量
  - `Normal`: 2x2
  - `BURST`: 2x2 及更大

## 如何使用

1. 在浏览器中打开 `lumines_frame_editor.html`。
2. 在左侧选择一个颜色，点击或划动鼠标以绘制方格。
3. 使用 `Add` 或 `Duplicate` 添加帧，如有必要可以在 `Caption` 中添加备注。
4. 点击 `Play` 按序观看所有帧。
5. 如果需要，可以先开启 `BURST枠を表示`，再点击 `Export PNG`。
如果要从图像中导入版面，复制游戏截图，在页面上按下 `Ctrl+V`，在右侧预览中拖动鼠标选择版面区域，然后点击 `Import From Image`。页面自动检测颜色，但不准确，因此通常需要手动调整。

## 操作方式

- 左键：绘制
- 右键：擦除
- 左右箭头：切换当前帧
- 空格：播放/暂停
- `N`：添加新的空白帧
- `D`：复制当前帧

## 文件结构

- `lumines_frame_editor.html`：程序本体
- `README.md`: 日文 README
- `README.en.md`: 英文 README
- `README.cns.md`: 简体中文 README

## 用途

此工具并非用于解开，而是用于记录 Lumines 版面，以便日后回顾和讨论。它适用于赛后复盘、策略笔记、方块摆法分析，以及分享版面随时间推移的变化。
